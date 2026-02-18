# vscode setting file

```json
{
  /* エディター */
  // フォントサイズ
  "editor.fontSize": 18,
  // インライン候補
  "editor.inlineSuggest.enabled": true,
  // 角括弧
  "editor.bracketPairColorization.enabled": true,
  // アクセシビリティ
  "editor.accessibilitySupport": "off",
  // フォントの種類
  "editor.fontFamily": "BIZ UDゴシック",
  // フォントの太さ
  "editor.fontWeight": "normal",

  // 起動時の画面
  "window.restoreWindows": "none",
  // ウェルカムページを表示
  "workbench.startupEditor": "welcomePage",
  // アイコン
  "workbench.iconTheme": "vscode-icons",
  // テーマ
  "workbench.colorTheme": "Default Dark+",

  /* ファイルツリー */
  // インデントガイド
  "workbench.tree.renderIndentGuides": "always",
  // インデントサイズ
  "workbench.tree.indent": 16,
  // フォルダ表示の圧縮
  "explorer.compactFolders": false,

  /* 拡張子毎の設定 */
  "files.associations": {
    "*.gs": "javascript"
  },

  /* 言語毎の設定 */
  "[html]": {
    "editor.defaultFormatter": "vscode.html-language-features"
  },
  "[markdown]": {
    "diffEditor.ignoreTrimWhitespace": true
  },
  "[yaml]": {
    "diffEditor.ignoreTrimWhitespace": true
  },

  /* 拡張機能 */

  // C#
  "dotnet.codeLens.enableReferencesCodeLens": false,

  // cmake
  "cmake.pinnedCommands": [
    "workbench.action.tasks.configureTaskRunner",
    "workbench.action.tasks.runTask"
  ],

  // drawio
  "hediet.vscode-drawio.resizeImages": null,

  // github copilot
  "github.copilot.enable": {
    "*": true,
    "plaintext": true,
    "markdown": true,
    "scminput": false,
    "yaml": true
  },

  // markdown
  "markdownlint.config": {
    "MD033": false
  },

  // powermode
  "powermode.enabled": true,
  "powermode.shake.intensity": 1
}
```
