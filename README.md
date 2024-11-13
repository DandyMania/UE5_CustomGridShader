# UE5_CustomGridShader
UE5向けグリッドシェーダー 

対応バージョン UE5.4

# 概要
パラメータによる多彩な設定が可能なグリッドシェーダー  
３種類のグリッドラインの線の色・太さ・間隔、背景カラーが設定可能  

# 使い方

* プロジェクト一式Cloneした後、CustomGridフォルダを同じ階層のまま自分のプロジェクトにコピーするか、
[UE4] 他プロジェクトからアセットを移動させる方法  
https://historia.co.jp/archives/275/  
の方法を参考にCustomGridフォルダ以下をお好きなプロジェクトに移動させてください

* デフォルトのグリッドからカスタムしたい場合は、CustomGrid/Materials/MT_CustomGrid からマテリアルインスタンスを作成しパラメータを変更してください
<img width="741" alt="materialinstance" src="https://user-images.githubusercontent.com/2414102/77820265-5f4f1100-7124-11ea-8c5c-0ff1008f88d9.png">

* あとはお好きなモデルにマテリアルを割り当てるとグリッドが表示されます

# シェーダーの各種パラメータ説明

| パラメータ | 説明 |
| ------------- | ------------- |
| Blink  | 0以外を入れると点滅するようになります。Emissiveの値を0以上にする必要があります。 |
| Emissive    | Wide/Midele のグリッドのエミッシブカラーの調整用 |
| Metallic  | 1.0に近づくほど金属っぽい表現になります |
| Roughness  | 1.0に近づくほどざらざらになります |
| **GridColor** |  |
| BackgroundColor  | 背景色  |
| GridColorMidele  | 中くらいの細かさのグリッドの色設定 |
| GridColorNarrow  | 一番細かいグリッドの色設定。一番下に描かれる |
| GridColorWide    | 基準となるグリッドの色設定。一番上に描かれる |
| **Grid Properties** |  |
| LineIntervalMiddle  | グリッドの間隔(中)。※単位はメートルです。 |
| LineIntervalNarrow  | グリッドの間隔(細) ※単位はメートルです。|
| LineIntervalWide  | グリッドの間隔(広) ※単位はメートルです。|
| LineSizeMiddle  | グリッド太さ(中) |
| LineSizeNarrow  | グリッド太さ(細) |
| LineSizeWide  | グリッド太さ(広) |
| **Text** |  |
| TextVisible  | テキスト表示切り替え |
| CrossVisible  | 十字テクスチャー表示切り替え |

# ライセンス

MIT
