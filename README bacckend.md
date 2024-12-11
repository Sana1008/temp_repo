## ABHIMANYU_MV
##  Table of Contents

- [ Overview](#-overview)
- [ Features](#-features)
- [ Project Structure](#-project-structure)
- [ Getting Started](#-getting-started)
  - [ Prerequisites](#-prerequisites)
  - [ Installation](#-installation)
  - [ Usage](#-usage)
- [ Contributing](#-contributing)
- [ License](#-license)

---

##  Overview

**This project is designed to verify the accuracy and relevance of titles using a combination of efficient algorithms, vector databases, and similarity checks. By integrating techniques such as cosine similarity, fuzzy matching, and Levenshtein distance, the system ensures that titles align closely with their associated content. The use of Redis for quick data access further enhances the system's performance and scalability.**

---

##  Features

1. Vector Database Integration
Utilizes vector databases (such as Redis) to store and retrieve embeddings efficiently for quick similarity searches.
2. Cosine Similarity Matching
Measures the similarity between title and content vectors to determine relevance by calculating cosine similarity scores.
3. Fuzzy Matching
Implements fuzzy string matching techniques to handle partial matches and identify titles with slight variations or typos.
4. Levenshtein Distance
Calculates the edit distance between strings to detect minor discrepancies, such as spelling errors or character swaps.
5. Combination Algorithm
Combines multiple similarity measures (cosine similarity, fuzzy matching, and Levenshtein distance) to improve accuracy and reliability of title verification.
6. Similarity Check
Performs a comprehensive similarity check to provide a confidence score for each title-to-content comparison.
7. Fast and Scalable
Utilizes Redis for rapid data storage and retrieval, making the system capable of handling large datasets efficiently.

---

##  Project Structure

```sh
└── trade-saarthi-backend/
    ├── API_flow.md
    ├── ReadMe.md
    ├── app.py
    ├── config
    │   ├── RedisConfig.py
    │   ├── __init__.py
    │   └── database.py
    ├── dataFiles
    │   ├── RestrictedPrefix.csv
    │   ├── RestrictedSuffix.csv
    │   ├── RestrictedWords.csv
    │   ├── final.csv
    │   ├── titlesWithCommonPreSuff.csv
    │   ├── titlesWithNonCommon.csv
    │   └── word_counts.csv
    ├── functions
    │   ├── AddCacheToRedis.py
    │   ├── CsvOperations.py
    │   ├── RestrictedListsFunctions.py
    │   └── __init__.py
    ├── models
    │   └── TradeMarkModel.py
    ├── requirements.txt
    ├── routes
    │   ├── RedisRoutes.py
    │   ├── RestrictedPrefixSuffixRoutes.py
    │   ├── RestrictedWordsRoutes.py
    │   ├── TitleCombinationRoute.py
    │   ├── TradeMarkRoute.py
    │   └── __init__.py
    └── utils
        └── path_utils.py
```


##  Getting Started

###  Prerequisites

Before getting started with trade-saarthi-backend, ensure your runtime environment meets the following requirements:

- **Programming Language:** Python
- **Package Manager:** Pip


###  Installation

Install trade-saarthi-backend using one of the following methods:

**Build from source:**

1. Clone the trade-saarthi-backend repository:
```sh
❯ git clone https://github.com/Smart-India-Hackathon-24/trade-saarthi-backend
```

2. Navigate to the project directory:
```sh
❯ cd trade-saarthi-backend
```

3. Install the project dependencies:


**Using `pip`** &nbsp; [<img align="center" src="https://img.shields.io/badge/Pip-3776AB.svg?style={badge_style}&logo=pypi&logoColor=white" />](https://pypi.org/project/pip/)

```sh
❯ pip install -r requirements.txt
```

###  Usage
Run trade-saarthi-backend using the following command:
**Using `pip`** &nbsp; [<img align="center" src="https://img.shields.io/badge/Pip-3776AB.svg?style={badge_style}&logo=pypi&logoColor=white" />](https://pypi.org/project/pip/)

```sh
❯ python {entrypoint}
```

##  License

This project is protected under the [SELECT-A-LICENSE](https://choosealicense.com/licenses) License. For more details, refer to the [LICENSE](https://choosealicense.com/licenses/) file.

---
