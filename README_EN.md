# TabPulse (ye!)

<p align="left">
  <a href="README.md">简体中文</a> | <b>English</b> | <a href="README_JA.md">日本語</a>
</p>

<p align="left">
  <a href="https://github.com/chenyiwanshishen-source/TabPulse/releases/latest/download/TabPulse-v2.0-trial.zip">
    <img src="https://img.shields.io/badge/%F0%9F%93%A6%20Download%20Trial-v2.0.0--trial-22c55e?style=for-the-badge" alt="Download Trial" />
  </a>
  <a href="https://github.com/chenyiwanshishen-source/TabPulse/releases/latest">
    <img src="https://img.shields.io/badge/Releases-Latest%20Release-2563eb?style=for-the-badge" alt="Releases" />
  </a>
</p>

A clean Chrome extension to manage your open tabs and bookmarks on one full-screen visual canvas. Built-in native support for English, Simplified Chinese, and Japanese, automatically matching your browser language.

When researching or working online, tabs easily pile up into the dozens. Closing them risks losing information; keeping them open slows down your browser. Bookmarks pile up into the thousands, becoming impossible to search through.
TabPulse solves this straightforwardly: it lays everything out on a clean full-screen board where you can search, drag, drop, and deduplicate. When you connect your own AI API key, you can ask it in plain language to organize, categorize, and clean up your collection, with multi-step undo for safety.

---

## Key Features

- **Fullscreen Visual Workspace**: View all open browser windows, tab groups, and bookmark trees on a single panoramic board. Drag and drop freely to reorganize.
- **Quick Bookmark Capsule**: Press a shortcut on any page to open a lightweight capsule drawer and save the page without interrupting your reading.
- **Bring Your Own AI Model**: Supports OpenAI, Claude, DeepSeek, SiliconFlow, MiniMax, Moonshot, and local Ollama. Simply paste your API key; the extension auto-detects the provider.
- **Natural Language Organizing**: Tell the AI what you want in plain words (e.g., "Group all design system articles into a new folder", "Find duplicate links"). The AI presents an interactive plan drawer for your confirmation before touching anything.
- **Multi-Step Undo**: Every AI action or batch change has a history trail. Undo any unwanted step with one click (default keeps 5 undo steps, customizable in settings).
- **Native Trilingual Support**: Full interface translations for English, 简体中文, and 日本語, automatically switching based on your system language.
- **Strict Local Privacy**: No private telemetry or intermediate servers. All bookmarks and API keys stay inside your browser's local storage (`chrome.storage`). AI requests are dispatched directly from your browser to your chosen model provider.

---

## Trilingual Terminology & Feature Comparison (多语言对照)

All actions and features correspond directly across English, Chinese, and Japanese:

| English | 简体中文 (Chinese) | 日本語 (Japanese) | Description |
|---|---|---|---|
| **Fullscreen Workspace** | 全屏看板 / 工作台 | フルスクリーンワークスペース | Panoramic board to organize tabs and bookmarks |
| **Bookmark current page** | 收藏当前页面 | 現在のページを保存 | Quick shortcut to save the active webpage |
| **Quick actions** | 快捷操作 | クイック操作 | Batch actions: deduplication, dead links, grouping |
| **AI organization** | AI 智能整理 | AI 整理 | Natural language dialog-driven reorganization |
| **Tab plan preview** | 页签整理方案预览 | タブ整理案のプレビュー | Interactive confirmation drawer before applying changes |
| **One-click undo supported** | 支持一键撤销 | ワンクリックで元に戻せます | Multi-step rollback protection against mistakes |
| **Find duplicates** | 检查重复项 | 重複をチェック | Scan and remove duplicate bookmark entries |
| **Check broken links** | 检查失效网址 | リンク切れをチェック | Check for dead or unreachable URLs |
| **Trash** | 回收站 | ゴミ箱 | Safely hold deleted items before permanent removal |
| **Allow AI to control webpages** | 允许 AI 操作网页 | AI によるウェブページ操作を許可 | Optional permission for deeper reading and automation |

---

## 30-Second Quick Start

This repository contains a pre-built extension package ready to load directly into Google Chrome.

### 1. Load into Chrome

1. Go to [Releases](https://github.com/chenyiwanshishen-source/TabPulse/releases/latest) and download **[TabPulse-v2.0-trial.zip](https://github.com/chenyiwanshishen-source/TabPulse/releases/latest/download/TabPulse-v2.0-trial.zip)**, then unzip it to a local folder.
2. Open Google Chrome and navigate to:
   ```text
   chrome://extensions/
   ```
3. Toggle on **Developer mode** in the top-right corner.
4. Click **Load unpacked** in the top-left corner.
5. Select this unpacked directory (the one containing `manifest.json`).

### 2. Quick Bookmark Shortcut

On any web page, press the default shortcut to bring up the quick bookmark capsule:
- **Mac**: `Option` (⌥) + `Shift` (⇧) + `D`
- **Windows**: `Alt` + `Shift` + `D`

> To customize the shortcut, go to `chrome://extensions/shortcuts` in your browser.

### 3. Add Your AI API Key

When you are ready to try AI-assisted organization:
1. Click the extension icon to open the TabPulse workspace, then open the Settings modal.
2. Paste your API key into the configuration field. The extension will automatically match the provider and model.
3. The key is stored purely inside your local browser and can be replaced or cleared anytime.

---

## Feedback & Community

TabPulse is an actively evolving project. If you spot a bug, run into lag, or have design suggestions, please feel free to open an Issue on GitHub. Enjoy your organized browsing!

---

## License

This project is released under the [MIT License](LICENSE).
