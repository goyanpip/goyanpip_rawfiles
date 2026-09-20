# goyanpip_rawfiles

Personal userscripts, custom CSS, and uBlock Origin filters for making modern websites less annoying.
個人使用的 Userscript、Custom CSS 與 uBlock Origin Filter 集合，用來把現在那些越來越肥、越來越亂、越來越愛塞垃圾功能的網站改回比較能用的樣子。

---

## 🇬🇧 English

### Why?

Modern websites keep changing their UI, removing useful features, and adding more and more useless shit.
YouTube is probably the biggest example.

It keeps getting redesigned, features disappear, random buttons get added, the player gets covered with extra UI, and the sidebar keeps changing.

At some point I just thought:
**Fuck it. I'll change it myself.**

So this repository contains my personal modifications for websites I actually use. This is **not** meant to be a universal filter list. It's my browser, my preferences, and my way of getting rid of bullshit I don't want.

---

## 🇹🇼 繁體中文

### 為什麼做這個？

現在很多網站越做越肥，UI 越改越亂，原本好用的功能一直被刪掉，然後又一直加一些根本沒人在乎的 shit。
YouTube 是最明顯的例子。一直改版、一直換 UI、一直塞新按鈕、播放器上面一堆沒必要的東西，側邊欄也一直亂改。

最後我的想法就是：

**既然網站不給我想要的介面，那我自己改。**

所以這個 Repository 放的就是我平常實際使用的網站修改。這不是什麼「適合所有人」的 Filter List。

就是單純：
**我不爽的東西 → 刪掉。**  
**我覺得難用的東西 → 改掉。**  
**我想要的功能 → 自己補。**

---

# Features

### YouTube

The main target of this project.

My YouTube modifications mainly focus on:

- Removing unnecessary player UI and overlays
- Cleaning up the right-click menu
- Removing unwanted Live Chat elements
- Removing useless notifications
- Cleaning up the sidebar
- Reordering sidebar sections
- Removing unnecessary footer / country information
- Removing extra buttons and decorations
- Reducing visual clutter
- Keeping the player focused on the actual video

### What gets removed?

Some examples:

- `複製嵌入程式碼`
- `複製偵錯資訊`
- `排解播放問題`
- Unwanted Live Chat UI
- Extra player gradients
- Chapter decorations
- Unnecessary notification UI
- Promotional / experimental UI
- Extra sidebar sections
- Footer and copyright clutter

Basically, if something doesn't help me watch the video, navigate the site, or actually use YouTube, there's a good chance I removed it.

### What gets modified?
The filters don't only hide things.
Some parts are rearranged or customized.
For example, the YouTube sidebar is manually reordered so that the sections I actually use appear where I want them instead of following YouTube's default order.

---

# uBlock Origin
All uBlock Origin filters are stored in:

`filters.txt`

The filters cover multiple websites, including:

- YouTube
- Google / Gemini / Gmail / Drive
- Startpage
- GitHub
- Reddit
- Facebook / Instagram / X
- Twitch
- Bilibili / Pixiv / NicoNico
- Wikipedia
- edX
- PyPI / Python
- Proton Mail
- Canva
- Chess.com
- and various other websites I use

The purpose is generally the same:

**Remove clutter, promotions, unnecessary UI, annoying widgets, and shit I don't want to see.**
Some filters simply hide an element.
Others change the layout or remove an entire section.

---

# Personal CSS / Userscripts

I also use a heavily customized CSS userscript through Violentmonkey. It has been modified and rewritten quite heavily from other people's code to fit my own preferences. Because of that, the complete userscript is not currently included here. The uBlock filters are the more portable part of this project.

---

# Recommended Extensions

These work well with my setup:

- YouTube Auto HD
- Hide Shorts for YouTube™
- Return YouTube Dislike
- Volume Booster for YouTube™
- YouTube LiveChat Flusher / Danmaku Chat
- YouTube Screenshot
- YouTube Livestreams Theater Mode
- YouTube 繁體自動翻譯修正

---

# Important

These filters are **highly personal**.

They may:

- Break after a website redesign
- Hide something you actually want
- Stop working when CSS class names change
- Conflict with other extensions
- Look completely fucking ridiculous to someone with different preferences

That's fine.

I made these for **my own browser experience**. Modern websites change their frontend constantly, so maintenance is expected.

---

# Philosophy

> If I don't need it, remove it.

I don't want websites deciding what my interface should look like.

I don't need another giant banner.

I don't need another useless button.

I don't need another promotional popup.

I don't need five different features doing basically the same fucking thing.

I just want the website to be usable.

So I remove the shit I don't want and keep the parts I actually use.

---

# Files

```text
goyanpip_rawfiles/
├── README.md
├── filters.txt
└── ...
