# ASA-MEDIA-PROJECT

SNS・動画コンテンツの企画から投稿までをチームで管理するためのリポジトリです。  
GitHub の Issues・Projects と連携し、進捗の可視化とタスク漏れ防止を目的としています。

---

## 📌 プロジェクトの概要

| 項目 | 内容 |
|------|------|
| **目的** | YouTube・X（Twitter）・TikTok 等のコンテンツ企画・制作・投稿を一括管理する |
| **運用形態** | 企画 → 台本・素材準備 → 制作・編集 → レビュー → 投稿 の流れを Issue とタスクボードで可視化する |
| **主な利用者** | 企画・運用担当、編集者（必要に応じて参加） |

---

## 📂 フォルダ構成

```
ASA-MEDIA-PROJECT/
├── README.md                 # 本ファイル（概要・運用ルール・構成説明）
├── STATUS.md                 # 進捗サマリ（共有用1本リンク。LINE 等でこの URL を送る）
├── task_board.md             # タスク進捗の一覧（未着手・進行中・レビュー中・完了）
├── .github/
│   └── ISSUE_TEMPLATE/       # GitHub Issue のひな形
│       ├── video_planning.md # YouTube 動画企画用
│       └── sns_post.md       # X / TikTok 投稿用
├── contents/                 # 実際のコンテンツテキスト
│   ├── youtube/              # YouTube 動画の台本・構成
│   │   └── template_script.md
│   └── short_videos/         # ショート動画の企画メモ
│       └── template_idea.md
└── docs/                     # マニュアル・手順
    └── workflow.md           # 企画から投稿までの全体ワークフロー
```

---

## 🔄 運用ルール

### 1. タスク管理

- **進捗の確認**: 毎回のミーティングは `task_board.md` および GitHub の Issue / Projects のタスク一覧を見ながら開始する。
- **ステータス**: 未着手 → 進行中 → レビュー中 → 完了 のいずれかに必ず振り分ける。
- **担当**: Issue に Assignee を設定し、誰が何をいつまでにやるかを明確にする。

### 2. Issue の使い分け

- **YouTube 動画企画**: `.github/ISSUE_TEMPLATE/video_planning.md` を選択して Issue を作成する。
- **X / TikTok 投稿**: `.github/ISSUE_TEMPLATE/sns_post.md` を選択して Issue を作成する。
- その他のタスク（SOP 整備、テンプレ修正など）は通常の Issue で管理する。

### 3. コンテンツの配置

- 台本・企画メモは `contents/youtube/` または `contents/short_videos/` に配置する。
- ファイル名は日付や企画名を含め、検索しやすくする（例: `2026-02_〇〇企画_script.md`）。

### 4. 編集者への負担軽減

- タスクの更新・ラベル付けは主に運用担当が行い、編集者は「何を作るか」「どの状態か」を視覚的に把握できるようにする。
- 必要に応じて編集者を Issue にメンションし、レビューや確認を依頼する。

---

## 🚀 クイックスタート

1. **新規動画企画**: GitHub で New Issue → 「YouTube動画企画」テンプレートを選び、項目を記入する。
2. **新規 SNS 投稿**: 同様に「X/TikTok投稿」テンプレートで Issue を作成する。
3. **進捗確認**: `task_board.md` を開き、未着手・進行中・レビュー中・完了ごとの一覧を確認する。
4. **ワークフロー詳細**: `docs/workflow.md` で企画から投稿までの手順を確認する。

---

## 📤 進捗の共有（LINE など）

- **多数の人に「進捗はここで見られる」と伝えたいとき** → **[STATUS.md](STATUS.md)** の GitHub 上の URL を 1 本送る。
  - 例: `https://github.com/Asabis-Inc/ASA-MEDIA-PROJECT/blob/main/STATUS.md`
  - 開くと Markdown がレンダリングされ、サマリとタスク一覧・議事録へのリンクが表示される。
- より短い URL で共有したい場合は、GitHub Pages を有効化し、同じ内容をトップに置く運用も可能（詳細は Nexus 内 `11_Asabis/docs/Task_Management_View_And_Share_Draft.md` 参照）。

## 📎 関連リンク

- リポジトリ: [Asabis-Inc/ASA-MEDIA-PROJECT](https://github.com/Asabis-Inc/ASA-MEDIA-PROJECT)
- ミーティング議事録・運用メモ: Nexus 内 `11_Asabis/04_Meeting_Minutes/` を参照

---

*最終更新: 2026-02-21*
