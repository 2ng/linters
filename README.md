### @2ng/linters

## Stylelint

`.stylelintrc`

```json
{
  "extends": ["@tinkoff/linters/stylelint/bases/prettier.stylelint.json"]
}
```

---

`package.json`

Добавить в поле `scripts` команду:

```json
  "lint:styles": "stylelint --config .stylelintrc --fix \"./**/*.scss\""
```

Выполнение команды `npm run lint:styles` найдет все файлы `.scss` и перезапишет в отформатированном виде, согласно правилам файла `.stylelintrc`.

---

`VsCode`

Установить `stylelint.vscode-stylelint`

Для автоформата при сохранении в поле `editor.codeActionsOnSave` в `settings.json` добавить:

```json
  "source.fixAll.stylelint": true
```
---