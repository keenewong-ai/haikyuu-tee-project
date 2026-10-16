# 排球少年靈感 T 恤設計｜專案板

可視化專案看板（單頁 HTML），方便用瀏覽器睇素材／設計稿進度。

## 打開方式

- 本機：用瀏覽器開 `index.html`
- 線上：見 GitHub Pages URL（推送後生效）

## 點樣更新卡片

直接改 `index.html`：

1. **加新素材**：喺 `#materialCards` 入面複製一張 `.card`，改 `data-id`、`M-xxx`、標題、來源、狀態 pill。
2. **改狀態**：把 pill class／文字改成：
   - `pill-pending` → 待審
   - `pill-selected` → 已選用
   - `pill-rejected` → 已否決
   - `pill-designing` → 設計中
   - `pill-done` → 完成
3. **加設計稿**：刪除／隱藏 `#designEmpty`，喺 `#designs` 加同素材一樣結構嘅 `.card`，編號用 `D-001`…
4. **更新時間**：改 header 入面 `#lastUpdated` 文字（Asia/Taipei，例如 `2026-10-16 15:47 HKT`）。
5. **流程步驟**：改 `.step` 嘅 `active` class 同 pill。

改完後 `git add` → `commit` → `push`，Pages 會自動更新。

## 版權

唔好放《排球少年!!》官方角色圖、作品名商標、經典台詞上頁面或商品。只用可商用剪影＋原創字體排版。

## 編號

- 素材：`M-001`, `M-002`, …
- 設計稿：`D-001`, `D-002`, …
