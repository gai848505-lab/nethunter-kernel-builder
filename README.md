# Kali NetHunter Custom Kernel Builder (Automated GitHub Actions)

Dự án tự động biên dịch Kernel Kali NetHunter cho:
1. **LG V50 ThinQ** (`flashlmdd`, Snapdragon 855 / SM8150 - Linux Kernel 4.14)
2. **Asus ZenFone Max Pro M1** (`X00TD` / `ZB601KL` / `ZB602KL`, Snapdragon 636 / SDM660 - Linux Kernel 4.4)

---

## ⚡ Tính năng được tích hợp trong Kernel (Full NetHunter Support)
* **Wireless Injection & Monitor Mode:** Hỗ trợ `mac80211`, `cfg80211` và nạp driver cho các card USB Wi-Fi phổ biến (`Atheros ath9k_htc`, `Realtek rtl8187`, `rtl8812au`, `Ralink rt2800usb`, `Mediatek mt7601u`).
* **HID Attack (BadUSB):** Giả lập bàn phím/chuột qua cáp USB để chạy các script Ducky payload.
* **Chroot Namespaces:** Đầy đủ IPC, UTS, PID, NET namespaces tối ưu cho Kali NetHunter.
* **Đóng gói AnyKernel3:** Tự động xuất file flashable `.zip` có thể flash qua TWRP/OrangeFox hoặc nạp trực tiếp qua Magisk.

---

## 🚀 Hướng dẫn kích hoạt Build trên GitHub Actions
1. Vào tab **Actions** trên Repository GitHub này.
2. Chọn workflow tương ứng:
   * **Build NetHunter Kernel - LG V50 ThinQ**
   * **Build NetHunter Kernel - Asus Zenfone Max Pro M1**
3. Nhấn **Run workflow** -> Chọn branch `main` -> Nhấn **Run workflow**.
4. Sau khi quá trình build hoàn tất (khoảng 8 - 15 phút), cuộn xuống mục **Artifacts** để tải file `.zip` về điện thoại và flash!
