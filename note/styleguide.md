# Style Guide

shirokuma1101リポジトリ内でのStyle Guide

## スタイルについて

| name              | style                |
| ----------------- | -------------------- |
| CamelCase         | camelCase            |
| PascalCase        | PascalCase           |
| SnakeCase         | snake_case           |
| KebabCase         | kebab-case           |
| ConstantCase      | CONSTANT_CASE        |
| HungarianNotation | strName, intAge, ... |

### .editorconfig

``` .editorconfig
root = true

[*]
indent_style = space
indent_size = 2
end_of_line = lf
charset = utf-8
trim_trailing_whitespace = true
insert_final_newline = true

[*.{c,h,cc,hh,cpp,hpp}]
indent_size = 4
charset = utf-8-bom

[*.cs]
indent_size = 4

[*.go]
indent_style = tab

[*.{hlsl,hlsli}]
indent_size = 4

[*.py]
indent_size = 4

[*.rs]
indent_size = 4

```

## 総合的な命名規則

[初心者プログラマーのための変数/関数/メソッドの英語命名規則](https://qiita.com/YutaManaka/items/62dda256bb7ba6c08399)

## Git

### Git Repository

リポジトリ名はkebab-caseで記述する

### Git commit message

| normal word | light word | description                                 |
| ----------- | ---------- | ------------------------------------------- |
| add         | add        | Add new file                                |
| docs        | update     | Add or change docs (not including comments) |
| chore       | update     | Change build process, packaging, etc.       |
| feat        | update     | Add new features                            |
| fix         | fix        | Fix bugs                                    |
| refactor    | update     | Non-destructive code changes                |
| style       | update     | Change code style (including comments)      |
| test        | update     | Add or change test code                     |
| revert      | revert     | Undo a previous commit                      |
| remove      | remove     | delete file                                 |
| rename      | rename     | rename file                                 |

## C++

|                  |               |
| ---------------- | ------------- |
| Constant         | CONSTANT_CASE |
| Class            | PascalCase    |
| Structure        | PascalCase    |
| Enumerate        | PascalCase    |
| Enumerate member | CONSTANT_CASE |
| Variable         | camelCase     |
| Function         | PascalCase    |

### 優先順位

それぞれの優先順位の間には空行を入れる

1. pragma once
2. define (include guard)
3. include (standard library (using <>) e.g. `<memory>`)
4. include (system library (using <>) e.g. `<Windows.h>`), pragma comment (as needed)
5. include (internal library (using "")), pragma comment (as needed)
6. include (third party library (using "")), pragma comment (as needed)
7. pragma warning (as needed)
8. class, struct, namespace
9. public, protected, private
10. constructor, destructor
11. getter, setter
12. member variable

### 役割について

- namespace
  - inlineを必ず付ける
  - 定数にはconstexperを利用する
- class, struct
  - 一つでも関数を定義する場合はclass、変数のみの場合はstructを使用する

### 変数について

但し以下の場合は接頭辞を使用し、camelCase、PascalCaseを使用する

|                  |                |
| ---------------- | -------------- |
| Global Variable  | g_{camelCase}  |
| Private Variable | m_{camelCase}  |
| Pointer          | p{PascalCase}  |
| Shared Pointer   | sp{PascalCase} |
| Unique Pointer   | up{PascalCase} |
| Weak Pointer     | wp{PascalCase} |

## Python

PEP8に準拠
[PEP8](https://pep8-ja.readthedocs.io/ja/latest/)

|                   |               |
| ----------------- | ------------- |
| Constant          | CONSTANT_CASE |
| Class             | PascalCase    |
| Raise             | PascalCase    |
| Package           | lowercase     |
| Module            | snake_case    |
| Function, Method  | snake_case    |
| Variable          | snake_case    |
| Internal Function | _snake_case   |
| Internal Variable | _snake_case   |
