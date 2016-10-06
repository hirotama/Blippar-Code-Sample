# Blippar-Code-Sample
Learning about Blippar, it's a first demo from the official tutorial

The official site:(may need login)
https://developer.blippar.com/portal/documentation/

Node.js part we are needed:
===
javascript/
    package.json
      {
        "version": "1.0.0",
        "description": "Developers Portal Demo",
        "main": "main.js",
        "blipp" : {
          "title": "Earth and Geolocation",
          "shortTitle": "Globe"
        },
        "dependencies": {
          "blippar": "1.2.68"
        }
    }

    main.js

assets/
    file1.png
    file2.png
    ...

markers/
    marker1.jpg
    marker2.jpg
    ...
===
上記のように、package.json　の3行目に　mainとしてmain.jsを使うという宣言をしているので、main.jsを用意するのだが、もちろん、この名前を変えて、別名のjavascriptファイルから開始してもかまわない。

main.jsの中身をみていく。
最初の行は必ず、次のように書いて始まる。
var blipp = require('blippar').blipp;
これにより、blipparクラスがすべて呼ばれ、グローバルオブジェクトのblippに格納される。

blippは最低ひとつのシーンが必要になる。sceneというオブジェクトを使って、シーンを構築する。
var scene = blipp.addScene();





