tg\_stickers\_helper
---

一個批量 Telegram Sticker 匯入工具。先與 `@Stickers` 對話，進入到讓妳發送 png 的會話時就可以使用這個工具了。

首先，編譯 tg-cli 並開啟 RPC：

```
telegram-cli --json -P 9000
```

`tg_stickers_helper` 從標準輸入讀取 json，格式如下：

```
{png: "/path/to/png", emoji: "emoji"}
```

也就是說：

```
./tg_stickers_helper < stickers.json
```

以上。
