# TabPulse (ye!)

<p align="left">
  <a href="README.md">简体中文</a> | <a href="README_EN.md">English</a> | <b>日本語</b>
</p>

<p align="left">
  <a href="https://github.com/chenyiwanshishen-source/TabPulse/releases/latest/download/TabPulse-v2.0-trial.zip">
    <img src="https://img.shields.io/badge/%F0%9F%93%A6%20%E3%81%8A%E8%A9%A6%E3%81%97%E7%89%88%E3%82%92%E3%83%80%E3%82%A6%E3%83%B3%E3%83%AD%E3%83%BC%E3%83%89-v2.0.0--trial-22c55e?style=for-the-badge" alt="お試し版をダウンロード" />
  </a>
  <a href="https://github.com/chenyiwanshishen-source/TabPulse/releases/latest">
    <img src="https://img.shields.io/badge/Releases-%E3%83%AA%E3%83%AA%E3%83%BC%E3%82%B9%E4%B8%80%E8%A6%A7-2563eb?style=for-the-badge" alt="Releases" />
  </a>
</p>

<p align="center">
  <img src="icons/brand/mascot-scratch.webp" alt="頭をかくフォルダーキャラクター" width="150" />
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <img src="icons/brand/mascot-wave.webp" alt="手を振るフォルダーキャラクター" width="120" />
  <br />
  <sub>ツールに親しみやすさを添えるため、日常的なフォルダーの形をベースに動くマスコットキャラクターをデザインしました。</sub>
</p>

開いているタブとブックマークをひとつの大画面キャンバスで直感的に整理できる Chrome 拡張機能です。日本語、英語、簡体字中国語の 3 言語にネイティブ対応しており、ブラウザの言語設定に応じて自動で切り替わります。

調べ物をしているとタブが数十個も開きっぱなしになり、閉じると後で困るし、開いたままだと重くなる。ブックマークも気づけば何千個も溜まり、探すのが大変――。
TabPulse は、そんな日常のストレスを解消するために作られました。見やすいフルスクリーン看板でドラッグ＆ドロップ、検索、重複整理ができるほか、お好みの AI API キーを登録すれば、普段の自然な言葉でまとめて整理を依頼できます。操作はいつでも元に戻せる安全設計です。

---

## 主な機能

- **フルスクリーンワークスペース**: 開いているすべてのウィンドウ、タブグループ、ブックマークフォルダーをパノラマ表示。直感的なドラッグ＆ドロップで自在に整理できます。
- **現在のページをクイック保存**: 閲覧中にショートカットキーを押すだけで、邪魔にならない小さなカプセル型ドロワーが開き、読書を中断せずにすぐ保存できます。
- **お好みの AI モデルと連携**: OpenAI、Claude、DeepSeek、SiliconFlow、MiniMax、Moonshot、ローカルの Ollama に対応。API キーを貼り付けるだけで、対応サービスを自動認識します。
- **自然な言葉で AI 整理**: 「デザイン関連の記事を新しいフォルダーにまとめて」「重複しているリンクを探して」など、普段の話し言葉で指示できます。AI は実行前に必ず確認ドロワーを表示するため、勝手に変更される心配はありません。
- **安心の取り消し機能**: AI の整理や手動の一括操作には履歴が記録され、ワンクリックで前の状態に戻せます（標準で直近 5 回分保持、設定で変更可能）。
- **3 言語ネイティブ対応**: 日本語、English、简体中文の UI を完全収録。ブラウザ言語に合わせて自動で最適化されます。
- **ローカル完結のプライバシー保護**: 開発者独自のサーバーは存在せず、閲覧履歴やブックマークを収集することはありません。データと API キーはすべてブラウザ内（`chrome.storage`）に安全に保存され、AI 呼び出し時はブラウザから各社公式 API へ直接送信されます。

---

## 機能デモ（1.5倍速）

> すべてのデモ動画は要点をスムーズにご確認いただけるよう、あらかじめ **1.5倍速** に調整されています。

### 1. ログインと API Key 設定（貼り付けるだけで自動認識）

https://github.com/user-attachments/assets/a276fb8f-366e-48de-8ec2-2d9c1c12feb8

### 2. フルスクリーンタブ看板とリアルタイム編集

https://github.com/user-attachments/assets/d89a6602-4983-43b7-a275-41d5264fbffe

### 3. AI によるブックマークの一括整理（実行前確認ドロワー）

https://github.com/user-attachments/assets/84aa6437-7b4f-4260-87de-b6c378098737

---

## 3 言語 機能・用語対照表 (Trilingual Comparison)

本拡張機能のすべての機能・UI 表記は、日・英・中の 3 言語で直接対応しています:

