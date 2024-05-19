# Style Guide

Style Guide for shirokuma1101 repository

## About style

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

[*.{bat,cmd}]
end_of_line = crlf

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

## Comprehensive naming convention

[初心者プログラマーのための変数/関数/メソッドの英語命名規則](https://qiita.com/YutaManaka/items/62dda256bb7ba6c08399)

## Git

### Git Repository

リポジトリ名は`KebabCase`で記述する。

### Git commit message

| normal word | light word | description                                                                                |
| ----------- | ---------- | ------------------------------------------------------------------------------------------ |
| add         | add        | Add new file (except docs file and test file)                                              |
| chore       | update     | Change build process, packaging, etc.                                                      |
| docs        | update     | Add or change docs<br>(Use "style" when writing directly in the source file)               |
| feat        | update     | Add new features                                                                           |
| fix         | fix        | Fix bugs                                                                                   |
| refactor    | update     | Non-destructive code changes                                                               |
| style       | update     | Change code style<br>(Including when writing comments or docs directly in the source file) |
| test        | update     | Add or change test code                                                                    |
| remove      | remove     | Delete file                                                                                |
| rename      | rename     | Rename file                                                                                |
| revert      | revert     | Undo a previous commit                                                                     |

## C++

### Style Guide

|             |              |
| ----------- | ------------ |
| Constant    | ConstantCase |
| class       | PascalCase   |
| struct      | PascalCase   |
| enum        | PascalCase   |
| Enum member | ConstantCase |
| Variable    | CamelCase    |
| Function    | PascalCase   |

### Priority

それぞれの優先順位の間には空行を入れる。

1. File description (Doxygen style is preferred)
2. Include guard (pragma once)
3. include guard (ifndef, define e.g. `#ifndef HOGE_H_`)
4. include (standard library (using <>) e.g. `<memory>`)
5. include (system library (using <>) e.g. `<Windows.h>`), pragma comment (as needed)
6. include (internal library (using "")), pragma comment (as needed)
7. include (third party library (using "")), pragma comment (as needed)
8. pragma warning (as needed)
9. namespace, enum, struct, class
10. public, protected, private
11. constructor, destructor
12. getter, setter
13. member variable

### About roles

- namespace
  - `inline`を必ず付ける
  - 定数は`constexper`を利用する
- class, struct
  - 一つでも関数を定義する場合はclass、変数のみの場合はstructを使用する。

### About variable

但し以下の場合は接頭辞を使用し、`CamelCase`、`PascalCase`を併用する。

|                  |                |
| ---------------- | -------------- |
| Global Variable  | g_{CamelCase}  |
| Private Variable | m_{CamelCase}  |
| Pointer          | p{PascalCase}  |
| Shared Pointer   | sp{PascalCase} |
| Unique Pointer   | up{PascalCase} |
| Weak Pointer     | wp{PascalCase} |

### About definition

`ifdef`、`ifndef`を利用する場合は`endif`のコメントにdefine名を記述する。<br>
(e.g. `#endif //HOGE_H_`)

### About braces

トップレベルの関数のみ改行し、それ以外の場合は全て横に記述する

## C\#

### Style Guide

|             |              |
| ----------- | ------------ |
| Constant    | ConstantCase |
| class       | PascalCase   |
| struct      | PascalCase   |
| enum        | PascalCase   |
| Enum member | PascalCase   |
| Method      | PascalCase   |
| Property    | PascalCase   |
| field       | CamelCase    |

### Priority

1. using
2. namespace
3. enum
4. struct, class
5. constant
6. property
7. field
8. static method
9. method

## Python

PEP8に準拠
[PEP8](https://pep8-ja.readthedocs.io/ja/latest/)

|                   |                         |
| ----------------- | ----------------------- |
| Constant          | ConstantCase            |
| Class             | PascalCase              |
| Raise             | PascalCase              |
| Package           | lowercase               |
| Module            | SnakeCase               |
| Function, Method  | SnakeCase               |
| Variable          | SnakeCase               |
| Internal Function | SnakeCase with _ prefix |
| Internal Variable | SnakeCase with _ prefix |
