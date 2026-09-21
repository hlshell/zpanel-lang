# zpanel-lang

zpanel 的國際化（i18n）語言文件，使用 JSON 格式提供介面文字與翻譯內容。

## 語言文件位置

請將語言 JSON 文件存放在 zpanel 二進制目錄下的 `etc/lang` 目錄內：

```text
<zpanel-binary-directory>/etc/lang/
```

例如：

```text
/usr/local/zpanel/etc/lang/
```

## 文件格式

每個語言使用一個獨立的 JSON 文件，文件名稱通常使用語言代碼，例如：

```text
etc/lang/en.json
etc/lang/zh-TW.json
etc/lang/zh-CN.json
```

JSON 文件中的鍵值應保持與 zpanel 使用的語言鍵一致，值則填入對應語言的翻譯：

```json
{
  "app.title": "zpanel",
  "common.save": "儲存",
  "common.cancel": "取消"
}
```

## 新增或修改翻譯

1. 在二進制目錄下建立或編輯 `etc/lang/<language-code>.json`。
2. 使用有效的 UTF-8 JSON 格式。
3. 保留既有語言鍵，不要任意更改鍵名。
4. 完成後重新啟動 zpanel，讓新的語言文件生效。
