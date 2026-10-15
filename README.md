<!-- ffxiv-tc-port 繁體中文說明開始 -->
# FfxivArgLauncher(台服 fork)

Dalamud 注入器自己啟動遊戲時用的輔助函式庫（上游 [ottercorp/FfxivArgLauncher](https://github.com/ottercorp/FfxivArgLauncher)）：建立遊戲行程、調整行程的存取權限（ACL），以及修補遊戲讀取登入參數的流程。

## 台服 fork 的目的

- 讓 Dalamud 本體的子模組網址指向本 org，建置不依賴上游 repo 是否還在、有沒有被改寫。

## 與上游的差異

- 沒有我方的 commit，分支內容與上游相同。
- Dalamud 本體釘的是以 .NET 9 為目標的版本；分支頂端多一顆上游改用 .NET 10 的 commit，本體沒有採用。

## 誰在用它

- [Dalamud](https://github.com/ffxiv-tc-port/Dalamud)：子模組 `lib/FfxivArgLauncher`，由 `Dalamud.Injector` 以專案參照引用。

<!-- ffxiv-tc-port 繁體中文說明結束 -->
