# Kernel-Custom-6.16.0-unknown1337+

Custom Linux Kernel 6.16.0 by unknown1337

---

## 📦 **Isi Repo (Bahasa Indonesia)**

- `vmlinuz-6.16.0-unknown1337+`  → Kernel image
- `initramfs-6.16.0-unknown1337+.img`  → (Opsional) Initramfs (kalau ada)
- `System.map-6.16.0-unknown1337+`  → Kernel symbol table
- `config-6.16.0-unknown1337+`  → Config kernel waktu build

---

## ✨ **Fitur / Perubahan**
- Build custom dengan EXTRAVERSION: `-unknown1337+`
- Kernel versi **6.16.0**
- Cocok untuk eksperimen, testing, & security tuning (misal anti-rootkit)
- Konfigurasi sudah dipatch buat kebutuhan advanced user

---

## 🧑‍💻 **Install Manual**

> **PENTING:** Backup kernel & bootloader sebelum replace kernel default!

1. **Copy file ke `/boot`**
    ```sh
    sudo cp vmlinuz-6.16.0-unknown1337+ /boot/
    sudo cp System.map-6.16.0-unknown1337+ /boot/
    sudo cp config-6.16.0-unknown1337+ /boot/
    sudo cp initramfs-6.16.0-unknown1337+.img /boot/   # kalau ada
    ```

2. **Update GRUB / Bootloader**
    ```sh
    sudo grub-mkconfig -o /boot/grub/grub.cfg
    ```

3. **Reboot**, lalu pilih kernel baru di menu boot.

---

## ❓ **FAQ**

- **Q:** _Aman install kernel custom ini buat daily driver?_
  - **A:** Aman selama sudah backup & siap kemungkinan error/kernel panic.

- **Q:** _Bisa request patch/module lain?_
  - **A:** Buka Issue/PR di repo!

---

## 📢 **Kredit**

- Build: [unknown1337](https://github.com/PsychoH4x0r)
- Kernel: [kernel.org](https://kernel.org)

---

## LICENSE

GPLv2 (mengikuti lisensi Linux Kernel)

---

# English Version

Custom Linux Kernel 6.16.0 by unknown1337

---

## 📦 **Repository Contents**

- `vmlinuz-6.16.0-unknown1337+`  → Kernel image
- `initramfs-6.16.0-unknown1337+.img`  → (Optional) Initramfs (if present)
- `System.map-6.16.0-unknown1337+`  → Kernel symbol table
- `config-6.16.0-unknown1337+`  → Kernel build configuration

---

## ✨ **Features / Changes**
- Custom build with EXTRAVERSION: `-unknown1337+`
- Kernel version: **6.16.0**
- Suitable for experiments, testing, and security tuning (e.g., anti-rootkit)
- Config already patched for advanced users

---

## 🧑‍💻 **Manual Installation**

> **IMPORTANT:** Backup your current kernel and bootloader before replacing your default kernel!

1. **Copy files to `/boot`**
    ```sh
    sudo cp vmlinuz-6.16.0-unknown1337+ /boot/
    sudo cp System.map-6.16.0-unknown1337+ /boot/
    sudo cp config-6.16.0-unknown1337+ /boot/
    sudo cp initramfs-6.16.0-unknown1337+.img /boot/   # if present
    ```

2. **Update GRUB / Bootloader**
    ```sh
    sudo grub-mkconfig -o /boot/grub/grub.cfg
    ```

3. **Reboot** and select the new kernel from the boot menu.

---

## ❓ **FAQ**

- **Q:** _Is it safe to use this custom kernel for daily use?_
  - **A:** Safe as long as you’ve backed up your kernel & bootloader and are prepared for possible kernel panic or issues.

- **Q:** _Can I request other patches/modules?_
  - **A:** Open an Issue/PR on this repo!

---

## 📢 **Credits**

- Built by: [unknown1337](https://github.com/PsychoH4x0r)
- Upstream kernel: [kernel.org](https://kernel.org)

---

## LICENSE

GPLv2 (follows the official Linux Kernel license)
