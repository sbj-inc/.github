Hi there 👋
# 🏗 sbj-inc — 開発方針 / Development Policy

## 🧩 ブランチの切り方
開発者は **issueごとにブランチ** を切って作業します。  
ブランチ名は **`issue-{番号}-{画面名(EN)}`** の形式で命名してください（例：`issue-123-Login`）。  
それ以外のブランチ（`fix/`, `hotfix/`, `release/` など）は現時点では不要です。  

**issueごとにブランチを切る理由：** プルリクエストが溜まれば溜まるほど、レビューやマージの負担が増え、開発フローが滞るためです。  
小規模な単位で進めることで、迅速なフィードバックと早期の統合を実現します。

この構成は初期構想段階のため、**プロジェクトの進捗や規模拡大に応じて見直し予定**です。


---

## 🧠 方針概要
- シンプルで再現性の高い開発フローを採用  
- 小規模チームでも高速に試行錯誤できる構成  
- 自動化・共通化を重視し、プロジェクト横断の整合性を維持  

---
## ストーリポイント目安

本プロジェクトでは、**スクラム開発＋Lean＋ページ駆動**をベースとした開発手法を採用しています。  
ストーリポイントは、作業の複雑さと不確実性を考慮して見積もります。

| ポイント | 難易度の目安       | 例                    |
| ---- | ------------ | -------------------- |  
| 1    | とても簡単（1時間以内） | バリデーション修正、小さな文言修正    |
| 2    | 簡単（半日以内）     | 画面上の軽微なAPI呼び出し追加     |
| 3    | 普通（1日程度）     | 新規API連携＋UI修正         |
| 5    | やや複雑（1〜2日）   | 新機能の中規模開発、外部APIとの統合  |
| 8    | 複雑（2〜3日）     | 新ページ＋複数API連携＋バリデーション |
| 13   | 非常に複雑（3〜5日）  | フロント・バック両対応、大規模リファクタ |
| 20   | 極めて不確実       | スパイク（調査）、大規模リデザイン    |

---
## 📋 スクラム開発の進め方

本プロジェクトでは、**スクラム開発＋Lean＋ページ駆動**をベースとした開発手法を採用しています。

### スプリントの流れ

1. **スプリント計画（Sprint Planning）**
   - プロダクトバックログから、スプリントで実現する目標を決定
   - 各ストーリーを詳細化し、タスクに分解
   - ストーリポイントを見積もり、スプリントバックログを作成

2. **デイリースタンドアップ（Daily Standup）**
   - 前日に何をしたか、今日何をするか、ブロッカーがないかを共有
   - 短時間（15分程度）で実施し、チームの進捗を可視化

3. **スプリントレビュー（Sprint Review）**
   - スプリントで完成した機能をデモし、ステークホルダーからフィードバックを受ける
   - ページ駆動の観点から、実際の画面やユーザーフローを確認

4. **レトロスペクティブ（Retrospective）**
   - スプリントを振り返り、良かった点・改善点を共有
   - Leanの考え方に基づき、無駄を削減し、価値の流れを改善

### 進め方の原則

- **小さな単位で価値を提供**：1つのストーリーは1つの画面や機能に焦点を当てる
- **継続的な改善**：レトロスペクティブで得た知見を次のスプリントに反映
- **透明性の確保**：進捗やブロッカーを可視化し、チーム全体で共有

---

## 🌍 Branching Strategy (English)
Developers should create **branches per issue** for new features.  
Branch names should follow the format **`issue-{number}-{screen-name}`** (e.g., `issue-123-login-screen`).  
Other branch types are **not required at this stage** (e.g., `fix/`, `hotfix/`, `release/`).  

**Why create branches per issue:** Accumulating pull requests increases review and merge overhead, slowing down the development flow.  
Working in smaller increments enables rapid feedback and early integration.

This is an **initial structure**, and will evolve as the project grows or development needs change.

---

## 🧭 Guiding Principles
- Keep the workflow simple and reproducible  
- Enable rapid prototyping within small teams  
- Maintain consistency through automation and shared standards
