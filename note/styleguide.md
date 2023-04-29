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

| normal word | light word | description                           |
| ----------- | ---------- | ------------------------------------- |
| add         | add        | Add new file                          |
| docs        | update     | Add or change docs                    |
| chore       | update     | Change build process, packaging, etc. |
| feat        | update     | Add new features                      |
| fix         | fix        | Fix bugs                              |
| refactor    | update     | Refactor code                         |
| style       | update     | Change code style                     |
| test        | update     | Add or change test code               |
| revert      | revert     | Undo a previous commit                |
| remove      | remove     | delete file                           |
| rename      | rename     | rename file                           |

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
