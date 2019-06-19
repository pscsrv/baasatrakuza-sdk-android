![BaaS@rakuza](http://www.raku-za.jp/baas/images/baasatrakuza_logo.png)

# BaaS@rakuza SDK for Android

BaaS@rakuzaをAndroidより利用するためのSDKです。  
BaaS@rakuzaのご利用については [BaaS@rakuza製品サイト](http://www.raku-za.jp/baas/) をご確認ください。

## 対応バージョン

サポートされるBaaS@rakuzaのバージョンは以下の通りです。

BaaS@rakuza SDK バージョン|BaaS@rakuza バージョン|
|:-:|:-:|
|:new: 2.2.1|2.3.x, 2.4.x, 2.5.x|
|2.2.0|2.3.x, 2.4.x, 2.5.x|
|2.1.0|2.1.0, 2.2.0|
|2.0.1|2.0.0|
|2.0.0|2.0.0|


## インストール方法

* ZIPファイル形式にてダウンロード、もしくはリポジトリをcloneします。

```
git clone https://github.com/pscsrv/baasatrakuza-sdk-android
```

* ダウンロードしたプロジェクト内の*libs*ディレクトリ内のファイル一式を、利用したいプロジェクトの*libs*フォルダにコピーします。

**詳しい利用方法は、 [マニュアル](https://github.com/pscsrv/baasatrakuza-sdk-android/blob/master/manual/BaaSAtRakuzaSDK%E3%83%AA%E3%83%95%E3%82%A1%E3%83%AC%E3%83%B3%E3%82%B9%E3%83%9E%E3%83%8B%E3%83%A5%E3%82%A2%E3%83%AB_Android.pdf) を参照してください。**


## 利用準備

* RKZServiceを初期化します。*初期化する際に利用するライセンスキーは [BaaS@rakuza製品サイト](http://www.raku-za.jp/baas/) にてお申込みください。*

```
RKZClient.getInstance().initialize(getApplicationContext(), "{配布されたテナントキー}", new OnInitializeListener() {
    @Override
    public void onInitialize(boolean isSuccess, RKZResponseStatus status) {
        if (isSuccess) {
            // 成功!!!
        }
    }
});
```

**詳しい利用方法は、 [マニュアル](https://github.com/pscsrv/baasatrakuza-sdk-android/blob/master/manual/BaaSAtRakuzaSDK%E3%83%AA%E3%83%95%E3%82%A1%E3%83%AC%E3%83%B3%E3%82%B9%E3%83%9E%E3%83%8B%E3%83%A5%E3%82%A2%E3%83%AB_Android.pdf) を参照してください。**

## Copyright and License

Copyright (c) 2015-2017 People Software Corp. (http://www.pscsrv.co.jp)
