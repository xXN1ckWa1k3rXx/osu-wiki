# Writing

*For the formatting standards, see: [Article style criteria/Formatting](../Formatting)*

*Notice: This article uses [RFC 2119](https://tools.ietf.org/html/rfc2119) to describe requirement levels.*

All English articles must use plain English.

## Language register

There are two language registers on the wiki: neutral and informal.

The neutral register is the default on the wiki.

The informal register is special and given to a small handful of articles. Some examples with this register include [FAQ](/wiki/FAQ) and [Help Centre](/wiki/Help_Centre).

For both registers, all rules in this part of the article style criteria must be followed. Exceptions for either register will be noted.

## British English

British English spelling variants must be used when there are conflicting spellings of English words. For example, use:

- `colour` instead of `color`
- `centre` instead of `center`
- `skilful` instead of `skillful`
- `analyse` instead of `analyze`

## Capitalisation

### Article names

Article names, when written in a paragraph, must not be capitalised, unless it is a link that points to the article or it is a proper noun (e.g. BanchoBot). The following is an example:

```markdown
If you want to know more about chat, refer to [Chat Console](/wiki/Chat_Console).
```

### Game modifiers

Game modifiers must have the word `mod` after the mod name to reduce ambiguity. These must be spelt as seen below (letter casing and spacing must match):

- `Easy` or `EZ`
- `No Fail` or `NF`
- `Half Time` or `HT`
- `Daycore` or `DC`
- `Hard Rock` or `HR`
- `Sudden Death` or `SD`
- `Perfect` or `PF`
- `Double Time` or `DT`
- `Nightcore` or `NC`
- `Fade In` or `FI`
- `Hidden` or `HD`
- `Flashlight` or `FL`
- `Relax` or `RL`
- `Autopilot` or `AP`
- `Target Practice` or `TP`
- `Spun Out` or `SO`
- `1K`, `2K`, `3K`, `4K`, `5K`, `6K`, `7K`, `8K`, and `9K`
  - If referring to the key mods collectively, use `xK`.
- `Co-op` or `CO`
- `Random` or `RD`
- `Mirror` or `MR`
- `Auto` or `AT`
- `Cinema` or `CM`
- `Touch Device` or `TD`
- `ScoreV2`

---

These game modifiers are no longer being used by osu!; however, if needed, these must be spelt as seen below (letter casing and spacing must match):

- `Fade Out`
- `No Video`
- `10K`
- `Taiko`

---

When writing out game modifiers for tournament articles, they must instead use upper camel case (omit the space and keep the letter casing as seen above).

### Gameplay elements

Gameplay elements must not be capitalised, unless they act as a title for a link that points to the article. The following is an example:

```markdown
In the osu! game mode, beatmaps are composed of three different gameplay elements: hit circles, sliders, and spinners.
```

### Language names

Language names must be capitalised. The following is an example:

```markdown
The `#spanish` chat channel is for those who speak Spanish.
```

### Proper nouns

Proper nouns must be capitalised. The following is an example:

```markdown
Dean Herbert (also known as peppy) created osu! back in 2007.
```

### Trademarks

*For rules regarding osu!, see: [osu!](#osu!)*

The following trademarks must be spelt as follows (letter casing must match):

- `Discord`
- `Facebook`
- `GitHub`
- `Google`
- `Reddit`
- `Skype`
- `Twitch`
- `Twitter`
- `YouTube`

Trademarks must not be followed by the trademark or registered trademark symbols.

## Date and time

### Date formatting

The formats found in [Wikipedia:Manual of Style/Dates and numbers § Formats](https://en.wikipedia.org/wiki/Wikipedia:Manual_of_Style/Dates_and_numbers#Formats) are all accepted date formats. Date formatting should be consistent throughout the entire article.

The `YYYY-MM-DD` date format should only be used in tables.

### Time formatting

Time formatting must be done using the following format:

```markdown
HH:MM TIMEZONE
```

Time is written in 24-hour format and any single digits must be prefixed with a zero. The timezone must be written immediately after the time and should be in UTC+0 for global events or in the timezone of the event for smaller events. Use `UTC` instead of `GMT`.

Bad examples:

```markdown
3:30 PM UTC
22:30 (UTC+7)
11:30
```

Good examples:

```markdown
15:30 UTC
22:30 UTC+7
11:30 UTC-4
```

`UTC` (without an offset) is implied to be `UTC+0`. Either one may be used, but usage must be consistent. UTC with an explicit 0 offset must use a plus symbol (`+`).

### Date and time formatting

When both date and time are used together, the date must be written first, followed by the time. The time must be in between parenthesis (`(` and `)`).

Bad examples:

```markdown
October 25, 2016 at 11:45 UTC
October 25, 2016 11:45 UTC
```

Good example:

```markdown
October 25, 2016 (11:45 UTC)
```

## Game modes

Game modes must be written as follows:

- `osu!`
- `osu!taiko`
- `osu!catch`
- `osu!mania`

Referring to the old game mode names (i.e. `Catch the Beat`, `Taiko`, and `Mania`) may be done if discussing said game mode's previous name.

## osu!

The name of the game, osu!, must not be capitalised or italicised. The osu! official branding must not use any spaces. Examples include:

- `osu!academy`
- `osu!api`
- `osu!catch`
- `osu!direct`
- `osu!keyboard`
- `osu!mania`
- `osu!store`
- `osu!stream`
- `osu!supporter`
- `osu!tablet`
- `osu!taiko`
- `osu!talk`
- `osu!tourney`

User titles that include `osu!` as part of the title name must be capitalised. Examples include:

- `osu! Alumni`
- `osu! Champion`

For all other terms, osu! must be treated as a [qualifying noun](https://en.wikipedia.org/wiki/Noun_adjunct). This means adding a space between osu! and the noun it modifies. Examples include:

- `osu! tournaments`
- `osu! community`
- `osu! chat`
- `osu! client`
- `osu! wiki`

---

`osu!` should not end a sentence. If it does, use a full stop (`.`) or question mark to get `osu!.` or `osu!?`.

`osu!` must not be followed by an exclamation mark (i.e. `osu!!`). The sentence must be rewritten to ensure that this will not occur.

## Terminology

These words must be spelt as follows (spacing must match):

- `approach circle`
- `game mode` (or `mode`)
- `game mod` (or `mod`)
- `gameplay`
- `hit burst`
- `hit circle`
- `hitsound`
- `in-game`
- `playstyle`
- `slider tick`
- `slider ball`
- `slider path`
- `Kudosu` (to be treated as a proper noun)

---

Some words have variants. Their preferred spelling must be used and is as follows:

- `creator` or `mapper` instead of `beatmapper`.
- `mapped` instead of `beatmapped`.
- `BN` or `Beatmap Nominators` when referring to the *Beatmap Nominators*.
- `sign in` instead of `log in`, unless the name of a button or link says otherwise.
- `sign out` instead of `log out`, unless the name of a button or link says otherwise.
- `register` instead of `sign up`, unless the name of a button or link says otherwise.

### Tournament articles

These words must be spelt as follows (spacing must match):

- `NoMods`, `NoMod`, or `NM`
- `FreeMods`, `FreeMod`, or `FM`
- `Tiebreaker`

## Abbreviations, acronyms, and initialisms

Abbreviations, acronyms, and initialisms must have their meaning written out upon their first occurrence. Other occurrences are optional, but done only when necessary. The following is an example:

```markdown
The NC (Nightcore) mod is similar to the DT (Double Time) mod because both NC and DT increase the speed of the music by 50%. However, NC will change the pitch of the music and add a clap and finish to the beat.
```

Abbreviations, acronyms, and initialisms must be capitalised, with exception. The following are examples:

- `CS` for `Circle Size`
- `AR` for `Approach Rate`
- `DT` for `Double Time`
- `SBS` for `Storyboard Scripting`

---

Use `e.g.` for "for example" and `i.e.` for "that is".

---

Abbreviations, acronyms, and initialisms should not be pluralised. The following is an example:

```markdown
Avoid:  BNs can nominate your beatmap.

Prefer: Beatmap Nominators can nominate your beatmap.
```

## Perspective

`player`, `user`, `skinner`, `storyboarder`, and `creator` should be used when referring to the reader or another person. `they`, `them`, `their`, and `theirs` may be used when needed.

`you` and `your` should be avoided. `I` must not be used. `we`, `he` or `his`, and `she` or `her` must not be used (see above for other terms).

---

[Articles with informal registers](#language-register) may ignore this section; however, `I` in paragraphs should be avoided.

## Grammar and syntax

Articles should prefer using simpler [American grammar and syntax](https://www.thepunctuationguide.com/british-versus-american-style.html).

### Contractions

Contractions must not be used.

[Articles with informal registers](#language-register) may use contractions; however, usage should stay consistent throughout the entire article.

### Numbers

*For number formatting, see [Wikipedia's Manual of Style on Number formatting](https://en.wikipedia.org/wiki/Wikipedia:Manual_of_Style#Numbers)*

[Articles with informal registers](#language-register) may ignore this section; however, usage should stay consistent throughout the entire article.

### Semicolons

[Articles with informal registers](#language-register) should avoid using semicolons (`;`).

### Serial comma

The serial comma, also known as the Oxford or Harvard comma, must be used.

### Logical quotations

Refer to [Wikipedia's Manual of Style for logical quotations](https://en.wikipedia.org/wiki/Wikipedia:Manual_of_Style#Punctuation_inside_or_outside).

From Wikipedia's Manual of Style:

> Include terminal punctuation within the quotation marks only if it was present in the original material, and otherwise place it after the closing quotation mark. For the most part, this means treating periods and commas in the same way as question marks: keep them inside the quotation marks if they apply only to the quoted material and outside if they apply to the whole sentence.

## Pronunciation

Written pronunciation must use the [International Phonetic Alphabet](https://en.wikipedia.org/wiki/Help:IPA/English).
