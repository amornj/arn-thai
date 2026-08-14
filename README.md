# Arn Thai — High-Yield Thai Vocabulary

Thai→English vocabulary filtered from LEXITON dictionary (40,854 → 5,000 high-yield words).

## Source
- **Dictionary**: [LEXITRON](https://github.com/chameleonTK/thai-dictionary) (`telex.xml`) — 40,854 Thai→English entries
- **Frequency list**: [Phupha Thai Word Frequency](https://zenodo.org/records/18490474) — 61,577 words ranked by Common Crawl frequency

## Methodology
1. Parsed all 40,854 LEXITRON entries
2. Deduplicated by headword (33,059 unique words)
3. Cross-referenced with Thai word frequency corpus
4. Kept top 5,000 most frequent words that have English translations in LEXITRON
5. Result: **5,000 words (12.2% of original)** — high-yield, commonly used Thai vocabulary

## Data format
`thai_words.json` — array of objects:
```json
{
  "word": "กา",
  "pos": "N, V",
  "english": "crow; kettle; mark",
  "thai_def": "นกชนิด Corvus macrorhynchos...",
  "sample": "กาเป็นนกที่ฉลาด",
  "freq": 193460292
}
```

## Stats
- 69% have Thai definitions
- 91% have sample sentences
- Top POS: N (2,231), V (1,405), ADV (231), ADJ (176)