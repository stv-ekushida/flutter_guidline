# flutter_guidline

## 1. 初期設定

|No.|設定項目|必須|共通|iOS|Android|
|:----|:----|:----|:----|:----|:----|
|1|アプリアイコンの設定|○|○| | |
|2|アダプティブアイコンの設定|○| | |○|
|3|スプラッシュ画面の設定|○|○| | |
|4|サポート言語の設定| | | | |
|5|Flavorの設定|○|○| | |
|6|ステータスバーの透過|○| | |○|
|7|タイムゾーンの設定|○| | | |
|8|端末の文字サイズ無効化| | | | |
|9|署名(jks)の作成、設定|○| | |○|
|10|Provisining Profileの作成、設定|○| |○| |
|11|メトリックス計測|○|○| | |
|12|Viewportの設定|-| | | |
|13|Firebaseの設定|-|○| | |
|14|フォントの設定|-|○| | |
|15|端末縦固定|-|○| | |

## アプリアイコンの設定 / アダプティブアイコンの設定

[flutter_launcher_icons](https://pub.dev/packages/flutter_launcher_icons)


``` : pubspec.yaml
flutter_icons:
  android: "launcher_icon"
  ios: true
  image_path: "assets/images/icon.png"
  adaptive_icon_background: "assets/images/adaptive-icon-background.png"
  adaptive_icon_foreground: "assets/images/adaptive-icon-foreground.png"
```  

下記のコマンドを実行する
```
flutter pub run flutter_launcher_icons:main
```

## スプラッシュ画面の設定
[flutter_native_splash](https://pub.dev/packages/flutter_native_splash)


``` : puspec.yaml
flutter_native_splash:
  image: "assets/images/splash.png"
  color: "ffffff"
```

下記のコマンドを実行する
```
flutter pub run flutter_native_splash:create
```

## サポート言語の設定
https://docs.flutter.dev/development/accessibility-and-localization/internationalization


## Flavorの設定

## ステータスバーの透過

```
  SystemChrome.setSystemUIOverlayStyle(SystemUiOverlayStyle(
    statusBarColor: Colors.transparent,
  ));
```



