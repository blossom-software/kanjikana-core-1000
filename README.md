# Kanjikana Core 1000

A curated list of 1,000 common Japanese words, in a suggested study order, with their readings and meanings in nine languages.

- Browse the list, with audio: [kanjikana.com/en/words/core-1000](https://kanjikana.com/en/words/core-1000)
- Study it with flashcards: [Kanjikana Core 1000 on Recall](https://recall.cards/library/decks/gqzmapoaibnvbsktneyf)

## The file

Everything is in [`kanjikana-core-1000.json`](kanjikana-core-1000.json):

```json
{
  "name": "Kanjikana Core 1000",
  "version": "1.0.1",
  "license": "CC-BY-4.0",
  "url": "https://kanjikana.com/en/words/core-1000",
  "words": [
    {
      "rank": 1,
      "word": "はい",
      "reading": "はい",
      "meanings": {
        "en": "yes, okay, here",
        "de": "ja, okay, hier (beim Namensaufruf)",
        "es": "sí, de acuerdo, presente",
        "fr": "oui, d'accord, présent",
        "id": "ya, baik, hadir",
        "ko": "네, 좋아요, 네 (출석 대답)",
        "pt": "sim, certo, presente",
        "ru": "да, хорошо, здесь (на перекличке)",
        "vi": "vâng, được, có đây"
      }
    }
  ]
}
```

| Field | Content |
|---|---|
| `rank` | The word's place in the suggested study order, from 1 to 1000. |
| `word` | The word as it is usually written: in kanji when it is usually written in kanji, in kana otherwise (そば, しばらく). |
| `reading` | Its reading, in hiragana, or in katakana for words written in katakana. |
| `meanings` | Its meanings as comma-separated glosses, keyed by language: English (`en`), German (`de`), Spanish (`es`), French (`fr`), Indonesian (`id`), Korean (`ko`), Brazilian Portuguese (`pt`), Russian (`ru`) and Vietnamese (`vi`). |

## How the list was made

The list is meant to be the 1,000 words a beginner should learn first, in the order they will need them. That is not the same as the 1,000 most frequent words: subtitles rarely name a weekday, and the news is full of words a beginner does not need yet.

- **Candidates:** the JLPT N5 and N4 vocabulary and the words dictionaries mark as common.
- **Ranking:** how often a word is heard in film and TV subtitles, cross-checked with learner-oriented lists and the JLPT levels.
- **Curation:** closed sets enter together and in order (numbers, days of the week, family words, これ・それ・あれ). Words frequent on screen but not useful first (rough speech, police and courtroom vocabulary) are left out. Words were then reviewed one by one, added or removed, and their readings checked.
- **Meanings:** the English meanings keep only the senses a beginner needs, edited from dictionary definitions. The other languages are translated from the English, with AI assistance.

### Sources

Words were selected with the help of:

- the JLPT levels from [Jonathan Waller's JLPT Resources](https://www.tanos.co.uk/jlpt/), licensed under [CC BY](https://creativecommons.org/licenses/by/4.0/);
- the frequency tags of [JMdict](https://www.edrdg.org/wiki/index.php/JMdict-EDICT_Dictionary_Project), the property of the [Electronic Dictionary Research and Development Group](https://www.edrdg.org/), used in conformance with the Group's [licence](https://www.edrdg.org/edrdg/licence.html) (CC BY-SA 4.0).

## License

The Kanjikana Core 1000 is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) (full text in [LICENSE](LICENSE)). You can reuse it for any purpose, including commercial use, and adapt it, as long as you credit Kanjikana with a link to the list's page.

For example:

> Word list: [Kanjikana Core 1000](https://kanjikana.com/en/words/core-1000) by Kanjikana, licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).

The audio on the website is not part of this repository or of the license.

## Suggesting changes

Suggestions are welcome: a word that should be in the list or out of it, a better place in the order, a wrong reading, an unclear meaning or translation. Open an issue, or a pull request that edits the JSON file.

The file is generated from the list Kanjikana maintains, so a pull request is not merged as it is: accepted changes are applied to that list and published in the next version. Contributions are made under the same CC BY 4.0 license.

## Versions

Each published update is tagged and listed in the [releases](../../releases), with the words that came in and went out.

- A **major** version changes the file's format.
- A **minor** version changes which words are in the list, or their order.
- A **patch** version fixes readings, meanings or translations.
