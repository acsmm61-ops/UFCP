# Gerçek uygulama (APK / iOS) için — bilgisayar gerekir

Mac (iOS için) veya PC/Mac (Android için), Node.js 18+ kurulu olmalı.

    mkdir ufcp-app && cd ufcp-app
    npm init -y
    npm i @capacitor/core @capacitor/cli @capacitor/android @capacitor/ios
    npx cap init "KT-1T UFCP" com.ornek.ufcp --web-dir=www
    mkdir www && cp ../ufcp-pwa/* www/
    npx cap add android && npx cap add ios
    npx cap sync
    npx cap open android   # Android Studio -> Build > Build APK
    npx cap open ios       # Xcode -> cihaza çalıştır (Apple hesabı gerekir)

Kodu değiştirirsen www/ içini güncelle, sonra: npx cap sync
