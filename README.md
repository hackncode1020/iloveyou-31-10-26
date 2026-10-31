# I Love You in 52 Languages 🌍❤️🌹

**Live demo:** https://iloveyou-langs-hackncode.sites.tab.bot/
**Personalised:** https://iloveyou-langs-hackncode.sites.tab.bot/?name=Jaan

A slow, cinematic, one-page love website: it says **"I love you" in 52 languages** (50+), then every word gathers into a giant glowing particle **heart** with your love's pet name in the middle, and the heart blooms into a detailed **rose** 🌹.

Day 5 of 100 · made by [@hack.n.code](https://www.instagram.com/hack.n.code/)

## ✨ Features

- 🌌 **Starry romantic intro** with a big glowing "Tap to begin 💖" button
- 💬 **8 headline languages, one at a time, BIG**: English, French, Spanish, Japanese, Korean, Arabic, Gujarati and Hindi. Each word is built from ~2,400 glowing particles that flow from the previous word, then the real text glows in with a shimmer sweep (right-to-left for Arabic), with the language name and pronunciation underneath
- 🌪️ **Language storm**: 44 more languages pop in and fill the whole screen as a glowing word cloud, with a live "N / 52 languages" counter
- 🇮🇳 **15 Indian languages**: Hindi, Gujarati, Marathi, Tamil, Telugu, Kannada, Malayalam, Bengali, Punjabi, Odia, Assamese, Urdu, Sanskrit, Nepali, Konkani (+ Sinhala)
- 🌍 **World languages**: French, Spanish, Italian, German, Portuguese, Russian, Japanese, Korean, Chinese, Arabic, Turkish, Greek, Hebrew, Thai, Vietnamese, Indonesian, Swahili, Persian, Dutch, Polish, Swedish, Ukrainian, Filipino, Irish, Hawaiian, Latin, Norwegian, Finnish, Czech, Hungarian, Romanian, Malay, Zulu, Icelandic, Welsh
- ❤️ **"52 languages… one meaning"**, then all the words dissolve into sparks that fly into a **beating particle heart** with the pet name in the centre
- 🌹 **Heart → rose**: the heart becomes a glowing outline while a canvas rose grows: the stem rises, the leaves unfurl, and the petals unfold layer by layer, with a glow, sparkles and falling petals
- 💌 Final line: "*<name>*, in every language, my answer is you 🌹"
- 📲 **WhatsApp share** with a personalised `?name=` link
- ✍️ **Make one**: type a pet name (or tap a chip: my love, sweetheart, cutiee, baby, Jaan) and send or copy your own link
- 🎹 **Soft piano music** made live with the WebAudio API (no audio files), with an on/off toggle
- ↻ **Replay**
- 📱 Mobile-first and BIG: it fills the phone screen, the main words are 48px+, and the buttons are large. Tested at 390×844 and 360×640
- 🔤 Every script renders with Google Noto fonts (Devanagari, Gujarati, Tamil, Telugu, Kannada, Malayalam, Bengali, Gurmukhi, Oriya, Sinhala, Nastaliq Urdu, Naskh Arabic, Hebrew, Thai, JP, KR, SC). The font files are subset to only the letters used, so they load fast and show no tofu boxes

## 🔗 URL options

| Param | Example | What it does |
|---|---|---|
| `name` | `?name=Jaan` | The pet name in the heart and the final line (default: `my love`) |
| `demo` | `?demo=1` | Auto-plays the whole show (used for recording) |

## 🛠️ Tech

Plain **HTML + CSS + JavaScript + Canvas 2D**, with no libraries.
- Text → particles: each word is drawn to an offscreen canvas, and its pixels are sampled as particle targets
- Heart: the parametric curve `x = 16 sin³t, y = 13 cos t − 5 cos 2t − 2 cos 3t − cos 4t`
- Rose: procedural Bézier petals plus spiralling cupped crescents, with radial gradients and shadows
- A deterministic timeline drives every scene, so the animation is smooth and replayable

## 🚀 Run it

Open `index.html` in a browser (or serve the folder). That's it.

---
Made with ❤️ by **@hack.n.code** · Comment **LOVE** on the reel for more 💬
