# Decibel locale tasks

Source: `locales/landing-phrases.json`. The local instrument name is correct: Sonomètre, шумомер, Fonometro, Dezibel-Messgerät, 分贝计, 騒音計. Keep it. Put `dB` in the title next to it. On ru and uk the Cyrillic form `дБ` is the right spelling. Do not "fix" it to Latin `dB`.

`шумовая экспозиция` is the noise-exposure term. Leave it.

The on-page product name comes from the App Store name the builder inserts. German store subtitle is `Schallpegel`. Russian store name stays `Decibel Meter: Уровень громкости` — that is the search phrase. Do not change it to `уровень звука`. The landing title stays `Шумомер и уровень звука в дБ`. Do not change the landing noun `Dezibel-Messgerät` or `шумомер`.

## Do once

1. Append ` | dB` to any `metaTitle` that has neither `dB` nor `дБ`. Do not append it twice.
2. fr-CA is 47 of 50 fields copied from fr. Keep `Sonomètre` and `dB`. Rewrite `metaDescription`, `heroTagline`, and `faqSubtitle` so the page is not the same document. Spain and Mexico are already different (`sonómetro` / `decibelios` vs `medidor de decibeles`). Leave that split.

## Per locale

| Locale | Key | Now | Write |
|---|---|---|---|
| hu | `metaTitle` | `Decibelmérő és hangerőszint` | `Decibelmérő \| dB` |
| hu | `metaDescription` | `Mérje a hangerőt` | `Mérjen hangnyomásszintet decibelben iPhone-on vagy Androidon. Valós idejű dB, NIOSH és OSHA módok, frekvenciaelemzés és zajterhelés. Ingyenes.` |
| hu | `metaKeywords` | `hangerőszint` | `hangnyomásszint` |
| th | `faq4A`, `feature5Desc` | `วัดปริมาณรังสีเสียง` | `วัดปริมาณเสียง`. `รังสี` is radiation. |
| ar | `feature4Desc` | `وs3 (3000 ملي ثانية)` | `وS (3000 ملي ثانية)`. That is the S time weighting. |
| de | store subtitle used as the on-page name | `Lautstärke Pegel` | `Schallpegel`. Title stays `Dezibel-Messgerät und Schallpegel` and gains `\| dB` if `dB` is absent. |
| ru | store name | `Decibel Meter: Уровень громкости` | Keep it. `громкость` is the query. Title `Шумомер и уровень звука в дБ` stays. |
| fr | title | `Sonomètre et niveau sonore en dB` | keep |
| fr-CA | `metaDescription` | same as fr | `Sonomètre pour iPhone et Android. Mesurez le niveau sonore en dB, avec les modes NIOSH et OSHA, pour le bruit au travail.` |
| es | title | `Sonómetro y nivel de sonido en dB` | keep |
| es-MX | title | `Medidor de decibeles y nivel de sonido` | `Medidor de decibeles y nivel de sonido en dB` |
| zh-Hans | `metaTitle` | `分贝计与声级测量` | `分贝计与声级测量 \| dB` |
| zh-Hant | `metaTitle` | `分貝計與聲級測量` | `分貝計與聲級測量 \| dB` |
| ja | `metaTitle` | `デシベル騒音計と音量レベル` | `デシベル騒音計 \| dB`. `音量` is volume. The noun `騒音計` stays. |
| ko | `metaTitle` | `데시벨 소음 측정기와 소리 크기` | `데시벨 소음 측정기 \| dB` |
| en | `metaTitle` | `Decibel Meter \| dB Sound Level` | keep the title. Add the word `decibel` to the H1. The H1 never says it. |

Every other locale follows the same title rule: local meter name, then `| dB` or `| дБ`. No other wording change unless the title calls the app a volume knob (`hangerő`, `Lautstärke`, `громкость`, `głośność`, `hlasitost`, `lydstyrke`, `ένταση`, `glasnoća`). If that word is the only noun, put the meter word back and keep dB.

Rebuild `hu/index.html`, `th/index.html`, and `ar/index.html`. Hungarian must not say `hangerő`. Thai must not say `รังสี`. Arabic must not say `s3`.
