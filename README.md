# spresense_onewire

## overview

ソニー製マイコンSPRESENSEにてDS18B20などの1-Wireセンサを使用する場合に、OneWireライブラリにてデータが取得できない事象が確認されています。
https://forum.developer.sony.com/topic/678/compatibility-software-hardware-with-onewire-library

上記ページでもありますが、OneWireライブラリのソースを変更することで対応可能です。  

ここでは実際にライブラリをどのように書き換えたのかと、動作サンプル置き場となります。

## attention

- 動作サンプルでincludeしているライブラリは、書き換え後のライブラリです。
- ライブラリを上書きする形で変えているため、Arduino環境に戻った時にどのような影響が出るかは不明です。
- 動作確認のみを行うため、このサンプルではピン番号をOneWire.cppに直に記述しています。