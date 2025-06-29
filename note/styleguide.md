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

# using directive preferences
dotnet_diagnostic.IDE0005.severity = warning
csharp_using_directive_placement = outside_namespace:warning

# Code-block preferences
csharp_prefer_braces = true:warning
csharp_prefer_simple_using_statement = true:warning
csharp_style_namespace_declarations = block_scoped:warning
csharp_style_prefer_method_group_conversion = true:warning
csharp_style_prefer_top_level_statements = true:warning
csharp_style_prefer_top_level_statements = true:warning
csharp_style_prefer_primary_constructors = true:warning

# Expression-bodied members
csharp_style_expression_bodied_constructors = true:warning
csharp_style_expression_bodied_methods = true:warning
csharp_style_expression_bodied_operators = true:warning
csharp_style_expression_bodied_properties = true:warning
csharp_style_expression_bodied_indexers = true:warning
csharp_style_expression_bodied_accessors = true:warning
csharp_style_expression_bodied_lambdas = true:warning
csharp_style_expression_bodied_local_functions = true:warning

# Expression-level preferences
dotnet_diagnostic.IDE0001.severity = warning
dotnet_diagnostic.IDE0002.severity = warning
dotnet_diagnostic.IDE0004.severity = warning
dotnet_diagnostic.IDE0010.severity = warning
dotnet_style_object_initializer = true:warning
dotnet_style_collection_initializer = true:warning
dotnet_style_prefer_collection_expression = true:warning
dotnet_style_coalesce_expression = true:warning
dotnet_style_null_propagation = true:warning
dotnet_style_prefer_auto_properties = true:warning
dotnet_style_explicit_tuple_names = true:warning
dotnet_diagnostic.IDE0035.severity = warning
dotnet_style_prefer_inferred_tuple_names = true:warning
dotnet_style_prefer_inferred_anonymous_type_member_names = true:warning
dotnet_style_prefer_is_null_check_over_reference_equality_method = true:warning
dotnet_style_prefer_conditional_expression_over_assignment = true:warning
dotnet_style_prefer_conditional_expression_over_return = true:warning
dotnet_diagnostic.IDE0050.severity = warning
dotnet_diagnostic.IDE0051.severity = warning
dotnet_diagnostic.IDE0052.severity = warning
dotnet_style_prefer_compound_assignment = true:warning
csharp_style_unused_value_expression_statement_preference = discard_variable:warning
csharp_style_unused_value_assignment_preference = discard_variable:warning
dotnet_diagnostic.IDE0070.severity = warning
dotnet_style_prefer_simplified_interpolation = true:warning
dotnet_style_prefer_simplified_boolean_expressions = true:warning
dotnet_diagnostic.IDE0082.severity = warning
dotnet_diagnostic.IDE0100.severity = warning
dotnet_diagnostic.IDE0120.severity = warning
dotnet_style_namespace_match_folder = true:warning

csharp_style_throw_expression = true:warning
csharp_style_inlined_variable_declaration = true:warning
csharp_prefer_simple_default_expression = true:warning
csharp_style_prefer_local_over_anonymous_function = true:warning
csharp_style_deconstructed_variable_declaration = true:warning
csharp_style_prefer_index_operator = true:warning
csharp_style_prefer_range_operator = true:warning
dotnet_diagnostic.IDE0072.severity = warning
dotnet_diagnostic.IDE0080.severity = warning
csharp_style_implicit_object_creation_when_type_is_apparent = true:warning
dotnet_diagnostic.IDE0110.severity = warning
csharp_style_prefer_null_check_over_type_check = true:warning
csharp_style_prefer_tuple_swap = true:warning
dotnet_style_prefer_foreach_explicit_cast_in_source = when_strongly_typed:warning ;when_strongly_typed
csharp_style_prefer_utf8_string_literals = true:warning
dotnet_diagnostic.IDE0240.severity = warning
dotnet_diagnostic.IDE0241.severity = warning
dotnet_style_prefer_collection_expression = true:warning

# Field preferences
dotnet_style_readonly_field = true:warning

# Language keyword vs. framework types preferences
dotnet_style_predefined_type_for_locals_parameters_members = true:none ;none
dotnet_style_predefined_type_for_member_access = true:none ;none

