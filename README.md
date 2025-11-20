
# Bangla-Grammer (Bangla Grammar Resources)

A structured, developer-friendly collection of Bengali (Bangla) dictionary and grammar-adjacent data in JSON format — ideal for apps, websites, and NLP projects.

## 🎯 What this repository offers

This repository contains JSON-data files in Bengali, covering resources such as:

- সমার্থক শব্দ (synonyms)  
- বিপরীত শব্দ (antonyms)  
- এক কথায় প্রকাশ (one-word expressions)  
- দেশ-রাজধানী-মুদ্রা (country-capital-currency) mapping  
  …and more.

These datasets are designed to be easy to integrate for developers working on Bangla language tools, websites, mobile apps, and natural-language-processing projects.  
(As noted in the repo description.) :contentReference[oaicite:2]{index=2}

## ✅ Features

- Plain JSON format: easy to parse in JavaScript, Python, Java, etc.  
- Bengali language resources — targeted at Bangla speaking developers & applications.  
- Suitable for language-learning, dictionary apps, NLP pipelines, word games, etc.  
- Open format: you can adapt, extend, remix (see license section).

## 📂 Repository Contents

Here’s a listing of the main files/folders:

```

README.md
এককথায় প্রকাশ.json
দেশ রাজধানী মুদ্রা.json
বিপরীত শব্দ.json
সমার্থক শব্দ.json

````

Each JSON file contains a list or mapping of Bengali words/expressions and their related data.

## 🧮 How to use

### Example in JavaScript (Node.js)

```js
const fs = require('fs');

const synonyms = JSON.parse(fs.readFileSync('সমার্থক শব্দ.json', 'utf-8'));

// Example: get synonyms of a word
const word = 'ভালো';
if (synonyms[word]) {
  console.log(`${word} এর সমার্থক শব্দ হলো: ${synonyms[word].join(', ')}`);
} else {
  console.log(`${word} এর জন্য কোনো তথ্য নেই।`);
}
````

### Example in Python

```py
import json

with open('বিপরীত শব্দ.json', encoding='utf-8') as f:
    antonyms = json.load(f)

word = 'উপর'
if word in antonyms:
    print(f"{word} এর বিপরীত শব্দঃ {', '.join(antonyms[word])}")
else:
    print(f"{word} এর জন্য তথ্য নেই।")
```

You can integrate this data into websites, mobile apps (KaiOS/Android/iOS), quiz engines, NLP preprocessing systems, etc.

## 📌 Use Cases

* Bangla dictionary / thesaurus apps
* Word-games: synonyms/antonyms finders
* Educational platforms (e.g., vocabulary building)
* Natural-Language-Processing (NLP) tasks: e.g., synonym expansion, antonym detection
* Language-learning websites targeting Bangla speakers

## 🛠 Contribution

Contributions are welcome! If you’d like to help:

1. Fork the repository.
2. Create a new branch (`git checkout -b new-entry`).
3. Add or improve entries in the JSON files. Please ensure proper Bengali spelling, encoding (UTF-8), and consistent formatting.
4. Submit a Pull Request (PR) explaining your changes.
5. I will review and merge if quality is good.

### Guidelines

* Maintain UTF-8 encoding for all files.
* Avoid duplicates (check if the word already exists).
* Use proper Bengali spelling; consistency helps.
* For big additions, consider splitting into multiple PRs for review ease.

## 📄 License

This repository is open-source. You may use, modify and distribute the data, subject to the terms of the license.

*(You should specify the actual license e.g., MIT, Apache, CC-BY. If none yet, consider adding one.)*

## 🙋 About the Author & Contact

Author: Shifat Hossain
Repository: [https://github.com/shifat100/bangla-grammer](https://github.com/shifat100/bangla-grammer) ([GitHub][1])
Feel free to open issues or contact for questions/suggestions.

---

Thank you for using **Bangla-Grammer**! 🙏
Let’s build richer Bangla language tools together.



[1]: https://github.com/shifat100/bangla-grammer "GitHub - shifat100/bangla-grammer: This repository provides a structured and developer-friendly collection of Bangla (Bengali) dictionary data in JSON format. It includes সমার্থক শব্দ (synonyms), বিপরীত শব্দ (antonyms), and এক কথায় প্রকাশ (one-word expressions)—perfect for apps, websites, and NLP projects."
