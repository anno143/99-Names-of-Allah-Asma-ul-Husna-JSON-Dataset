# 99 Names of Allah (Asma ul Husna) — JSON Dataset

A clean, ready-to-use JSON dataset of the **99 Names of Allah (أسماء الله الحسنى)** with fully vocalized Arabic, transliteration, Quranic references, and meanings in **English, French and Urdu**.

> "And to Allah belong the best names, so invoke Him by them." — *Surah Al-A'raf, 7:180*

## Used in the Fajr App

This dataset powers the 99 Names section of **[Fajr: Prayer Alarm & Adhan](https://play.google.com/store/apps/details?id=com.alifanalytics.fajr_app)**, an Android app by [Alif Analytics](https://play.google.com/store/apps/details?id=com.alifanalytics.fajr_app).

<a href="https://play.google.com/store/apps/details?id=com.alifanalytics.fajr_app">
  <img alt="Get it on Google Play" src="https://play.google.com/intl/en_us/badges/static/images/badges/en_badge_web_generic.png" height="60">
</a>

## Features

- All 99 names with fully vocalized Arabic (with harakat)
- Scholarly transliteration (e.g. `Ar-Raḥmān`, `Al-Quddūs`)
- Quran references where the name or its root word appears (`surah:ayah`)
- English meaning + clear, short description
- French meaning + description
- **Urdu meaning and description (اردو)**
- Plain UTF-8 JSON — Arabic, Urdu and French text is stored as readable characters, not escaped sequences

## File

```
99_Names_Of_Allah.json
```

## Data Structure

```json
{
  "code": 200,
  "status": "OK",
  "data": [
    {
      "number": 1,
      "name": "ٱلرَّحْمَٰنُ",
      "transliteration": "Ar-Raḥmān",
      "found": "(1:3)(17:110)",
      "en": {
        "meaning": "The Most Merciful, The Entirely Merciful",
        "desc": "The One who wills goodness and mercy for all of His creation; His mercy encompasses everything."
      },
      "fr": {
        "meaning": "Le Tout-Miséricordieux",
        "desc": "Clément envers ses créatures. ..."
      },
      "ur": {
        "meaning": "نہایت رحم کرنے والا",
        "desc": "اپنی تمام مخلوق کے لیے بھلائی اور رحمت چاہنے والا؛ اس کی رحمت ہر چیز پر چھائی ہوئی ہے۔"
      }
    }
  ]
}
```

| Field | Type | Description |
|---|---|---|
| `number` | int | Position in the list (1–99) |
| `name` | string | Arabic name, fully vocalized |
| `transliteration` | string | Latin transliteration |
| `found` | string | Quran references for the name or its root word, format `(surah:ayah)` |
| `en.meaning` / `en.desc` | string | English meaning and description |
| `fr.meaning` / `fr.desc` | string | French meaning and description |
| `ur.meaning` / `ur.desc` | string | Urdu meaning and description |

## Usage

Direct link to the raw file:

```
https://raw.githubusercontent.com/anno143/99-Names-of-Allah-Asma-ul-Husna-JSON-Dataset/main/99_Names_Of_Allah.json
```


**JavaScript**

```js
const res = await fetch("https://raw.githubusercontent.com/anno143/99-Names-of-Allah-Asma-ul-Husna-JSON-Dataset/main/99_Names_Of_Allah.json");
const { data } = await res.json();
console.log(data[0].name, data[0].ur.meaning);
```

**Python**

```python
import json

with open("99_Names_Of_Allah.json", encoding="utf-8") as f:
    names = json.load(f)["data"]

for n in names:
    print(n["number"], n["transliteration"], "-", n["en"]["meaning"], "-", n["ur"]["meaning"])
```

**Dart / Flutter**

```dart
final jsonStr = await rootBundle.loadString('assets/99_Names_Of_Allah.json');
final List names = json.decode(jsonStr)['data'];
print(names.first['ur']['meaning']);
```

> Tip: Urdu and Arabic are right-to-left. Render them with RTL text direction and a font that supports Arabic script (e.g. Noto Nastaliq Urdu, Noto Naskh Arabic, Amiri).

## Changes from the Original Dataset

This repo builds on [KabDeveloper/99-Names-Of-Allah](https://github.com/KabDeveloper/99-Names-Of-Allah/blob/main/99_Names_Of_Allah.json). Changes made:

- Added `ur` (Urdu meanings) for all 99 names, sourced from the [Online Tasbih Counter Asma ul Husna PDF](https://onlinetasbihcounter.com/wp-content/uploads/2026/08/asma-ul-husna-99-names-of-allah.pdf)
- Added `ur.desc` (Urdu descriptions) for all 99 names
- Updated Arabic names to fully vocalized forms
- Updated transliterations to a consistent scholarly style
- Updated English meanings (`en.meaning`)
- Decoded double-escaped characters (e.g. `\u00e9` showing up literally in French text)
- Fixed #50 (Ash-Shahīd), where the English and French descriptions were swapped
- Fixed #39 (Al-Muqīt), where the French meaning contained a sentence instead of a title
- Tidied Quran reference formatting (e.g. `(4:15 8)` → `(4:158)`)
- Trimmed stray whitespace and stray `}` characters
- Fixed Arabic spelling of #80 (ٱلتَّوَّابُ) and #89 (ٱلْمُغْنِي)
- Used one style for ʿayn (ʿ) and hamza (ʾ) in transliterations, and doubled consonants (e.g. `Al-ʿAfuww`, `Al-Mudhill`)
- Corrected French meanings that were wrong or repeated (#20, #21, #59, #63, #64, #69, #71, #72, #78) and typos (#62, #85, #95)
- Rewrote all 99 English descriptions (`en.desc`) in clear, consistent English, matching the Urdu descriptions
- Checked every Quran reference against the Quran text ([Tanzil](https://tanzil.net)); replaced references that did not mention the name or its root (#22, #41, #57, #71, #77, #92) and added verses where the name itself appears (#23, #28, #94); references are sorted by surah
- Second review (see [REVIEW.md](REVIEW.md)): added verses where the name itself appears (#19, #34, #43, #48, #55, #60, #66, #87, #97 and others), replaced references that were not about Allah (#96, #98, #99), and fixed French mistranslations (#23 "L'Éleveur", #39, #45, #51, #82, #90), English spelling and meaning consistency (#8, #24, #45, #64, #68, #87), and the duplicate Urdu meaning of #29/#86

## A Note on the List

The number ninety-nine is established in Sahih al-Bukhari (6410) and Sahih Muslim (2677). The commonly printed enumerated list traces to Jami' at-Tirmidhi (3507), and other scholars have compiled slightly different lists. Meanings here are translations to aid understanding and are not a substitute for tafsir or scholarly explanation.

Every reference in `found` has been checked. Each verse contains the name itself or a word from the same root used for Allah's action (e.g. يَقْبِضُ for Al-Qābiḍ), with the exceptions noted below. Some names (e.g. Al-Qābiḍ, Al-Khāfiḍ, Al-Jalīl, Aṣ-Ṣabūr) do not occur word for word in the Quran and come from the hadith list, so their references point to the root. For three names there is no verse where Allah is the subject of the root, so their references carry the meaning instead: Al-Khāfiḍ (95:5), Al-Māniʿ (35:2, 67:21) and Aṣ-Ṣabūr (16:61, 35:45). [REVIEW.md](REVIEW.md) has a table showing, for each name, whether the name itself appears in the Quran, plus hadith references for the names known from the hadith.

## Contributing

Corrections are welcome, especially for translations. Please open an issue or a pull request with the name number, the field, and a source for the correction.

## Credits

- Base dataset (French text and original references): [KabDeveloper/99-Names-Of-Allah](https://github.com/KabDeveloper/99-Names-Of-Allah)
- Urdu meanings: [Asma ul Husna PDF — Online Tasbih Counter](https://onlinetasbihcounter.com/wp-content/uploads/2026/08/asma-ul-husna-99-names-of-allah.pdf)
- English and Urdu descriptions: written for this dataset by Alif Analytics, based on the common understanding of each name
- Quran text used to verify references: [Tanzil](https://tanzil.net)
- Compilation and updates: [Alif Analytics](https://play.google.com/store/apps/details?id=com.alifanalytics.fajr_app)

## License

Free to use in personal and commercial projects. Please keep a link back to this repository and to the original dataset.
