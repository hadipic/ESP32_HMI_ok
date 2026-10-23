# ESP32 HMI (Touch LCD SPI)

**طراحی سخت‌افزاری کامل بورد HMI مبتنی بر ESP32 با نمایشگر لمسی LCD از طریق رابط SPI**

این مخزن شامل فایل‌های طراحی PCB و شماتیک پروژه **ESP32 HMI** است که با نرم‌افزار **Altium Designer** ساخته شده است.

---

## درباره پروژه

این بورد یک رابط انسان-ماشین (HMI) کم‌حجم و کاربردی بر پایه ماژول **ESP32** است که برای اتصال مستقیم به نمایشگرهای TFT لمسی از طریق رابط **SPI** طراحی شده است.

### ویژگی‌های اصلی
- پشتیبانی از ESP32 (ماژول‌های رایج مانند ESP32-WROOM / ESP32-WROVER)
- اتصال نمایشگر TFT LCD با رابط SPI
- پشتیبانی از تاچ (Touch Controller)
- طراحی مناسب برای کاربردهای صنعتی، خانگی و پروژه‌های IoT
- فایل‌های کامل شماتیک و PCB آماده تولید

---

## محتویات مخزن

| فایل | توضیح |
|------|------|
| `ESP32_HMI.PrjPcb` | فایل پروژه اصلی Altium Designer |
| `ESP32_HMI.schdoc` | شماتیک مدار |
| `ESP32_HMI.PcbDoc` | طراحی PCB |
| `ESP32_HMI1.PcbLib` | کتابخانه قطعات PCB |
| `ESP32_HMI.PcbDoc.htm` | گزارش خروجی PCB |

> **نکته:** فایل‌های شماتیک و PCB به صورت باینری هستند و برای باز کردن آن‌ها به نرم‌افزار **Altium Designer** نیاز دارید.

---

## پیش‌نیازها