# Modifier preferences
csharp_preferred_modifier_order = public,protected,internal,private,file,static,extern,new,virtual,abstract,sealed,override,readonly,unsafe,required,volatile,async
dotnet_style_require_accessibility_modifiers = always

csharp_prefer_static_local_function = true:suggestion ;suggestion
dotnet_diagnostic.IDE0064.severity = warning
csharp_style_prefer_readonly_struct = true:warning
csharp_style_prefer_readonly_struct_member = true:warning

# Null-checking preferences
csharp_style_conditional_delegate_call = true:warning

# Parameter preferences
dotnet_code_quality_unused_parameters = true:warning

# Pattern-matching preferences
csharp_style_pattern_matching_over_as_with_null_check = true:warning
csharp_style_pattern_matching_over_is_with_cast_check = true:warning
csharp_style_prefer_switch_expression = true:warning
csharp_style_prefer_pattern_matching = true:warning
csharp_style_pattern_matching_over_as_with_null_check = true:warning
csharp_style_prefer_not_pattern = true:warning
csharp_style_prefer_extended_property_pattern = true:warning

# Suppression preferences
dotnet_remove_unnecessary_suppression_exclusions = true:warning

# This. and me. preferences
dotnet_style_qualification_for_field = false:warning ;false
dotnet_style_qualification_for_property = false:warning ;false
dotnet_style_qualification_for_method = false:warning ;false
dotnet_style_qualification_for_event = false:warning ;false

# var preferences
csharp_style_var_for_built_in_types = true:warning
csharp_style_var_when_type_is_apparent = true:warning
csharp_style_var_elsewhere = true:warning

# Correctness
dotnet_diagnostic.UNT0004.severity = warning
dotnet_diagnostic.UNT0005.severity = warning
dotnet_diagnostic.UNT0007.severity = warning
dotnet_diagnostic.UNT0008.severity = warning
dotnet_diagnostic.UNT0009.severity = warning
dotnet_diagnostic.UNT0012.severity = warning
dotnet_diagnostic.UNT0013.severity = warning
dotnet_diagnostic.UNT0020.severity = warning
dotnet_diagnostic.UNT0021.severity = warning
dotnet_diagnostic.UNT0023.severity = warning
dotnet_diagnostic.UNT0025.severity = warning
dotnet_diagnostic.UNT0027.severity = warning
dotnet_diagnostic.UNT0029.severity = warning
dotnet_diagnostic.UNT0030.severity = warning
dotnet_diagnostic.UNT0031.severity = warning
dotnet_diagnostic.UNT0033.severity = error
# Performance
dotnet_diagnostic.UNT0001.severity = warning
dotnet_diagnostic.UNT0002.severity = warning
dotnet_diagnostic.UNT0017.severity = warning
dotnet_diagnostic.UNT0018.severity = warning
dotnet_diagnostic.UNT0019.severity = warning
dotnet_diagnostic.UNT0022.severity = warning
dotnet_diagnostic.UNT0024.severity = warning
dotnet_diagnostic.UNT0026.severity = warning
dotnet_diagnostic.UNT0028.severity = warning
dotnet_diagnostic.UNT0032.severity = warning
dotnet_diagnostic.UNT0034.severity = warning
dotnet_diagnostic.UNT0035.severity = warning
dotnet_diagnostic.UNT0036.severity = warning
dotnet_diagnostic.UNT0037.severity = warning
# TypeSafety
dotnet_diagnostic.UNT0003.severity = warning
dotnet_diagnostic.UNT0006.severity = error
dotnet_diagnostic.UNT0010.severity = warning
dotnet_diagnostic.UNT0011.severity = warning
dotnet_diagnostic.UNT0014.severity = warning
dotnet_diagnostic.UNT0015.severity = error
dotnet_diagnostic.UNT0016.severity = warning

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
| Class       | PascalCase   |
| Struct      | PascalCase   |
| Enum        | PascalCase   |
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
e.g. `#endif //HOGE_H_`

### About braces

トップレベルの関数のみ改行し、それ以外の場合は全て横に記述する

## C\#

### Style Guide

|             |              |
| ----------- | ------------ |
| Constant    | ConstantCase |
| class       | PascalCase   |
| struct      | PascalCase   |
| Enum        | PascalCase   |
| Enum member | PascalCase   |
| Method      | PascalCase   |
| Property    | PascalCase   |
| Field       | CamelCase    |

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
