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

  /* 拡張子毎の設定 */
  "files.associations": {
    "*.gs": "javascript"
  },

  /* 拡張機能 */

  // C#
  "dotnet.codeLens.enableReferencesCodeLens": false,

  // Markdown
  "markdownlint.config": {
    "MD033": false
  },

  // drawio
  "hediet.vscode-drawio.resizeImages": null,

  // powermode
  "powermode.enabled": true,
  "powermode.shake.intensity": 1,

  // diff
  "diffEditor.ignoreTrimWhitespace": false,
  "[yaml]": {
    "diffEditor.ignoreTrimWhitespace": true
  },
  "[markdown]": {
    "diffEditor.ignoreTrimWhitespace": true
  },

  // github copilot
  "github.copilot.enable": {
    "*": true,
    "plaintext": true,
    "markdown": true,
    "scminput": false,
    "yaml": true
  }
}
```
