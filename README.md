# TabPulse (ye!)

<p align="left">
  <b>简体中文</b> | <a href="README_EN.md">English</a> | <a href="README_JA.md">日本語</a>
</p>

一款集中管理浏览器标签页与书签的 Chrome 扩展.内置中文,英文,日文三种语言界面,根据系统语言自动匹配.

平时查资料开几十个标签页,关了怕丢,不关又卡;书签存了几千个,越积越乱,找起来像大海捞针.
TabPulse 就是为了解决这件事做的:给你一个干净清晰的全屏大看板,能拖拽,能搜索,能去重;接上你自己的 AI 密钥后,还能直接用大白话让它帮你批量分类和整理,而且改动支持多步撤销.

---

## 核心功能

- **全屏工作台**:把所有打开的标签页和书签树平铺在看板里,窗口,分组,层级一眼看清,支持直接拖拽整理.
- **快速唤醒收藏**:浏览任意网页时按快捷键,弹出轻量胶囊面板快速归档,不打断当前阅读.
- **接自己的 AI 模型**:支持 OpenAI,Claude,DeepSeek,硅基流动,MiniMax,Moonshot 以及本地 Ollama.直接填入 API Key 即可,插件会自动识别对应配置.
- **自然语言辅助整理**:可以用大白话给 AI 下指令(比如"把所有跟设计规范相关的网页单独建个文件夹归类","找出重复的书签").AI 在动手前会先展示操作计划抽屉,由你确认后再执行.
- **安全可撤销**:任何 AI 或手动批量操作都有历史记录,误操作支持一键按步撤销(默认保留 5 步,可在设置中调整).
- **多语言原生支持**:界面内置简体中文,English 与日本語,随浏览器系统语言自动切换.
- **隐私干净**:没有我们自己的云端服务器,不收集你的浏览历史和书签.所有数据和 API Key 都保存在浏览器本地(`chrome.storage`),调用 AI 时直接由你的浏览器向模型厂商官方接口发起请求.

---

## 多语言核心功能与术语对照 (Language Comparison / 言語対照)

插件内所有交互与功能均提供中,英,日三语原生对照:

| 简体中文 (Chinese) | English | 日本語 (Japanese) | 说明 / Description |
|---|---|---|---|
| **全屏看板 / 工作台** | Fullscreen Workspace | フルスクリーンワークスペース | 平铺管理所有标签页与书签树的大看板 |
| **收藏当前页面** | Bookmark current page | 現在のページを保存 | 默认快捷键快速归档当前网页 |
| **快捷操作** | Quick actions | クイック操作 | 一键去重,检查失效与批量分组 |
| **AI 智能整理** | AI organization | AI 整理 | 自然语言对话式归类与层级重构 |
| **页签整理方案预览** | Tab organization plan preview | タブ整理案のプレビュー | 执行前由用户确认的操作计划抽屉 |
| **支持一键撤销** | One-click undo supported | ワンクリックで元に戻せます | 历史记录按步撤销,防止误操作 |
| **检查重复项** | Find duplicates | 重複をチェック | 扫描并清理重复收藏的书签链接 |
| **检查失效网址** | Check broken links | リンク切れをチェック | 快速排查无法访问的死链 |
| **回收站** | Trash | ゴミ箱 | 暂时存放删除项,支持期限内恢复 |
| **允许 AI 操作网页** | Allow AI to control webpages | AI によるウェブページ操作を許可 | 可选高级权限,由模型辅助深度浏览 |

---

## 30 秒安装与使用

这是一个免打包的已编译体验版,直接载入 Chrome 即可使用.

### 1. 安装到 Chrome

1. 前往 [Releases 发布页面](https://github.com/chenyiwanshishen-source/TabPulse/releases/latest) 点击下载 **[TabPulse-v2.0-trial.zip](https://github.com/chenyiwanshishen-source/TabPulse/releases/latest/download/TabPulse-v2.0-trial.zip)** 安装包,并解压到你常用的本地文件夹.
2. 打开 Chrome 浏览器,在地址栏输入并回车:
   ```text
   chrome://extensions/
   ```
3. 在页面右上角打开 **"开发者模式"** 开关.
4. 点击左上角出现的 **"加载已解压的扩展程序"** 按钮.
5. 选择解压后的文件夹(包含 `manifest.json` 的目录)即可完成加载.

### 2. 快捷键收藏网页

在任意网页上按默认快捷键即可呼出收藏胶囊:
- **Mac**: `Option` (⌥) + `Shift` (⇧) + `D`
- **Windows**: `Alt` + `Shift` + `D`

> 如果快捷键被其他软件占用或想换键位,可在浏览器的 `chrome://extensions/shortcuts` (扩展程序 → 键盘快捷键) 中直接修改.

### 3. 配置 API Key

首次使用 AI 整理功能时:
1. 点击插件图标打开 TabPulse 主界面,进入设置面板.
2. 在 API 配置栏直接粘贴你自己的 API Key(支持各大主流平台或本地模型),插件会自动匹配对应的厂商与接口.
3. 密钥只保存在你的本地浏览器中,随时可清除或更换.

---

## 欢迎反馈

这是一个仍在持续迭代的测试版本.如果在使用中遇到 bug,卡顿,或者对交互和功能有任何想法与吐槽,都欢迎在 GitHub 提 Issue 反馈.祝你整理顺手,浏览愉快!

---

## 开源协议

本项目采用 [MIT 许可证](LICENSE).
