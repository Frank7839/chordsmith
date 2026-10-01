# Chordsmith guide voice

The in-ear guide plays these 26 words on the beat. Make them once in ElevenLabs and Chordsmith does the rest: it trims the silence at the start of each word so it lands exactly on the beat.

## Settings in ElevenLabs

- **Model:** Eleven Multilingual v2. It supports the `<break>` pause tags below. Eleven v3 ignores them.
- **Voice:** calm, clear and a little clipped, like a stage manager. Avoid breathy or "storyteller" voices.
- **Stability:** about 75%, so every word sounds the same.
- **Similarity:** about 75%
- **Style:** 0
- **Speed:** 1.0
- **Speaker boost:** on

## Script: paste this as one generation

```
One. <break time="1.0s" /> Two. <break time="1.0s" /> Three. <break time="1.0s" /> Four. <break time="1.0s" />
Intro. <break time="1.0s" /> Verse. <break time="1.0s" /> Verse one. <break time="1.0s" /> Verse two. <break time="1.0s" /> Verse three. <break time="1.0s" /> Verse four. <break time="1.0s" />
Pre-chorus. <break time="1.0s" /> Chorus. <break time="1.0s" /> Bridge. <break time="1.0s" /> Solo. <break time="1.0s" /> Interlude. <break time="1.0s" /> Instrumental. <break time="1.0s" /> Tag. <break time="1.0s" /> Outro. <break time="1.0s" />
Build. <break time="1.0s" /> Down. <break time="1.0s" /> All in. <break time="1.0s" /> Big. <break time="1.0s" /> Hits. <break time="1.0s" /> Break. <break time="1.0s" /> Last time. <break time="1.0s" /> Key change.
```

Listen once before you download. Each word should be clearly separated, with nothing extra said between them. If a word comes out odd, regenerate.

## Getting it into Chordsmith

You can do one or both of these.

**A. Just your phone (to test):** In Chordsmith, go to **In-ear guide → Voice clips → Load one recording** and pick the downloaded MP3. The grid dots turn green once it's loaded.

**B. Everyone who uses the app:** Rename the file to `all.mp3` and upload it to the repo inside a folder called `voice`, so the path is `voice/all.mp3`.

## Re-doing single words

Generate just that word and name the file after it, for example `chorus.mp3`, `verse-2.mp3` or `all-in.mp3`. Then either load it with **Load separate files**, or upload it to `voice/`. A file in `voice/` replaces that word from `all.mp3` only when `all.mp3` is absent. A file loaded on the phone always wins.

## Clip names, in order

`1` `2` `3` `4` · `intro` `verse` `verse-1` `verse-2` `verse-3` `verse-4` · `pre-chorus` `chorus` `bridge` `solo` `interlude` `instrumental` `tag` `outro` · `build` `down` `all-in` `big` `hits` `break` `last-time` `key-change`

**Tip:** The voice says whatever is in the file. So a Hindi or Telugu set works too: record "Mukhda" into `chorus` and "Antara" into `verse`.
