# Arabdic — مشروع Flutter جاهز (Android & iOS)

## التشغيل محليًا
```
flutter pub get
flutter run
```

> إذا لم تكن مجلدات المنصات موجودة على جهازك:
```
flutter create .
```

## البناء عبر GitHub Actions (ملفات جاهزة للتثبيت)
### Android — APK
1) ارفع مجلد المشروع إلى مستودع GitHub جديد
2) افتح تبويب **Actions** وشغّل **Build Android APK**
3) حمّل Artifact: `arabdic-android-apk` (ملف `app-release.apk`)

### iOS — TestFlight (يلزم حساب Apple Developer)
- أضف Secrets إلى GitHub:
  - `APP_STORE_CONNECT_API_KEY_ID`
  - `APP_STORE_CONNECT_API_KEY_ISSUER_ID`
  - `APP_STORE_CONNECT_API_PRIVATE_KEY`
  - `APP_BUNDLE_ID` (مثل: com.yourname.arabdic)
- شغّل **iOS TestFlight Upload** وسيُرفع البناء إلى TestFlight.

