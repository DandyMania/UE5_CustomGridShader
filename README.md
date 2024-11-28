# UE5_CustomGridShader
UE5向けグリッドシェーダー 

対応バージョン UE5.4

# 概要
パラメータによる多彩な設定が可能なグリッドシェーダー  
３種類のグリッドラインの線の色・太さ・間隔、テクスチャの設定が可能です  
![image](https://github.com/user-attachments/assets/e627a7d8-8c18-413a-8a9e-7c57a9bc2f11)

# 使い方

* プロジェクト一式Cloneした後、CustomGridフォルダを同じ階層のまま自分のプロジェクトにコピーするか、
[UE4] 他プロジェクトからアセットを移動させる方法  
https://historia.co.jp/archives/275/  
の方法を参考にCustomGridフォルダ以下をお好きなプロジェクトに移動させてください

* デフォルトのグリッドからカスタムしたい場合は、CustomGrid/Materials/MT_CustomGrid からマテリアルインスタンスを作成しパラメータを変更してください
![image](https://github.com/user-attachments/assets/e8d1f8cf-639f-46ca-8568-3d4e6a21994e)

* あとはお好きなモデルにマテリアルを割り当てるとグリッドが表示されます

# シェーダーの各種パラメータ説明

| パラメータ | 説明 |
| ------------- | ------------- |
| **GridColor** |  |
| BackgroundColor  | 床のカラー  |
| BackgroundWall  | 壁のカラー  |
| GridColorMidele  | 中くらいの細かさのグリッドの色設定 |
| GridColorNarrow  | 一番細かいグリッドの色設定。一番下に描かれる |
| GridColorWide    | 基準となるグリッドの色設定。一番上に描かれる |
| **Grid Properties** |  |
| GridLocal | アクターローカルなグリッドを表示 |
| LineIntervalMiddle  | グリッドの間隔(中)|
| LineIntervalNarrow  | グリッドの間隔(細)|
| LineIntervalWide  | グリッドの間隔(広)|
| LineSizeMiddle  | グリッド太さ(中) |
| LineSizeNarrow  | グリッド太さ(細) |
| LineSizeWide  | グリッド太さ(広) |
| **Misc** |  |
| Blink  | 0以外を入れると点滅するようになります。Emissiveの値を0以上にする必要があります。 |
| Emissive    | Wide/Midele のグリッドのエミッシブカラーの調整用 |
| Metallic  | 1.0に近づくほど金属っぽい表現になります |
| Roughness  | 1.0に近づくほどざらざらになります |
| **Texture** |  |
| Checker  | チェッカー表示用テクスチャ |
| Checker  | チェッカーのカラー |
| Checker Tiling  | チェッカータイリング間隔 |
| Cross  | クロステクスチャー |
| Cross Color  | クロステクスチャーの色 |
| Cross Tiling  | クロステクスチャーのタイリング間隔 |
| Cross Visible  | クロステクスチャー表示設定 |
| Text  | テキスト表示設定 |
| Text Color  | テキストの色 |
| Text Tiling  | テキストのタイリング間隔 |
| Text Visible  | テキストの表示設定 |

# ライセンス

MIT
