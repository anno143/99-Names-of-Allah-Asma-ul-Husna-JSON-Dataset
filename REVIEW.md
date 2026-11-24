# Translation, Description and Reference Review

This review checks all 99 entries of `99_Names_Of_Allah.json`: the Arabic, transliteration, the English, French and Urdu meanings and descriptions, and every Quran reference in `found`.

Every reference was checked by machine against the Quran text from [Tanzil](https://tanzil.net) (simple-clean), and the questionable ones were then read by hand. Hadith numbers follow the numbering used on [sunnah.com](https://sunnah.com).

## 1. Issues fixed in this change

### Quran references (`found`)

| # | Name | Problem | Change |
|---|---|---|---|
| 19 | Al-ʿAlīm | No reference had the name in its definite form | Added 2:32 (إنك أنت العليم الحكيم) |
| 29 | Al-ʿAdl | Only one reference | Added 16:90 (إن الله يأمر بالعدل) |
| 34 | Al-Ghafūr | No reference had the definite name | Added 85:14 (وهو الغفور الودود) |
| 43 | Ar-Raqīb | Missing a clear verse | Added 33:52 (وكان الله على كل شيء رقيبا) |
| 48 | Al-Majīd | Only one reference | Added 85:15 (ذو العرش المجيد) |
| 55 | Al-Waliyy | Missing the best-known verse | Added 2:257 (الله ولي الذين آمنوا) |
| 60 | Al-Muḥyī | The exact form appears twice; only one was listed | Added 41:39 (لمحيي الموتى) |
| 66 | Al-Wāḥid | The name itself (ٱلْوَاحِد) appears in 6 verses, none of which were listed | Added 12:39, 13:16 (الله الواحد القهار) |
| 87 | Al-Jāmiʿ | The name appears in 2 verses about Allah; only one was listed | Added 4:140 (إن الله جامع المنافقين والكافرين) |
| 90 | Al-Māniʿ | 67:21 uses a different root (أمسك), not م ن ع | Added 35:2 (وما يمسك فلا مرسل له). There is no Quran verse where Allah is the subject of م ن ع, so both references are by meaning |
| 96 | Al-Bāqī | 28:60 (وما عند الله خير وأبقى) describes what is *with* Allah, not Allah | Replaced with 20:73 (والله خير وأبقى) |
| 97 | Al-Wārith | Only one reference | Added 21:89 (وأنت خير الوارثين), 28:58 (وكنا نحن الوارثين) |
| 98 | Ar-Rashīd | 2:256 (قد تبين الرشد من الغي) is about guidance becoming clear, not about Allah | Replaced with 18:24 (عسى أن يهدين ربي لأقرب من هذا رشدا) |
| 99 | Aṣ-Ṣabūr | 2:153, 3:200 and 103:3 describe **human** patience only | Replaced with 16:61 and 35:45 (Allah delays punishment until an appointed time), kept 16:127. See the hadith in section 3 |

### English

| # | Field | Before | After | Why |
|---|---|---|---|---|
| 8 | meaning | The Honorable | The Honourable | The rest of the English uses British spelling (honour, judgement, fulfil) |
| 24 | meaning | The Bestower of Honor | The Bestower of Honour | The same field mixed "Honourer" and "Honor" |
| 45 | meaning | the Boundless | The Boundless | Capitalisation |
| 87 | meaning | the Uniter | The Uniter | Capitalisation |
| 64 | meaning | The Ever-Wealthy, The Self-Sufficient | The Finder, The Self-Sufficient | Al-Wājid comes from و ج د (to find). The Urdu (پانے والا) and the English description ("finds whatever He wills") already say "Finder"; the old meaning did not match them |
| 68 | meaning | The Self-Subsisting, … | The Eternal Refuge, … | "Self-Subsisting" is the standard meaning of #63 Al-Qayyūm; aṣ-Ṣamad is the One to whom all turn in need |

### Urdu

| # | Before | After | Why |
|---|---|---|---|
| 29 | انصاف کرنے والا | عادل، سراپا انصاف | Same meaning as #86 Al-Muqsiṭ; the two names now differ |

### French

| # | Field | Problem | Fix |
|---|---|---|---|
| 4 | desc | The description was only a title ("Le Sanctifié") | A full description that matches the English and Urdu |
| 8 | desc | "El-Aziz" | Al-ʿAzīz |
| 13 | desc | "l'arabe perdu" (lost Arabic) is not accurate | l'arabe ancien |
| 23 | meaning, desc | **"L'Éleveur" means a livestock breeder in French** | Celui qui élève |
| 32 | meaning | "Le Très Doux" was almost the same as #30 "Le Doux" | Le Longanime (the usual French for al-Ḥalīm) |
| 33 | desc | "Al-Adhīm" | Al-ʿAẓīm |
| 36 | desc | "tous ce qu'Il a créé" | tout ce qu'Il a créé |
| 39 | desc | The description said the word was "lost Arabic" and was about judging details. That does not match the meaning (Le Nourricier). Al-Muqīt is in the Quran (4:85) | Rewritten to match the meaning |
| 45 | desc | "Il a rempli tout vide" (He filled every void) suggests that Allah takes up space | Rewritten: His knowledge, mercy and generosity encompass everything |
| 51 | meaning | "Le Véridique" means "the truthful" | La Vérité |
| 72 | desc | Editorial note "(cf no 71)" left in the text | Removed |
| 81 | desc | "Est le vengeur": the description only repeated the name | Real description |
| 82 | desc | "écarte du péché" means "keeps away from sin", not "erases sin" | efface le péché |
| 86 | meaning | L'Equitable | L'Équitable |
| 90 | meaning, desc | "Le Défenseur" leaves out the "withholding" meaning. "Celui dont ils devront être préservés" says the creatures must be protected *from Allah* | Celui qui retient, Le Protecteur / "ce dont elle doit être préservée" |
| many | desc | No final full stop | Added |

### Transliteration

| # | Before | After |
|---|---|---|
| 85 | Dhū al-Jalāli wa-l-Ikrām | Dhū al-Jalāl wa-l-Ikrām. No other transliteration has a case ending |

## 2. Issues found but not changed (need a human or scholarly decision)

These are rewrites or judgement calls, not plain errors. They are listed so a reviewer can decide.

**French descriptions** (most come from the original dataset):

- **#1 / #2 Ar-Raḥmān / Ar-Raḥīm**: In the usual scholarly distinction, Ar-Raḥmān is mercy to all creation and Ar-Raḥīm is mercy shown especially to the believers. The English and Urdu follow this. The French #2 instead describes general mercy (rain sent even to sinners), which is the meaning of Ar-Raḥmān.
- **#6 Al-Muʾmin**: The description calls the name "mysterious even for Muslims" and lists the articles of faith. It never explains the name (the Giver of security and faith).
- **#12 Al-Bāriʾ**: "Celui qui lève Sa création…" leaves out the main meaning, creating without an earlier model, which the English and Urdu give.
- **#18 Al-Fattāḥ**: "Le Grand Juge" gives only one of the two meanings (the Opener and the Judge).
- **#55 Al-Waliyy, #79 Al-Barr, #85 Dhū al-Jalāl**: Long sentences that are hard to follow. #79 goes off topic into who is called Muslim and who is not.
- **#60 Al-Muḥyī**: "redonne vie aux corps … des anges". The Islamic texts do not describe angels as having bodies that die and are raised again.
- **#62 Al-Ḥayy**: A run-on sentence with a quotation from aṭ-Ṭaḥāwī that has no punctuation.
- **#71 / #72**: Both open with "exempt des caractéristiques des créatures et meilleur que toute créature", which has nothing to do with bringing forward or delaying.
- Transliteration in the French text does not match the `transliteration` field (e.g. "Ar-Rahmān", "Al-Mu'min", "Al-‘Alīm").

**Urdu meanings** (from the source PDF):

- **#76 Al-Bāṭin "پوشیدہ سے واقف"**: Gives only "Knower of the hidden". The name itself means "the Hidden" (الباطن), which the description already gives. "باطن، پوشیدہ" would fit better.
- **#82 Al-ʿAfuww "معاف کرنے والا"**: Close to #14 and #34. "درگزر کرنے والا، گناہ مٹانے والا" would show the sense of erasing sin.

**English**:

- **#91 Aḍ-Ḍārr "The Creator of Harm"**: Accurate, but many translations use "The Distresser" or pair the name with #92 ("The One who brings harm and benefit"), as the scholars recommend.

**Arabic**: #11 ٱلْخَٰلِقُ uses the Quranic dagger alif, while names of the same pattern (ٱلْقَابِضُ, ٱلْبَاسِطُ, ٱلْبَارِئُ) use a full alif. This is not wrong, but it is inconsistent.

**Shared references**: Some entries share the same references (#5–#10 → 59:23; #58/#59; #73–#76 → 57:3; #24/#25/#84 → 3:26; #41/#85 → 55:27, 55:78). This is correct, because these verses name several attributes together.

**README**: The README said every reference contains "the name itself or a word from the same root". That was not true for #22 (95:5), #90 and #99. The README has been updated to explain that these are meaning-based.

## 3. Where each name is mentioned

"The name itself" means the name, or its exact word form, is used for Allah in at least one listed verse. "Root / meaning only" means the name is known from the hadith list (Jāmiʿ at-Tirmidhī 3507) and the verses use a word from the same root. Where the table says "meaning-based", they carry the meaning. For these names, the hadith column gives a sahih or well-known narration that uses the name or its verb.

The count of 99 names comes from Ṣaḥīḥ al-Bukhārī 6410 and Ṣaḥīḥ Muslim 2677. The enumerated list comes from Jāmiʿ at-Tirmidhī 3507.

| # | Name | Mentioned in the Quran as | References (`found`) | Hadith |
|---|---|---|---|---|
| 1 | Ar-Raḥmān (ٱلرَّحْمَٰنُ) | the name itself | 1:3, 17:110 |  |
| 2 | Ar-Raḥīm (ٱلرَّحِيمُ) | the name itself | 2:163, 3:31, 4:100, 5:3 |  |
| 3 | Al-Malik (ٱلْمَلِكُ) | the name itself | 20:114, 23:116, 59:23, 62:1 |  |
| 4 | Al-Quddūs (ٱلْقُدُّوسُ) | the name itself | 59:23, 62:1 |  |
| 5 | As-Salām (ٱلسَّلَامُ) | the name itself | 59:23 | Muslim 591 (اللهم أنت السلام) |
| 6 | Al-Muʾmin (ٱلْمُؤْمِنُ) | the name itself | 59:23 |  |
| 7 | Al-Muhaymin (ٱلْمُهَيْمِنُ) | the name itself | 59:23 |  |
| 8 | Al-ʿAzīz (ٱلْعَزِيزُ) | the name itself | 3:6, 4:158, 9:40, 48:7 |  |
| 9 | Al-Jabbār (ٱلْجَبَّارُ) | the name itself | 59:23 |  |
| 10 | Al-Mutakabbir (ٱلْمُتَكَبِّرُ) | the name itself | 59:23 |  |
| 11 | Al-Khāliq (ٱلْخَٰلِقُ) | the name itself | 6:102, 13:16, 39:62, 40:62, 59:24 |  |
| 12 | Al-Bāriʾ (ٱلْبَارِئُ) | the name itself | 59:24 |  |
| 13 | Al-Muṣawwir (ٱلْمُصَوِّرُ) | the name itself | 59:24 |  |
| 14 | Al-Ghaffār (ٱلْغَفَّارُ) | the name itself | 20:82, 38:66, 39:5, 40:42, 71:10 |  |
| 15 | Al-Qahhār (ٱلْقَهَّارُ) | the name itself | 13:16, 14:48, 38:65, 39:4, 40:16 |  |
| 16 | Al-Wahhāb (ٱلْوَهَّابُ) | the name itself | 3:8, 38:9, 38:35 |  |
| 17 | Ar-Razzāq (ٱلرَّزَّاقُ) | the name itself | 51:58 |  |
| 18 | Al-Fattāḥ (ٱلْفَتَّاحُ) | the name itself | 34:26 |  |
| 19 | Al-ʿAlīm (ٱلْعَلِيمُ) | the name itself | 2:32, 2:158, 3:92, 4:35, 24:41, 33:40 |  |
| 20 | Al-Qābiḍ (ٱلْقَابِضُ) | root / meaning only | 2:245, 39:67 | Abu Dawud 3451, Tirmidhi 1314 |
| 21 | Al-Bāsiṭ (ٱلْبَاسِطُ) | root / meaning only | 2:245, 13:26 | Abu Dawud 3451, Tirmidhi 1314 |
| 22 | Al-Khāfiḍ (ٱلْخَافِضُ) | root / meaning only (meaning-based: 95:5) | 56:3, 95:5 | Muslim 179 (يخفض القسط ويرفعه) |
| 23 | Ar-Rāfiʿ (ٱلرَّافِعُ) | the name itself | 3:55, 6:83, 58:11 | Muslim 179 |
| 24 | Al-Muʿizz (ٱلْمُعِزُّ) | root / meaning only | 3:26 |  |
| 25 | Al-Mudhill (ٱلْمُذِلُّ) | root / meaning only | 3:26 |  |
| 26 | As-Samīʿ (ٱلسَّمِيعُ) | the name itself | 2:127, 2:256, 8:17, 49:1 |  |
| 27 | Al-Baṣīr (ٱلْبَصِيرُ) | the name itself | 4:58, 17:1, 42:11, 42:27 |  |
| 28 | Al-Ḥakam (ٱلْحَكَمُ) | the name itself | 6:114, 22:69 | Abu Dawud 4955 (إن الله هو الحكم) |
| 29 | Al-ʿAdl (ٱلْعَدْلُ) | root / meaning only | 6:115, 16:90 |  |
| 30 | Al-Laṭīf (ٱللَّطِيفُ) | the name itself | 6:103, 22:63, 31:16, 33:34 |  |
| 31 | Al-Khabīr (ٱلْخَبِيرُ) | the name itself | 6:18, 17:30, 49:13, 59:18 |  |
| 32 | Al-Ḥalīm (ٱلْحَلِيمُ) | the name itself | 2:235, 17:44, 22:59, 35:41 |  |
| 33 | Al-ʿAẓīm (ٱلْعَظِيمُ) | the name itself | 2:255, 42:4, 56:96 |  |
| 34 | Al-Ghafūr (ٱلْغَفُورُ) | the name itself | 2:173, 8:69, 16:110, 41:32, 85:14 |  |
| 35 | Ash-Shakūr (ٱلشَّكُورُ) | the name itself | 35:30, 35:34, 42:23, 64:17 |  |
| 36 | Al-ʿAliyy (ٱلْعَلِيُّ) | the name itself | 4:34, 31:30, 42:4, 42:51 |  |
| 37 | Al-Kabīr (ٱلْكَبِيرُ) | the name itself | 13:9, 22:62, 31:30 |  |
| 38 | Al-Ḥafīẓ (ٱلْحَفِيظُ) | the name itself | 11:57, 34:21, 42:6 |  |
| 39 | Al-Muqīt (ٱلْمُقِيتُ) | the name itself | 4:85 |  |
| 40 | Al-Ḥasīb (ٱلْحَسِيبُ) | the name itself | 4:6, 4:86, 33:39 |  |
| 41 | Al-Jalīl (ٱلْجَلِيلُ) | root / meaning only | 55:27, 55:78 |  |
| 42 | Al-Karīm (ٱلْكَرِيمُ) | the name itself | 27:40, 82:6 |  |
| 43 | Ar-Raqīb (ٱلرَّقِيبُ) | the name itself | 4:1, 5:117, 33:52 |  |
| 44 | Al-Mujīb (ٱلْمُجِيبُ) | the name itself | 11:61 |  |
| 45 | Al-Wāsiʿ (ٱلْوَاسِعُ) | the name itself | 2:268, 3:73, 5:54 |  |
| 46 | Al-Ḥakīm (ٱلْحَكِيمُ) | the name itself | 31:27, 46:2, 57:1, 66:2 |  |
| 47 | Al-Wadūd (ٱلْوَدُودُ) | the name itself | 11:90, 85:14 |  |
| 48 | Al-Majīd (ٱلْمَجِيدُ) | the name itself | 11:73, 85:15 |  |
| 49 | Al-Bāʿith (ٱلْبَاعِثُ) | root / meaning only | 22:7, 58:6 |  |
| 50 | Ash-Shahīd (ٱلشَّهِيدُ) | the name itself | 4:166, 22:17, 41:53, 48:28 |  |
| 51 | Al-Ḥaqq (ٱلْحَقُّ) | the name itself | 6:62, 22:6, 23:116, 24:25 |  |
| 52 | Al-Wakīl (ٱلْوَكِيلُ) | the name itself | 3:173, 4:171, 28:28, 73:9 |  |
| 53 | Al-Qawiyy (ٱلْقَوِيُّ) | the name itself | 22:40, 22:74, 42:19, 57:25 |  |
| 54 | Al-Matīn (ٱلْمَتِينُ) | the name itself | 51:58 |  |
| 55 | Al-Waliyy (ٱلْوَلِيُّ) | the name itself | 2:257, 4:45, 7:196, 42:28, 45:19 |  |
| 56 | Al-Ḥamīd (ٱلْحَمِيدُ) | the name itself | 14:8, 31:12, 31:26, 41:42 |  |
| 57 | Al-Muḥṣī (ٱلْمُحْصِي) | root / meaning only | 19:94, 36:12, 58:6, 72:28, 78:29 |  |
| 58 | Al-Mubdiʾ (ٱلْمُبْدِئُ) | root / meaning only | 10:34, 27:64, 29:19, 85:13 |  |
| 59 | Al-Muʿīd (ٱلْمُعِيدُ) | root / meaning only | 10:34, 27:64, 29:19, 85:13 |  |
| 60 | Al-Muḥyī (ٱلْمُحْيِي) | the name itself | 7:158, 15:23, 30:50, 41:39, 57:2 |  |
| 61 | Al-Mumīt (ٱلْمُمِيتُ) | root / meaning only | 3:156, 7:158, 15:23, 57:2 |  |
| 62 | Al-Ḥayy (ٱلْحَيُّ) | the name itself | 2:255, 3:2, 25:58, 40:65 |  |
| 63 | Al-Qayyūm (ٱلْقَيُّومُ) | the name itself | 2:255, 3:2, 20:111 |  |
| 64 | Al-Wājid (ٱلْوَاجِدُ) | root / meaning only | 38:44, 93:7 |  |
| 65 | Al-Mājid (ٱلْمَاجِدُ) | root / meaning only | 11:73, 85:15 |  |
| 66 | Al-Wāḥid (ٱلْوَاحِدُ) | the name itself | 2:163, 5:73, 9:31, 12:39, 13:16, 18:110 |  |
| 67 | Al-Aḥad (ٱلْأَحَدُ) | the name itself | 112:1 |  |
| 68 | Aṣ-Ṣamad (ٱلصَّمَدُ) | the name itself | 112:2 |  |
| 69 | Al-Qādir (ٱلْقَادِرُ) | the name itself | 6:65, 36:81, 46:33, 75:40 |  |
| 70 | Al-Muqtadir (ٱلْمُقْتَدِرُ) | the name itself | 18:45, 54:42, 54:55 |  |
| 71 | Al-Muqaddim (ٱلْمُقَدِّمُ) | root / meaning only | 16:61, 50:28 | Bukhari 1120, Muslim 771 (أنت المقدم وأنت المؤخر) |
| 72 | Al-Muʾakhkhir (ٱلْمُؤَخِّرُ) | root / meaning only | 14:42, 71:4 | Bukhari 1120, Muslim 771 |
| 73 | Al-Awwal (ٱلْأَوَّلُ) | the name itself | 57:3 |  |
| 74 | Al-Ākhir (ٱلْآخِرُ) | the name itself | 57:3 |  |
| 75 | Aẓ-Ẓāhir (ٱلظَّاهِرُ) | the name itself | 57:3 |  |
| 76 | Al-Bāṭin (ٱلْبَاطِنُ) | the name itself | 57:3 |  |
| 77 | Al-Wālī (ٱلْوَالِي) | the name itself | 13:11 |  |
| 78 | Al-Mutaʿālī (ٱلْمُتَعَالِي) | the name itself | 13:9 |  |
| 79 | Al-Barr (ٱلْبَرُّ) | the name itself | 52:28 |  |
| 80 | At-Tawwāb (ٱلتَّوَّابُ) | the name itself | 2:128, 4:64, 49:12, 110:3 |  |
| 81 | Al-Muntaqim (ٱلْمُنْتَقِمُ) | the name itself | 32:22, 43:41, 44:16 |  |
| 82 | Al-ʿAfuww (ٱلْعَفُوُّ) | the name itself | 4:99, 4:149, 22:60 |  |
| 83 | Ar-Raʾūf (ٱلرَّءُوفُ) | the name itself | 3:30, 9:117, 57:9, 59:10 |  |
| 84 | Mālik al-Mulk (مَالِكُ ٱلْمُلْكِ) | the name itself | 3:26 |  |
| 85 | Dhū al-Jalāl wa-l-Ikrām (ذُو ٱلْجَلَالِ وَٱلْإِكْرَامِ) | the name itself | 55:27, 55:78 |  |
| 86 | Al-Muqsiṭ (ٱلْمُقْسِطُ) | root / meaning only | 3:18, 7:29 |  |
| 87 | Al-Jāmiʿ (ٱلْجَامِعُ) | the name itself | 3:9, 4:140 |  |
| 88 | Al-Ghaniyy (ٱلْغَنِيُّ) | the name itself | 3:97, 39:7, 47:38, 57:24 |  |
| 89 | Al-Mughnī (ٱلْمُغْنِي) | root / meaning only | 9:28, 53:48 |  |
| 90 | Al-Māniʿ (ٱلْمَانِعُ) | root / meaning only (meaning-based: 35:2, 67:21) | 35:2, 67:21 | Bukhari 844, Muslim 593 (لا مانع لما أعطيت) |
| 91 | Aḍ-Ḍārr (ٱلضَّارُّ) | root / meaning only | 6:17 |  |
| 92 | An-Nāfiʿ (ٱلنَّافِعُ) | root / meaning only | 48:11 |  |
| 93 | An-Nūr (ٱلنُّورُ) | the name itself | 24:35 |  |
| 94 | Al-Hādī (ٱلْهَادِي) | the name itself | 22:54, 25:31 |  |
| 95 | Al-Badīʿ (ٱلْبَدِيعُ) | the name itself | 2:117, 6:101 |  |
| 96 | Al-Bāqī (ٱلْبَاقِي) | root / meaning only | 20:73, 55:27 |  |
| 97 | Al-Wārith (ٱلْوَارِثُ) | the name itself | 15:23, 21:89, 28:58 |  |
| 98 | Ar-Rashīd (ٱلرَّشِيدُ) | root / meaning only | 18:24, 72:10 |  |
| 99 | Aṣ-Ṣabūr (ٱلصَّبُورُ) | root / meaning only (meaning-based: 16:61, 16:127, 35:45) | 16:61, 16:127, 35:45 | Bukhari 6099, Muslim 2804 (ما أحد أصبر على أذى سمعه من الله) |