| 日本語 (Japanese) | English | 简体中文 (Chinese) | 説明 |
|---|---|---|---|
| **フルスクリーンワークスペース** | Fullscreen Workspace | 全屏看板 / 工作台 | タブとブックマークを一覧整理する大画面キャンバス |
| **現在のページを保存** | Bookmark current page | 收藏当前页面 | ショートカットで素早く現在地をブックマーク |
| **クイック操作** | Quick actions | 快捷操作 | 重複削除、リンク切れ検査、一括グループ化 |
| **AI 整理** | AI organization | AI 智能整理 | 自然言語の対話によるフォルダー分類と構造整理 |
| **タブ整理案のプレビュー** | Tab plan preview | 页签整理方案预览 | 実行前にユーザーが確認できる計画ドロワー |
| **ワンクリックで元に戻せます** | One-click undo supported | 支持一键撤销 | 誤操作を防ぐ多段階の取り消し機能 |
| **重複をチェック** | Find duplicates | 检查重复项 | 重複登録されたリンクを検出してクリーンアップ |
| **リンク切れをチェック** | Check broken links | 检查失效网址 | アクセスできなくなった URL をすばやく特定 |
| **ゴミ箱** | Trash | 回收站 | 削除項目を一時保持し、期間内の復元に対応 |
| **AI によるウェブページ操作を許可** | Allow AI to control webpages | 允许 AI 操作网页 | AI アシスタントが詳細な読解を行うための拡張機能 |

---

## 30 秒で試せるインストール手順

ビルド済みパッケージのため、Google Chrome にそのまま読み込んですぐに使えます。

### 1. ダウンロードと Chrome への読み込み

以下のいずれかの方法でお試し版パッケージを取得できます:
- **方法 A (手軽に一括)**: リポジトリ右上の緑色の **`<> Code` → `Download ZIP`** をクリックしてダウンロードし、展開します。
- **方法 B (Releases ページ)**: ページ上部のダウンロードボタン、または [Releases ページ](https://github.com/chenyiwanshishen-source/TabPulse/releases/latest) から **[TabPulse-v2.0-trial.zip](https://github.com/chenyiwanshishen-source/TabPulse/releases/latest/download/TabPulse-v2.0-trial.zip)** をダウンロードし、展開します。

展開後、以下の手順で Chrome に読み込みます:
1. Chrome ブラウザを開き、アドレスバーに以下を入力して Enter を押します:
   ```text
   chrome://extensions/
   ```
3. 画面右上の **「デベロッパー モード」** スイッチをオンにします。
4. 左上に表示される **「パッケージ化されていない拡張機能を読み込む」** ボタンをクリックします。
5. 解凍したフォルダー（`manifest.json` が入っているディレクトリ）を選択すれば完了です。

### 2. ショートカットでクイック保存

任意のウェブページでデフォルトのショートカットキーを押すと、保存カプセルが表示されます:
- **Mac**: `Option` (⌥) + `Shift` (⇧) + `D`
- **Windows**: `Alt` + `Shift` + `D`

> キーの変更は、Chrome の `chrome://extensions/shortcuts`（拡張機能 → キーボード ショートカット）からいつでも行えます。

### 3. API Key の設定（貼り付けるだけで自動認識）

AI による整理機能は、キーを貼り付けるだけで手軽に使えます:
1. **DeepSeek API Key の利用がおすすめ**: 最もおすすめなのは DeepSeek の API Key です。ブックマーク整理ではページ一覧をまとめて送る必要がありますが、DeepSeek はキャッシュが非常によく効くため、利用料を大幅に抑えられます。**500 件のブックマークを一括整理**した場合でも、1 回あたりの費用はおよそ **0.1 元前後（約 0.014 米ドル / 約 2 円程度）** です。溜まった大量のリンクも気兼ねなくまとめて整理できます。
2. **ホーム画面でそのまま貼り付け**: TabPulse を開いて、AI パネルに直接 Key を貼り付けます（DeepSeek のほか、Claude、OpenAI、SiliconFlow、MiniMax、Moonshot、ローカル Ollama にも対応）。提供元は自動認識されるため、手動で細かい設定を選ぶ必要はありません。
3. **設定画面でいつでも変更可能**: 後から別のモデルに切り替えたい場合も、設定モーダルで新しい Key を貼り付けるだけで同様に認識されます。
4. **ブラウザ内にのみ安全保存**: Key はお使いのブラウザ内部（`chrome.storage`）にのみ保存され、外部サーバーに送信されることは一切ありません。いつでもワンクリックで削除できます。

---

## ご意見・フィードバック

現在も継続して改善を行っている開発版です。不具合、動作の重さ、デザインや使い勝手に関するご提案など、お気づきの点がございましたら GitHub の Issue までお気軽にお寄せください。快適なブラウジングをお楽しみください！

---

## ライセンス

本プロジェクトは [MIT ライセンス](LICENSE) のもとで公開されています。
