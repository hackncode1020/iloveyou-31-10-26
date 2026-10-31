# A Rose Made of "I Love You" in 52 Languages 🌹❤️

**Live demo:** https://iloveyou-langs-hackncode.sites.tab.bot/
**Personalised:** https://iloveyou-langs-hackncode.sites.tab.bot/?name=Jaan

A slow, cinematic one-page love website made of **typographic word art**. "I love you" in **52 languages (50+)** flows onto the screen. The words pack themselves into a **heart made entirely of text**, with your love's pet name in the middle. Then every word flies into place to form a **rose made only of words**: red and pink petals in a spiral, and a green stem and leaves.

Day 5 of 100 · made by [@hack.n.code](https://www.instagram.com/hack.n.code/)

## ✨ Features

- 🌌 **Starry romantic intro** with the pet name and a big glowing "Tap to begin 💖" button
- ✨ **Flow-in**: all 52 phrases float onto the screen in their own scripts, glowing red, pink and gold, while a counter climbs to "in 52 languages"
- ❤️ **Text heart**: the words pack densely into a heart shape, with an outline of words around it. It beats softly, with the pet name in the centre
- 🌹 **Text rose**: every word flows to a new spot:
  - outer petals filled with words and outlined with brighter words
  - a spiral of cupped inner petals written along curves
  - a golden "I love you" in the centre of the bloom
  - a green stem and two leaves (with veins) made of words
- 🍃 Words drift down like falling petals, and a shimmer of light sweeps across the rose
- 💌 Final line: "*<name>*, in 52 languages, my answer is you 🌹"
- 📲 **WhatsApp share** with a personalised `?name=` link
- ✍️ **Make one**: type a pet name (or tap a chip: my love, sweetheart, cutiee, baby, Jaan) and send or copy your own link
- 🎹 **Soft piano music** made live with the WebAudio API (no audio files), with an on/off toggle
- ↻ **Replay**
- 📱 Mobile-first and BIG: it fills the phone screen with large buttons. Tested at 390×844 and 360×640, with no overflow and no console errors

## 🌍 The 52 languages

**Indian (15 + Sinhala):** Hindi, Gujarati, Marathi, Tamil, Telugu, Kannada, Malayalam, Bengali, Punjabi, Odia, Assamese, Urdu, Sanskrit, Nepali, Konkani, Sinhala

**World:** English, French, Spanish, Japanese, Korean, Arabic, Italian, German, Portuguese, Russian, Chinese, Turkish, Greek, Hebrew, Thai, Vietnamese, Indonesian, Swahili, Persian, Dutch, Polish, Swedish, Ukrainian, Filipino, Irish, Hawaiian, Latin, Norwegian, Finnish, Czech, Hungarian, Romanian, Malay, Zulu, Icelandic, Welsh

Every script renders with Google Noto fonts: Devanagari, Gujarati, Tamil, Telugu, Kannada, Malayalam, Bengali, Gurmukhi, Odia, Sinhala, Nastaliq Urdu, Naskh Arabic, Hebrew, Thai, JP, KR and SC. The font files are subset to only the letters used, so they load fast and show no tofu boxes.

## 🔗 URL options

| Param | Example | What it does |
|---|---|---|
| `name` | `?name=Jaan` | The pet name in the heart and the final line (default: `my love`) |
| `demo` | `?demo=1` | Auto-plays the whole show (used for recording) |

## 🛠️ How it works

Plain **HTML + CSS + JavaScript + Canvas 2D**, with no libraries.
- **Shape packing:** the heart and the rose's petals and leaves are `Path2D` masks. Rows of words are packed inside each mask, in the petal's own rotated frame, using `isPointInPath`
- **Text on a path:** petal outlines, the inner spiral, the stem and the leaf veins are polylines, and the words follow each curve, rotated to its tangent
- **Morphing:** each word is a token that moves from the flow-in, to the heart, to the rose with eased, curved paths. Where the phrase changes, it cross-fades mid-flight
- **Glow:** the text layer is blurred at a third of the size and added back, which is cheap enough for phones

## 🚀 Run it

Open `index.html` in a browser (or serve the folder). That's it.

---
Made with ❤️ by **@hack.n.code** · Comment **LOVE** on the reel for the code 💬
