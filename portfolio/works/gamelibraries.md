# game-libraries

ゲーム開発に利用できるライブラリ

[game-libraries](https://github.com/shirokuma1101/game-libraries)

|          |                          |
| -------- | ------------------------ |
| 開発環境     | C++17,Visual Studio 2022 |
| 開発人数     | 1人                       |
| 開発期間     | 6ヶ月~                     |
| プラットフォーム | Windows                  |
| 担当箇所     | 全て                       |

## C++17 Header-Only libraries

C++17/DirectX11でのゲーム開発において、Unityのような算術やAsset操作ライブラリを自前で実装する必要がありました。今まではそれぞれのプロジェクトで個別にUtilityクラスを作成して実装していましたが、汎用的に利用できるものは別プロジェクトでまとめられた方が実装する都度実装する必要がなくなると考え、game-librariesとしてライブラリを制作しました。

現在はC++17をベースとしたメモリ関連のクラスや、`PhysX`,`DirectXTK`,`Effekseer`等の外部ライブラリを利用したWrapperを実装しています。

### 利用しやすくする工夫

コードは他の人と簡単に共有できるようにGitHub上で公開しています。また、ライブラリの種類として`Header Only`ライブラリとしました。

この理由として、

- 基本的にUtilityに分類されるような機能、もしくはWrapperなのでビルド時間に影響しにくい
- 環境に合わせたLibをBuildする必要がなく、Linkする等の手間が不要

という理由から、`Header OnlY`ライブラリとして作成しました。

また、作成する際の注意点など詳細はZennの記事で紹介しています。

[C++ライブラリ化のすゝめ](https://zenn.dev/kd_gamegikenblg/articles/d8bcb50348415e)

## Tools

使用するライブラリによって、Assetの種類が限定される場合がありました。そこで、複数の種類から利用できる種類に変換できるScriptをToolとして作成しました。基本的にオプションは引数として設定し、D&Dで簡単に変換できるようになっています。

- ConvertToWave<br>
  ファイルをWaveに変換
- EasyImageResizer<br>
  画像をリサイズ
- ImageRgbaExtractor<br>
  画像からのRGBA値を抽出
- VideoToSequentialImage<br>
  ビデオを連番画像に変換
