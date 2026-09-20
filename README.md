# goyanpip_rawfiles

**Language / 語言:** [English](#english) | [繁體中文](#繁體中文)

---

<a id="english"></a>
## 🇬🇧 English

This is my personal userscript and custom CSS for modifying HTML5 and YouTube. Recent YouTube has basically become unusable for me — they keep changing things, removing useful features, and shoving in useless "features" all the freaking time, and it drives me mad. So I've heavily modified the YouTube client into what I actually want, in the way that works best for me.

Below is an overview of what I've changed from the original YouTube webpage (note: **not** using VoraPis V3 / legacy YouTube plugins, etc.).

> ⚠️ **Disclaimer:** This is just my personal setup, and it may not be the best fit for you. Use it at your own risk! Remember to adjust things to your own preference before using it.

### 🧩 Recommended browser extensions

- **YouTube Auto HD**
- **Hide Shorts for YouTube™**
- **Return YouTube Dislike**
- **Volume Booster for YouTube™**
- **YouTube LiveChat Flusher (Danmaku Chat)**
- **YouTube Screenshot**
- **YouTube Livestreams Theater Mode**
- **YouTube 繁體自動翻譯修正**

### 🎨 Violentmonkey custom CSS userscript

I don't think I can share my custom Violentmonkey CSS userscript, since it might break GitHub's rules — I've heavily modified and rewritten other people's code to fit exactly what I want, so it's no longer really "theirs" to redistribute cleanly.

### 🚫 Custom uBlock filters

This is my **favourite part** — it fixes all the freaking bloated YouTube layout garbage that's ever been created. For example:

- Removes the YouTube "about" info clutter
- Cleans up the in-video player right-click menu (removes useless entries like "Copy embed code," "Copy debug info," and "Troubleshoot playback issues")
- Removes the fullscreen top-right overlay of like/dislike and the live chat tab
- **`youtube.com##ytd-mealbar-promo-renderer`** — hides the "Try YouTube Premium" mealbar popup that appears mid-browsing.
- **`youtube.com##ytd-popup-container:has(yt-mealbar-promo-renderer)`** — broader catch for Premium upsell popups.
- **`www.youtube.com##ytd-merch-shelf-renderer`** — removes the merch shelf under videos.
- **`www.youtube.com##ytd-ad-slot-renderer`** — general ad-slot container hider (test carefully, this can be broad).

### 📄 License / Notes

This is just my personal script which may not be the best fit for you. Use it at your own risk! Remember to adjust things to your preference before you use it.

---

<a id="繁體中文"></a>
## 🇹🇼 繁體中文

這是我個人使用的 userscript 以及自訂 CSS，用來修改 HTML5 網頁和 YouTube。因為原版的 YouTube 對我來說根本沒辦法用。一天到晚在那邊改東改西、移除有用的功能、加一堆沒用的破功能，快把我逼瘋了。最明顯的例子。一直改版、一直換 UI、一直塞新按鈕、播放器上面一堆沒必要的東西，側邊欄也一直亂改。所以我把 YouTube 客戶端重度魔改成我真正想要的樣子，用最適合我自己的方式來看影片跟追V。

以下是我對原始 YouTube 網頁所做的修改總覽（註：**不是**使用 VoraPis V3 或其他舊版 YouTube 外掛之類的東西）。

> ⚠️ **免責聲明：** 這只是我個人的設定，不一定適合你。使用前請自行承擔風險！使用前記得先改成你自己想要的樣子。

### 🧩 推薦安裝的擴充功能

- **YouTube Auto HD**
- **Hide Shorts for Youtube™**
- **Return YouTube Dislike**
- **Volume Booster for YouTube™**
- **YouTube LiveChat Flusher（彈幕聊天室）**
- **YouTube Screenshot**
- **YouTube Livestreams Theater Mode**
- **YouTube 繁體自動翻譯修正**

### 🎨 Violentmonkey 自訂 CSS userscript

我目前應該沒辦法分享我自己的 Violentmonkey 自訂 CSS userscript，因為這樣可能會違反 GitHub 的規範——我已經對別人的程式碼做了大量修改和重寫，改成我自己喜歡的樣子，所以已經不太算是原本「別人的」東西可以乾淨地轉發了。

### 🚫 自訂 uBlock 過濾規則

這是我**最喜歡的部分**——可以把所有 YouTube 曾經做過的那些爛透了、沒用的版面垃圾全部幹掉。舉例來說：

- 移除 YouTube 影片「關於」資訊那堆雜訊
- 清理影片播放器右鍵選單（移除「複製嵌入程式碼」、「複製偵錯資訊」、「排解播放問題」這種沒用的項目）
- 移除全螢幕右上角那個讚/倒讚以及聊天室分頁的浮動覆蓋層
- **`youtube.com##ytd-mealbar-promo-renderer`** — 隱藏瀏覽途中彈出的「試用 YouTube Premium」促銷條。
- **`youtube.com##ytd-popup-container:has(yt-mealbar-promo-renderer)`** — 更廣泛地攔截 Premium 促銷彈窗。
- **`www.youtube.com##ytd-merch-shelf-renderer`** — 移除影片下方的周邊商品貨架區塊。
- **`www.youtube.com##ytd-ad-slot-renderer`** — 通用廣告版位隱藏規則（此規則範圍較廣，請謹慎測試）。

### 📄 授權／備註

這只是我個人的腳本，不一定是最適合你的做法。使用請自行承擔風險！使用前記得先改成你自己想要的設定。