### نرم‌افزاری
- [Altium Designer](https://www.altium.com/) (نسخه ۲۰ یا بالاتر توصیه می‌شود)

### سخت‌افزاری پیشنهادی
- ماژول ESP32 (ترجیحاً با آنتن خارجی یا WROVER برای حافظه بیشتر)
- نمایشگر TFT LCD با رابط SPI (مثل ILI9341، ST7789، ILI9488 و ...)
- کنترلر تاچ مقاومتی یا خازنی سازگار با SPI/I2C
- قطعات پاور (رگولاتور ۳.۳ ولت، خازن‌ها، کانکتور USB و ...)

---

## نحوه استفاده

1. مخزن را کلون کنید یا به صورت ZIP دانلود کنید:
```bash
git clone https://github.com/hadipic/ESP32_HMI_ok.git
```

2. فایل `ESP32_HMI.PrjPcb` را با **Altium Designer** باز کنید.

3. شماتیک و PCB را بررسی و در صورت نیاز ویرایش کنید.

4. خروجی‌های تولید (Gerber، BOM، Pick & Place و ...) را از منوی **Fabrication Outputs** و **Assembly Outputs** استخراج کنید.

5. فایل‌های Gerber را برای ساخت PCB به کارخانه ارسال کنید.

---

## ساختار پیشنهادی پروژه (بعد از توسعه)

```
ESP32_HMI_ok/
├── Hardware/                 # فایل‌های طراحی سخت‌افزار
│   ├── ESP32_HMI.PrjPcb
│   ├── ESP32_HMI.schdoc
│   ├── ESP32_HMI.PcbDoc
│   └── Libraries/
├── Firmware/                 # (در صورت اضافه شدن) کدهای ESP-IDF یا Arduino
├── Docs/                     # مستندات و تصاویر
└── README.md
```

---

## کاربردهای پیشنهادی

- پنل کنترل هوشمند خانگی
- مانیتورینگ سنسورها و تجهیزات صنعتی
- داشبورد IoT
- کنترلر لمسی دستگاه‌های اندازه‌گیری
- پروژه‌های آموزشی و نمونه‌سازی سریع

---

## وضعیت پروژه

- طراحی سخت‌افزاری: **آماده**
- نرم‌افزار (Firmware): هنوز اضافه نشده
- مستندات کامل: در حال تکمیل

---

## مشارکت

اگر می‌خواهید در توسعه این پروژه مشارکت کنید:

1. پروژه را Fork کنید
2. یک Branch جدید بسازید
3. تغییرات خود را Commit کنید
4. Pull Request ارسال کنید

ایده‌ها و پیشنهادات شما از طریق Issues بسیار ارزشمند است.

---

## لایسنس

این پروژه در حال حاضر لایسنس مشخصی ندارد.  
در صورت استفاده تجاری یا انتشار مجدد، لطفاً با من  هماهنگ کنید.

---

## تماس و پشتیبانی

- مخزن گیت‌هاب: [https://github.com/hadipic/ESP32_HMI_ok](https://github.com/hadipic/ESP32_HMI_ok)
- در صورت نیاز به اصلاحات یا افزودن فایل‌های Gerber، BOM یا فریمور، از بخش Issues استفاده کنید.

---

**ساخته شده با** توسط [hadipic](https://github.com/hadipic)

 📚 منابع و مستندات

### 🔗 مخازن GitHub مرتبط

| پروژه | توضیحات | لینک GitHub |
|-------|---------|-------------|
| **EVM Linux** | ماشین مجازی برای لینوکس | [github.com/hadipic/evm-linux](https://github.com/hadipic/evm-linux) |
| **ESP32 EVM Bin** | فایل‌های باینری ESP32 | [github.com/hadipic/esp32-evm-bin](https://github.com/hadipic/esp32-evm-bin) |
| **EVM Java** | پیاده‌سازی جاوا | [github.com/hadipic/evm_java](https://github.com/hadipic/evm_java) |
| **LVGL GUI Builder** | همین پروژه | [github.com/hadipic/-home-shop-electronic-project-esp32-evm-esp32-gui-builder](https://github.com/hadipic/-home-shop-electronic-project-esp32-evm-esp32-gui-builder) |

### 📖 مقالات و آموزش‌ها
- **معرفی کامل EVM**: [shop-electronic.ir/ماشین-مجازی-جاوا-برای-امبد-بردها-evm-embedded-virtual-machi/](https://shop-electronic.ir/ماشین-مجازی-جاوا-برای-امبد-بردها-evm-embedded-virtual-machi/)
- **مستندات EVM**: [github.com/hadipic/evm-linux/wiki](https://github.com/hadipic/evm-linux/wiki)

---

## 👥 شبکه‌های اجتماعی و ارتباطی

### 💬 تلگرام
| نوع | نام | لینک |
|-----|-----|------|
| **گروه** | ESP32 Community | [t.me/+oi9QrKR1qdozZTc0](https://t.me/+oi9QrKR1qdozZTc0) |
| **گروه** | Embedded & Qt | [t.me/Embedded_Qt](https://t.me/Embedded_Qt) |
| **کانال** | ESP32 EVM | [t.me/esp32_evm](https://t.me/esp32_evm) |
| **ربات** | Shop Electronic | [@shop_electronic_bot](https://t.me/shop_electronic_bot) |

### 🌐 وبسایت‌ها
- **فروشگاه الکترونیک**: [shop-electronic.ir](https://shop-electronic.ir)
- **گیت‌هاب**: [github.com/hadipic](https://github.com/hadipic)

### 📧 مخازن کد
```text
EVM Linux:       github.com/hadipic/evm-linux
ESP32 EVM Bin:   github.com/hadipic/esp32-evm-bin  
EVM Java:        github.com/hadipic/evm_java
GUI Builder:     github.com/hadipic/-home-shop-electronic-project-esp32-evm-esp32-gui-builder

---
 
