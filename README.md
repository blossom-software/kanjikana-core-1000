# Kanjikana Core 1000

A manually curated list of 1,000 common Japanese words, in a suggested study order.

- Browse the list, with audio: [kanjikana.com/en/words/core-1000](https://kanjikana.com/en/words/core-1000)
- Study it with flashcards on Recall: [https://recall.cards/library/decks/gqzmapoaibnvbsktneyf](https://recall.cards/library/decks/gqzmapoaibnvbsktneyf)

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

1. The starting pool is all JLPT N5 and N4 words, plus the words JMdict tags as common (`ichi1`).
2. Words are ranked using their frequency in Netflix subtitles and in newspapers (JMdict `nf` tags), their rank in the iKnow Core 2000, and their JLPT level.
3. Particles, copulas and auxiliaries (は, が, です, ます…) are excluded from the list.
4. Words frequent in drama but not suited to a beginner are removed: insults, violence, crime vocabulary.
5. 19 closed sets enter together, by a fixed position: greetings, numbers, days of the week, family, colours... Some keep their own order (これ, それ, あれ).
6. Each word was checked by hand: 13 added, 31 removed, 16 kept against the ranking, 6 corrected (meaning, reading or spelling).
7. English meanings are generated with AI, limited to the senses a beginner needs. The other languages are translated from English with AI.

### Sources

Words were selected with the help of:

- the JLPT levels from [Jonathan Waller's JLPT Resources](https://www.tanos.co.uk/jlpt/), licensed under [CC BY](https://creativecommons.org/licenses/by/4.0/);
- the frequency tags of [JMdict](https://www.edrdg.org/wiki/index.php/JMdict-EDICT_Dictionary_Project), the property of the [Electronic Dictionary Research and Development Group](https://www.edrdg.org/), used in conformance with the Group's [licence](https://www.edrdg.org/edrdg/licence.html) (CC BY-SA 4.0);
- the word ranks of the [iKnow](https://iknow.jp/) Core 2000, used as one ranking signal. None of its content is reproduced.

## License

The Kanjikana Core 1000 is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) (full text in [LICENSE](LICENSE)). You can reuse it for any purpose, including commercial use, and adapt it, as long as you credit Kanjikana with a link to the list's page.

For example:

> Word list: [Kanjikana Core 1000](https://kanjikana.com/en/words/core-1000) by Kanjikana, licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).

The audio on the website is not part of this repository or of the license.

## Suggesting changes

Suggestions are welcome: a word that should be in the list or out of it, a better place in the order, a wrong reading, an unclear meaning or translation. Open an issue, or a pull request that edits the JSON file.

Accepted pull requests are merged, and the change is also applied to the list on Kanjikana, from which this file is generated.

By contributing, you agree to publish your contribution under CC BY 4.0.

## Versions

Each published update is tagged and listed in the [releases](../../releases), with the words that came in and went out.

- A **major** version changes the file's format.
- A **minor** version changes which words are in the list, or their order.
- A **patch** version fixes readings, meanings or translations.
