# CompilerSpell — Formal Language Spell Analyzer

> A compiler-theory-based spell and grammar analyzer that treats natural language as a formal language, applying **SDD**, **SLR(1)**, **CLR(1)**, and **LALR(1)** parsing techniques to detect and correct spelling errors.

---

## 📌 Overview

**CompilerSpell** is a browser-based application that bridges compiler design theory and natural language processing.

Instead of simple dictionary lookup, it models English text as a formal grammar and processes it through real compiler phases:

* Lexical Analysis
* Syntax-Directed Definition (SDD)
* LR Parsing (SLR, CLR, LALR)
* AST Visualization

This project demonstrates how compiler concepts can be applied to natural language.

---

## 🚀 Features

* 🔹 Multiple Parsing Techniques — SDD, SLR(1), CLR(1), LALR(1)
* 🔹 Custom Lexer / Tokenizer
* 🔹 Trie-Based Dictionary Lookup
* 🔹 Levenshtein Distance for corrections
* 🔹 Soundex Phonetic Matching
* 🔹 Attribute Grammar Evaluation
* 🔹 LR Parsing Tables & Parse Trace
* 🔹 AST (Parse Tree) Visualization
* 🔹 Grammar Rule Checker
* 🔹 Auto-Correct System
* 🔹 File Upload Support
* 🔹 Export Analysis Report
* 🔹 Zero Dependencies (Pure HTML, CSS, JS)

---

## 🖥️ How to Run

```bash
git clone https://github.com/your-username/compilerspell.git
cd compilerspell
open index.html
```

Or simply open `index.html` in any browser.

---

## 🧠 Compiler Phases

### 1. Lexical Analysis

Breaks input into tokens:

* WORD
* NUMBER
* PUNCT
* WS (whitespace)
* NL (newline)

---

### 2. Syntax-Directed Definition (SDD)

Grammar:

```
G = (N, Σ, P, S)

Document → Sentence+
Sentence → Word+ Punctuation
Word → CorrectWord | ErrorWord
```

Attributes computed:

* Accuracy
* Error count
* Suggestions
* Corrections

---

### 3. LR Parsing (SLR / CLR / LALR)

Supports:

* ACTION / GOTO tables
* FIRST / FOLLOW sets
* LR(0) item sets
* Parse trace simulation

---

### 4. Code Generation (Auto-Correct)

* Applies corrections automatically
* Preserves capitalization
* Maintains text structure

---

## 📂 Project Structure

```
compilerspell/
│
├── index.html
└── README.md
```

---

## ⚙️ Workflow

```
Input Text
   ↓
Lexer → Token Stream
   ↓
SDD → Attributes
   ↓
LR Parser → Tables + Trace
   ↓
Auto-Correct → Output
   ↓
AST → Visualization
```

---

## 🧩 Algorithms Used

* Trie (fast lookup)
* Levenshtein Distance (spell correction)
* Soundex (phonetic matching)
* LR Parsing Algorithms
* FIRST & FOLLOW computation

---

## 🛠️ Grammar Rules Checked

* Double spaces
* Punctuation spacing
* Duplicate words
* Lowercase "i"
* Sentence capitalization
* Double punctuation
* Article misuse (a/an)
* Missing commas

---

## 📋 Usage

1. Enter text or upload file
2. Choose parsing technique
3. Click **COMPILE**
4. View results:

   * Errors
   * Suggestions
   * Tokens
   * Corrected output
   * Parse tables
   * AST

---

## 🎓 Academic Concepts Covered

* Formal Grammar (G = N, Σ, P, S)
* Lexical Analysis
* Syntax-Directed Definitions
* LR Parsing (SLR, CLR, LALR)
* FIRST / FOLLOW Sets
* Parse Trees & AST




> *"Every sentence is a program. Every word is a token. Every error is a parse conflict."*
