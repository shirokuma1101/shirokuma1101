# 命名規則

shirokuma1101リポジトリ内での命名規則

## 総合的な命名規則

[初心者プログラマーのための変数/関数/メソッドの英語命名規則](https://qiita.com/YutaManaka/items/62dda256bb7ba6c08399)

## git commit message

| normalword | lightword | description |
| - | - | - |
| add | add | 新規ファイルの追加 |
| docs | update | ドキュメントの追加・変更 |
| chore | update | ビルド・パッケージングなどの変更 |
| feat | update | 新規機能の追加 |
| fix | fix | バグの修正 |
| refactor | update | リファクタリング |
| style | update | コードスタイルの変更 |
| test | update | テストコードの追加・変更 |
| revert | revert | 一つ前のコミットを取り消す |
| remove | remove | ファイルの削除 |
| rename | rename | ファイル名の変更 |

## C++

| | |
| - | - |
| 定数 | ALL_CAPS |
| クラス | PascalCase |
| 構造体 | PascalCase |
| 列挙体 | PascalCase |
| 列挙体のメンバ | ALL_CAPS |
| 変数 | camelCase |

### 変数について

但し以下の場合は接頭辞を使用し、camelCase、PascalCaseを使用する

| camelCase | |
| - | - |
| グローバル変数 | g_ |
| プライベートのメンバ変数 | m_ |

| PascalCase | |
| - | - |
| ポインタ型 | p |
| shared_ptr型 | sp |
| unique_ptr型 | up |
| weak_ptr型 | wp |

## Python

PEP8に準拠
[PEP8](https://pep8-ja.readthedocs.io/ja/latest/)

| | |
| - | - |
| 定数 | ALL_CAPS |
| クラス | PascalCase |
| 例外 | PascalCase |
| パッケージ | lowercase |
| モジュール | snake_case |
| 関数 | snake_case |
| 変数 | snake_case |
| 内部関数 | _snake_case |
| 内部変数 | _snake_case |
