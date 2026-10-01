# LORD MUSIC 🎵

موزیک پلیر با سه تم (آبی و مشکی، زرد و مشکی، خاکستری) و حالت دارک، لایت و سیستم.

## اجرا روی کامپیوتر
فایل `index.html` رو با Chrome یا Edge باز کن. همین.

## نصب روی گوشی (به شکل اپ)
1. کل پوشه رو روی یه هاست ساده آپلود کن (GitHub Pages، Netlify یا Vercel، رایگان).
2. لینک رو تو Chrome گوشی باز کن، منوی ⋮ و بعد **Add to Home screen / Install app**.
3. اپ با آیکون Lord Music نصب میشه و آفلاین هم کار می‌کنه.

## ساخت فایل APK اندروید
- ساده‌ترین راه: لینک سایت رو بده به **pwabuilder.com** و APK بگیر.
- یا با Capacitor:
  ```
  npm i @capacitor/core @capacitor/cli @capacitor/android
  npx cap init "Lord Music" com.lord.music --web-dir .
  npx cap add android
  npx cap open android
  ```
  بعد تو Android Studio گزینه‌ی Build APK.

## امکانات
- ۸ آهنگ دمو که زنده با Web Audio ساخته میشن (بدون نیاز به فایل)
- وارد کردن آهنگ‌های خودت (MP3، M4A، FLAC، WAV، OGG) با خوندن اسم، خواننده و کاور از تگ ID3، که روی خود دستگاه ذخیره میشن
- اکولایزر واقعی ۱۰ باندی + ۷ پریست + بیس بوست + Virtualizer
- متن آهنگ همزمان، تایمر خواب، صف پخش، شافل، تکرار (همه / یکی)
- علاقه‌مندی‌ها، جستجو، دسته‌بندی آلبوم و خواننده
- کنترل از صفحه‌ی قفل و هدفون (Media Session)
- میانبرهای کیبورد: Space پخش/توقف، ← → جلو و عقب ۱۰ ثانیه

## فایل‌ها
- `index.html` صفحه‌ی اصلی
- `styles.css` تم‌ها و ظاهر
- `app.js` منطق اپ
- `synth.js` موتور صدا و اکولایزر
- `data.js` آهنگ‌های دمو و پریست‌ها
- `manifest.webmanifest`, `sw.js`, `icon.*` برای نصب به‌عنوان اپ
