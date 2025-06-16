---
title: "web_copy — フォルダ運用 README"
updated: 2025-06-17
owner: "Soeno"
status: "approved"
---

# 01_web とは  
スタジオサイタマの **Web サイト用コピー／文言** を管理するディレクトリです。  
ライティング → レビュー → 本番デプロイ までをフォルダで段階管理します。

---

## フォルダ構成と役割

| フォルダ | 役割 | 編集権限 |
|----------|------|----------|
| **01_master** | **本番公開に使うマスター**。ここだけがデプロイ対象。 | 直接編集禁止<br>更新は Soeno のみ |
| **02_working** | ライターが草稿を書くワークスペース。`status: draft / review` を付けて PR | 全メンバー |
| **03_approved** | Kato / Soeno が内容を承認した後、一時的に置くステージング。 | Kato / Soeno |

---

## 更新手順（5ステップ）

1. **下書き作成**  
   `02_working` に新規 md を追加し `status: draft`  
   - セクション名は `NN_slug.md`（例 `02_speciality.md`）

2. **レビュー依頼**  
   `status: review` に変更
   - 修正箇所は `==ハイライト==`  
   - 補足は Callout `>` を使用

3. **承認**  
   Kato か Soeno が内容を確認し、`status: approved` へ
   03_approvedへ移動
   