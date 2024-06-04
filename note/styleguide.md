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

<details><summary>Click to show</summary>

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

;https://learn.microsoft.com/ja-jp/dotnet/fundamentals/code-analysis/style-rules/

dotnet_diagnostic.IDE0005.severity = error
csharp_using_directive_placement = outside_namespace:error

csharp_prefer_braces = true:error
csharp_prefer_simple_using_statement = true:error
csharp_style_namespace_declarations = block_scoped:error
csharp_style_prefer_method_group_conversion = true:error
csharp_style_prefer_top_level_statements = true:error
csharp_style_prefer_top_level_statements = true:error
csharp_style_prefer_primary_constructors = true:error

csharp_style_expression_bodied_constructors = true:error
csharp_style_expression_bodied_methods = true:error
csharp_style_expression_bodied_operators = true:error
csharp_style_expression_bodied_properties = true:error
csharp_style_expression_bodied_indexers = true:error
csharp_style_expression_bodied_accessors = true:error
csharp_style_expression_bodied_lambdas = true:error
csharp_style_expression_bodied_local_functions = true:error

dotnet_diagnostic.IDE0001.severity = error
dotnet_diagnostic.IDE0002.severity = error
dotnet_diagnostic.IDE0004.severity = error
dotnet_diagnostic.IDE0010.severity = error
dotnet_style_object_initializer = true:error
dotnet_style_collection_initializer = true:error
dotnet_style_prefer_collection_expression = true:error
dotnet_style_coalesce_expression = true:error
dotnet_style_null_propagation = true:error
dotnet_style_prefer_auto_properties = true:error
dotnet_style_explicit_tuple_names = true:error
dotnet_diagnostic.IDE0035.severity = error
dotnet_style_prefer_inferred_tuple_names = true:error
dotnet_style_prefer_inferred_anonymous_type_member_names = true:error
dotnet_style_prefer_is_null_check_over_reference_equality_method = true:error
dotnet_style_prefer_conditional_expression_over_assignment = true:error
dotnet_style_prefer_conditional_expression_over_return = true:error
dotnet_diagnostic.IDE0050.severity = error
dotnet_diagnostic.IDE0051.severity = error
dotnet_diagnostic.IDE0052.severity = error
dotnet_style_prefer_compound_assignment = true:error
csharp_style_unused_value_expression_statement_preference = discard_variable:error
csharp_style_unused_value_assignment_preference = discard_variable:error
dotnet_diagnostic.IDE0070.severity = error
dotnet_style_prefer_simplified_interpolation = true:error
dotnet_style_prefer_simplified_boolean_expressions = true:error
dotnet_diagnostic.IDE0082.severity = none ;none
dotnet_diagnostic.IDE0100.severity = error
dotnet_diagnostic.IDE0120.severity = error
dotnet_style_namespace_match_folder = true:error

csharp_style_throw_expression = true:error
csharp_style_inlined_variable_declaration = true:error
csharp_prefer_simple_default_expression = true:error
csharp_style_prefer_local_over_anonymous_function = true:error
csharp_style_deconstructed_variable_declaration = true:error
csharp_style_prefer_index_operator = true:error
csharp_style_prefer_range_operator = true:error
dotnet_diagnostic.IDE0072.severity = error
dotnet_diagnostic.IDE0080.severity = error
csharp_style_implicit_object_creation_when_type_is_apparent = true:error
dotnet_diagnostic.IDE0110.severity = error
csharp_style_prefer_null_check_over_type_check = true:error
csharp_style_prefer_tuple_swap = true:error
dotnet_style_prefer_foreach_explicit_cast_in_source = when_strongly_typed:error ;when_strongly_typed
csharp_style_prefer_utf8_string_literals = true:error
dotnet_diagnostic.IDE0240.severity = error
dotnet_diagnostic.IDE0241.severity = error
dotnet_style_prefer_collection_expression = true:error

dotnet_style_readonly_field = false:none ;false

dotnet_style_predefined_type_for_locals_parameters_members = true:none ;none
dotnet_style_predefined_type_for_member_access = true:none ;none

csharp_preferred_modifier_order = public, private, protected, internal, file, static, extern, new, virtual, abstract, sealed, override, readonly, unsafe, required, volatile, async
dotnet_style_require_accessibility_modifiers = always

csharp_prefer_static_local_function = true:suggestion ;suggestion
dotnet_diagnostic.IDE0064.severity = error
csharp_style_prefer_readonly_struct = true:error
csharp_style_prefer_readonly_struct_member = true:error

csharp_style_conditional_delegate_call = true:error
dotnet_code_quality_unused_parameters = true:error

csharp_style_pattern_matching_over_as_with_null_check = true:error
csharp_style_pattern_matching_over_is_with_cast_check = true:error
csharp_style_prefer_switch_expression = true:error
csharp_style_prefer_pattern_matching = true:error
csharp_style_pattern_matching_over_as_with_null_check = true:error
csharp_style_prefer_not_pattern = true:error
csharp_style_prefer_extended_property_pattern = true:error

dotnet_remove_unnecessary_suppression_exclusions = true:error

dotnet_style_qualification_for_field = false:error ;false
dotnet_style_qualification_for_property = false:error ;false
dotnet_style_qualification_for_method = false:error ;false
dotnet_style_qualification_for_event = false:error ;false

csharp_style_var_for_built_in_types = true:error
csharp_style_var_when_type_is_apparent = true:error
csharp_style_var_elsewhere = true:error

[*.go]
indent_style = tab

[*.{hlsl,hlsli}]
indent_size = 4

[*.py]
indent_size = 4

[*.rs]
indent_size = 4

```

</details>

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

### About specifier

1. public/private/protected/internal
2. static
3. virtual, abstract, partial, override
4. async
5. void

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
