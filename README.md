# jisho-dictionary-data

Prebuilt SQLite dictionary for [Jisho](https://github.com/simiriva95/jisho-desktop),
published as release assets. Nothing here is written by hand — the file is produced
by `pnpm data:build` in that repository.

Each release carries `dictionary.sqlite.gz`. The tag names the build date; the
`meta` table inside the database records the schema version and the version of
every source that went into it.

## Sources and licences

This database is a derived work of:

| Source | Licence |
| --- | --- |
| [JMdict/EDICT](https://www.edrdg.org/jmdict/j_jmdict.html) — words, readings, senses, English glosses | CC BY-SA 4.0, © Electronic Dictionary Research and Development Group |
| [KANJIDIC2](https://www.edrdg.org/wiki/index.php/KANJIDIC_Project) — kanji readings, meanings, stroke counts | CC BY-SA 4.0, © EDRDG |
| [RADKFILE](https://www.edrdg.org/krad/kradinf.html) — radical/kanji cross-reference | CC BY-SA 4.0, © EDRDG |
| [KanjiVG](https://kanjivg.tagaini.net/) — stroke order data by Ulrich Apel | CC BY-SA 3.0 |
| [Tatoeba](https://tatoeba.org) — example sentences | CC BY 2.0 FR |

The EDRDG files are used under the terms of the
[EDRDG licence](https://www.edrdg.org/edrdg/licence.html).

**This database is therefore distributed under CC BY-SA 4.0.** Share-alike applies:
if you redistribute it, modified or not, it stays under the same licence and the
attributions above must travel with it. The same attributions are also stored in the
`licence` table inside the database, so an application can show them offline.
