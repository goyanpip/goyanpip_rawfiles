# goyanpip_rawfiles

**Language / 語言:** [English](#english) | [繁體中文](#繁體中文)

---

<a id="english"></a>
## 🇬🇧 English

This is my personal userscript and custom CSS for modifying HTML5 and YouTube. Recent YouTube has basically become unusable for me — they keep changing things, removing useful features, and shoving in useless "features" all the freaking time, and it drives me mad. So I've heavily modified the YouTube client into what I actually want, in the way that works best for me to watch videos and vtubers.

Below is an overview of what I've changed from the original YouTube webpage (note: **not** using VoraPis V3 / legacy YouTube plugins, etc.).

> ⚠️ **Disclaimer:** This is just my personal setup, and it may not be the best fit for you. Use it at your own risk! Remember to adjust things to your own preference before using it.

### 🧩 Recommended browser extensions

- **YouTube Auto HD** ー Automatically sets videos to your preferred quality. (Force)
- **Hide Shorts for YouTube™** ー Hides YouTube Shorts from the interface.
- **Return YouTube Dislike** ー Restores estimated dislike counts on YouTube videos.
- **Volume Booster for YouTube™** ー Boosts volume beyond YouTube’s default limit. Up to 400%.
- **YouTube LiveChat Flusher ー (Danmaku Chat)** Youtube Danmaku-style chat. Like Niconico.
- **YouTube Screenshot** ー Captures video frames as screenshots with one click.
- **YouTube Livestreams Theater Mode** ー A Theater Mode look like Twitch. 
- **YouTube 繁體自動翻譯修正** ー Fixed Traditional Chinese auto-translated subtitles.
- **SponsorBlock** ー Skips sponsor segments and other marked sections using community data.
- **DeArrow** ー Replaces clickbait titles and thumbnails with community-made alternatives.


### 🎨 Violentmonkey custom CSS userscript

I don't think I can share my custom Violentmonkey CSS userscript, since it might break GitHub's rules — I've heavily modified and rewritten other people's code to fit exactly what I want, so it's no longer really "theirs" to redistribute cleanly.

But, I can suggest what i installed and recommand for you:

### 🧷 Userscripts I currently have installed

| Script | Author | Version | Users | Last updated |
|---|---|---|---|---|
| YouTube Embed Enhancer | jmpatag | 3.2.0 | 658k | 12d ago |
| YouTube Restore Scrollable Fullscreen | [Waldoocs](https://x.com/Waldoocs) ([GitHub](https://github.com/Waldoocs)) | 1.975k | — | 109d ago |
| YouTube restore old views and dates on video cards | — | — | 1.38k | 110d ago |
| Make YouTube Think Firefox is Chrome | kosherkale | — | 1.215k | 156d ago |
| YouTube Boost Chat | CY Fung | 0.3.32 | 259k | 187d ago |
| YouTube Boost Chat 名稱修復 (Nickname Restoration for Boost Chat) | CY Fung + lisheng099 + Pekoradaisuki0112 / AI | 0.1.3 | 6k | 187d ago |
| YouTube 全螢幕管理器 | — | 1.6 | 17k | 167d ago |
| Youtube Thumbnail Unfucker | TB-303 | 0.2 | 3k | 215d ago |
| Restore YouTube Username from Handle to Custom | CY Fung | 0.14.8 | 183k | 124d ago |
| Youtube Live Clock | Derek | 1.8.1 | 6k | 491d ago |
| YouTube 乾淨短網址分享器 | Max | 1.1.8 | 19k | 109d ago |
| YouTube 超快聊天 | CY Fung | 0.102.2 | 7501k | 203d ago |
| Hide YouTube Sign Out Button | Blumsie | — | 12k | 491d ago |
| YTBetter - Enable Rewind/DVR | copyMister | 3.0 | 6k | 324d ago |

> ⚠️ **Heads up on `YTBetter - Enable Rewind/DVR`:** this one actually works — it lets you scrub back through a live stream like real DVR footage. But there's a bug: with it enabled, YouTube comments won't load, and the homepage stops loading more videos when you scroll down. Install at your own risk!


### 🚫 Custom uBlock filters

This is my **favourite part** — it fixes all the freaking bloated YouTube layout garbage that's ever been created. For example:

- Removes the YouTube "about" info clutter
- Cleans up the in-video player right-click menu (removes useless entries like "Copy embed code," "Copy debug info," and "Troubleshoot playback issues")
- Removes the fullscreen top-right overlay of like/dislike and the live chat tab
- **`youtube.com##ytd-mealbar-promo-renderer`** — hides the "Try YouTube Premium" mealbar popup that appears mid-browsing.
- **`youtube.com##ytd-popup-container:has(yt-mealbar-promo-renderer)`** — broader catch for Premium upsell popups.
- **`www.youtube.com##ytd-merch-shelf-renderer`** — removes the merch shelf under videos.
- **`www.youtube.com##ytd-ad-slot-renderer`** — general ad-slot container hider (test carefully, this can be broad).


### 🎨 Stylus — my YouTube theme (the real heavy lifting)

I also use Stylus, and honestly this is the heaviest, most-modified part of my whole setup — more than any single userscript. This is basically my custom YouTube visual theme, the direct UI/visual layer on top of everything else: all-round removal of rounded corners, an OLED dark theme, a compact sidebar on the subscriptions page, hidden bottom YouTube info bar, hidden YouTube Music and Studio tabs (useless to me), auto-hiding sidebar, disabled thumbnail hover previews, the old classic (2022-era) video player, a live-stream clock next to the player controls, an OLED player button menu, and a lot more on top of that.

I can't share the actual CSS — this is the part I've customized the most and don't want to redistribute in detail — but here are the names of the Stylus styles I currently have installed, if you want to look them up and build your own version:

- YouTube - Create Your Theme (1.8.5)
- YouTube Grid 5
- 垃圾圓角 <--- My own css
- 3 row Manage Channels Subscriptions - Jan 2024
- DLLM sidebar咁撚大 (jm91.0.1) <--- My own css lol (Not going to Public)
- Focus by BlazingMedia for YouTube Music
- More Thumbnails per row [YouTube] (1.2.5)
- No Rounded YouTube
- Remove AI Overview
- Remove Magenta Color From YouTube Studio (2.8)
- Remove Rounded Corners From YouTube Player (1.02)
- Remove Youtube Shorts from search results
- restore corners
- Revert YouTube Studio UI (1.0.6)
- Roundless YouTube
- toolbar修正位置 (5.0.0) <--- My own css
- YCS Extended
- youtube - HTML5 player upgrade
- YouTube for Normal People (1.6.13)
- Youtube October 2025 Rework
- YouTube Premium svg logo
- YouTube Studio Old Icons (1.03)
- Youtube Studio 低評価非表示 (Hide low ratings on dashboard)
- YouTube 側邊欄極致優化
- YouTube 訂閱欄窄版 (1.0.5)
- YouTube播放bar救星 <--- My own css
- YT - Revert classic 'Subscribed' notification icon
- YT Fixes (1.4.8)
- 搜尋美化 <--- My own css
- 改變佈局/收窄sidebar (1.3.4) <--- My own css
- 目前能用的直角icon修正 <--- My own css
- 移除高斯模糊 <--- My own css


### 📄 License / Notes

This is just my personal script which may not be the best fit for you. Use it at your own risk! Remember to adjust things to your preference before you use it.

---

<a id="繁體中文"></a>
## 🇹🇼 繁體中文

這是我個人使用的 userscript 以及自訂 CSS，用來修改 HTML5 網頁和 YouTube。因為原版的 YouTube 對我來說根本沒辦法用。一天到晚在那邊改東改西、移除有用的功能、加一堆沒用的破功能，快把我逼瘋了。最明顯的例子。一直改版、一直換 UI、一直塞新按鈕、播放器上面一堆沒必要的東西，側邊欄也一直亂改。所以我把 YouTube 客戶端重度魔改成我真正想要的樣子，用最適合我自己的方式來看影片跟追V。

以下是我對原始 YouTube 網頁所做的修改總覽（註：**不是**使用 VoraPis V3 或其他舊版 YouTube 外掛之類的東西）。

> ⚠️ **免責聲明：** 這只是我個人的設定，不一定適合你。使用前請自行承擔風險！使用前記得先改成你自己想要的樣子。

### 🧩 推薦安裝的擴充功能

- **YouTube Auto HD** ー 自動將影片設為你偏好的畫質。(強制)
- **Hide Shorts for Youtube™** ー 隱藏 YouTube Shorts 內容與入口。
- **Return YouTube Dislike** ー 恢復顯示 YouTube 影片的估算倒讚數。
- **Volume Booster for YouTube™** ー 將音量提升至高於 YouTube 預設上限。上限400%
- **YouTube LiveChat Flusher** ー Youtube彈幕功能。跟Niconico一樣
- **YouTube Screenshot** ー 一鍵擷取影片畫面為截圖。
- **YouTube Livestreams Theater Mode** ー 一種類似Twitch的劇院模式。
- **YouTube 繁體自動翻譯修正** ー 修復繁體中文自動翻譯字幕品質壞掉問題。
- **SponsorBlock** ー 透過社群標記自動跳過贊助、片頭、片尾等片段。
- **DeArrow** ー 以社群提供的非釣魚標題與縮圖取代原版本。


### 🎨 Violentmonkey 自訂 CSS userscript

我目前應該沒辦法分享我自己的 Violentmonkey 自訂 CSS userscript，因為這樣可能會違反 GitHub 的規範——我已經對別人的程式碼做了大量修改和重寫，改成我自己喜歡的樣子，所以已經不太算是原本「別人的」東西可以乾淨地轉發了。

但是我可以分享我安裝了哪些：

### 🧷 我目前有安裝的 userscript

| 腳本 | 作者 | 版本 | 使用者數 | 最後更新 |
|---|---|---|---|---|
| YouTube Embed Enhancer | jmpatag | 3.2.0 | 658k | 12 天前 |
| YouTube Restore Scrollable Fullscreen | [Waldoocs](https://x.com/Waldoocs)（[GitHub](https://github.com/Waldoocs)） | 1.975k | — | 109 天前 |
| YouTube restore old views and dates on video cards | — | — | 1.38k | 110 天前 |
| Make YouTube Think Firefox is Chrome | kosherkale | — | 1.215k | 156 天前 |
| YouTube Boost Chat | CY Fung | 0.3.32 | 259k | 187 天前 |
| YouTube Boost Chat 名稱修復 | CY Fung + lisheng099 + Pekoradaisuki0112 / AI | 0.1.3 | 6k | 187 天前 |
| YouTube 全螢幕管理器 | — | 1.6 | 17k | 167 天前 |
| Youtube Thumbnail Unfucker | TB-303 | 0.2 | 3k | 215 天前 |
| Restore YouTube Username from Handle to Custom | CY Fung | 0.14.8 | 183k | 124 天前 |
| Youtube Live Clock | Derek | 1.8.1 | 6k | 491 天前 |
| YouTube 乾淨短網址分享器 | Max | 1.1.8 | 19k | 109 天前 |
| YouTube 超快聊天 | CY Fung | 0.102.2 | 7501k | 203 天前 |
| Hide YouTube Sign Out Button | Blumsie | — | 12k | 491 天前 |
| YTBetter - Enable Rewind/DVR | copyMister | 3.0 | 6k | 324 天前 |

> ⚠️ **關於 `YTBetter - Enable Rewind/DVR` 的注意事項：** 這個腳本真的有效——可以像 DVR 一樣拖回直播的過去畫面。但有個 bug：啟用後留言區不會載入，首頁往下滾動也不會繼續讀取影片。安裝請自行承擔風險！


### 🚫 自訂 uBlock 過濾規則

這是我**最喜歡的部分**——可以把所有 YouTube 曾經做過的那些爛透了、沒用的版面垃圾全部幹掉。舉例來說：

- 移除 YouTube 影片「關於」資訊那堆雜訊
- 清理影片播放器右鍵選單（移除「複製嵌入程式碼」、「複製偵錯資訊」、「排解播放問題」這種沒用的項目）
- 移除全螢幕右上角那個讚/倒讚以及聊天室分頁的浮動覆蓋層
- **`youtube.com##ytd-mealbar-promo-renderer`** — 隱藏瀏覽途中彈出的「試用 YouTube Premium」促銷條。
- **`youtube.com##ytd-popup-container:has(yt-mealbar-promo-renderer)`** — 更廣泛地攔截 Premium 促銷彈窗。
- **`www.youtube.com##ytd-merch-shelf-renderer`** — 移除影片下方的周邊商品貨架區塊。
- **`www.youtube.com##ytd-ad-slot-renderer`** — 通用廣告版位隱藏規則（此規則範圍較廣，請謹慎測試）。


### 🎨 Stylus — 我的 YouTube 主題（真正花最多心力的部分）

我也有在用 Stylus，老實說這是我整套設定裡改最兇、最花心力的部分——比任何一個 userscript 都還要多。這基本上就是我的 YouTube 視覺主題，是最直接影響畫面的那一層：全部移除圓角、OLED 深色主題、訂閱頁面的精簡版側邊欄、隱藏底部 YouTube 資訊列、隱藏對我來說沒用的 YouTube Music 和 Studio 分頁、側邊欄自動隱藏、關閉縮圖預覽動畫、恢復舊版（2022 年那款）的經典播放器、直播旁邊加上即時時鐘、OLED 風格的播放器按鈕選單，以及其他更多細節。

實際的 CSS 我沒辦法分享——這是我改最多、最不想公開細節的部分——但如果你想自己研究、打造你自己的版本，以下是我目前安裝的 Stylus 樣式名稱：

- YouTube - Create Your Theme (1.8.5)
- YouTube Grid 5
- 垃圾圓角 <-- 私人css
- 3 row Manage Channels Subscriptions - Jan 2024
- DLLM sidebar咁撚大 (jm91.0.1) <-- 私人css超好笑（不打算公開）
- Focus by BlazingMedia for YouTube Music
- More Thumbnails per row [YouTube] (1.2.5)
- No Rounded YouTube
- Remove AI Overview
- Remove Magenta Color From YouTube Studio (2.8)
- Remove Rounded Corners From YouTube Player (1.02)
- Remove Youtube Shorts from search results
- restore corners
- Revert YouTube Studio UI (1.0.6)
- Roundless YouTube
- toolbar修正位置 (5.0.0) <-- 私人css
- YCS Extended
- youtube - HTML5 player upgrade
- YouTube for Normal People (1.6.13)
- Youtube October 2025 Rework
- YouTube Premium svg logo
- YouTube Studio Old Icons (1.03)
- Youtube Studio 低評価非表示 (Hide low ratings on dashboard)
- YouTube 側邊欄極致優化
- YouTube 訂閱欄窄版 (1.0.5)
- YouTube播放bar救星
- YT - Revert classic 'Subscribed' notification icon
- YT Fixes (1.4.8)
- 搜尋美化 <-- 私人css
- 改變佈局/收窄sidebar (1.3.4) <-- 私人css
- 目前能用的直角icon修正 <-- 私人css
- 移除高斯模糊 <-- 私人css

### 📄 授權／備註

這只是我個人的腳本，不一定是最適合你的做法。使用請自行承擔風險！使用前記得先改成你自己想要的設定。
