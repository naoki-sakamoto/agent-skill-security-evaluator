---
description: Generate commit message using AI analysis of staged changes
allowed-tools: Task
---

# Commit-Message

AIエージェントを使用してステージされた変更から適切なコミットメッセージを生成

## Instructions

git diff --stagedの内容を分析し、以下の形式でコミットメッセージを日本語で生成してください：

1. 1行目: 変更の要約（50文字以内）
2. 2行目: 空行
3. 3行目以降: 詳細な説明
   - 何を変更したか
   - なぜ変更したか
   - 影響範囲

Conventional Commitsの形式に従ってください：
- feat: 新機能
- fix: バグ修正
- docs: ドキュメント
- style: フォーマット
- refactor: リファクタリング
- test: テスト
- chore: その他

## 注意事項

- コミットメッセージにはシングルクォート（'）やダブルクォート（"）を含めないでください
- 特殊文字やエスケープが必要な文字は避けてください
- ファイル名やパスを記載する場合は、括弧や引用符を使わずに記載してください