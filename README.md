# Arabic Text Cleaning & Normalization 

This project provides a robust preprocessing pipeline for cleaning Arabic text data, especially noisy or unstructured input such as Telegram messages. It uses Python regex and Unicode manipulation to normalize and sanitize messages for further natural language processing tasks.

##  Objectives

- Remove Arabic diacritics
- Remove elongation (Tatweel) characters
- Normalize Arabic/Western numerals
- Strip unwanted punctuation or symbols
- Preserve meaningful tokens like words, digits, and Telegram usernames (`@user`)

##  Features

-  Handles Arabic & English text
-  Converts Eastern Arabic numerals → Western (`٣٢١` → `321`)
-  Keeps important elements like `@usernames`, phone numbers, and Arabic words
-  Removes noise: emoji, decorations, redundant characters

##  Tech Stack

- Python
- Regular Expressions (`re`)
- `unicodedata`
- `pandas` for batch processing

##  Example Cleaning Steps

```text
Raw:
"ٓٓســ.ـكـِلـ.ــيـ.ـف  مــعـ.ـتــمد صــحـ.ـتــي ✅"

Cleaned:
"سكليف معتمد صحتي"
