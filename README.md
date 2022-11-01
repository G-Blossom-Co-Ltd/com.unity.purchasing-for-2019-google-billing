# com.unity.purchasing-for-2019-google-billing

2022/11/1 Google Play へのアップデートは Google Play Billing Library v4 が必須になった。  
Unityの In App Purchaing パッケージは、2020以降でないと上記に対応したバージョンに出来ない。  
このリポジトリは、Unity2019で　Google Play Billing Library v4 に対応するためのリソース。  

# 手順

1. Packagesフォルダ内を自身のプロジェクトのPackagesフォルダに配置
2. 自身のプロジェクトのPackages/manifest.jsonを開き、以下２つを削除。
```
    "com.unity.analytics": "x.x.x",
    "com.unity.purchasing": "x.x.x",
```
3. IAP初期化処理にUnity Gaming Servicesを初期化
参考: https://docs.unity3d.com/Packages/com.unity.purchasing@4.5/manual/UnityIAPInitializeUnityGamingServices.html
4. （In App Purchaing の v2.x.x または v3.x.x だった場合） パッケージマネージャにて表示される手順で移行を完了させる
<img width="737" alt="image" src="https://user-images.githubusercontent.com/101873335/199259109-fae24897-e5cf-460f-9bd7-2a7224b3d0f8.png">

