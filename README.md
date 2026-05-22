# Introduction to AntConc — Taiwanese Hokkien Corpus Materials

Materials for a crash course introduction to corpus linguistics 
and AntConc using Taiwanese Hokkien data.

**Graduate Institute of Linguistics, NTU — May 2026**

---

## What is in this repository

| File | Description |
|------|-------------|
| `kong_seg.txt` | 200 segmented sentences containing 講 (kóng) |
| `sue_seg.txt` | 200 segmented sentences containing 說 (sueh) |
| `antconc_visual_guide.pdf` | Step-by-step guide to loading the corpora in AntConc |
| `presentation.pdf` | Slides from the May 2026 session |

---

## Before the session

1. Download AntConc from [laurenceanthony.net/software/antconc](https://www.laurenceanthony.net/software/antconc/). Choose the version for your operating system
2. Download `kong_seg.txt` and `sue_seg.txt` from this repository
3. Download the visual guide and follow the instructions to load the files

---

## Data source

Sentences collected from the 臺灣台語語料庫 (Taiwan Taigi Corpus),  
maintained by the National Academy for Educational Research (國家教育研究院).  
[https://tggl.naer.edu.tw](https://tggl.naer.edu.tw)

Word segmentation performed with [Jieba](https://github.com/fxsjy/jieba) 
with a custom dictionary for Taiwanese Hokkien vocabulary.

---

## Methodological note

Segmentation was performed with Jieba, which was trained on Mandarin and 
is not optimised for Taiwanese Hokkien. This has two practical consequences 
for the corpus materials:

- 說 (sueh) segments more consistently, as it behaves similarly in Mandarin
- 講 (kóng) segments less reliably — it is more characteristically Taiwanese 
  and Jieba sometimes merges it with adjacent elements (e.g. 人講, 伊講) 
  rather than treating it as a standalone token

Results from AntConc, particularly collocate analysis of 講, should be treated 
as exploratory rather than definitive. A custom Taiwanese segmenter would be 
needed for more robust analysis.
