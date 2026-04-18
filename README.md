# Auto-Complete-Engine1
**AutoCompleteEngine** is a Java console application that utilizes the **Trie (Prefix Tree)** data structure to provide intelligent prefix-based word suggestions. The project focuses on optimizing search latency and memory scalability.

## 📌 Project Objectives
To build a robust word search engine capable of processing large-scale datasets with minimal latency while ensuring data persistence through file-based storage.

## 🛠 Functional Requirements

### 1. Dictionary Management
* **Insert:** Add new words with an associated **weight** to prioritize results.
* **Delete:** Remove words from the system without breaking the structure of related word branches.
* **Bulk Load:** Batch import vocabulary from external data files (`.txt`, `.csv`).
* **Persistence:** Automatically save and load the Trie state to/from the disk to prevent data loss after application shutdown.

### 2. Search & Suggestion
* **Word Search:** Check existence of a specific word.
* **Prefix Search:** Find all words starting with a specific character sequence.
* **Top-K Ranking:** Return a list of the top $K$ suggestions with the highest weights (e.g., most popular terms).
* **Instant Feedback:** An interactive mode where suggestions appear in real-time as the user types.
* **Collect All Words:** Ultility function for review and debug

---

## ⚙️ Non-functional Requirements

### 1. Language Constraints
* **English Only:** The engine is optimized for the standard A-Z English alphabet (case-insensitive).
* **Basic ASCII:** No support for Unicode or special diacritics, keeping the Node structure simple and memory-efficient.

### 2. Performance & Reliability
* **Search Latency:** $O(L)$ time complexity for all primary operations (where $L$ is word length).
* **Stability:** Robust handling of basic console inputs and file I/O errors.

---

## 🧪 Quality Assurance (QA)

### 1. Testing Strategy
* **Unit Testing:** Comprehensive tests using **JUnit 5** for all Trie logic.
* **Edge Cases:** Handling of empty strings, non-alphabetic inputs, and very short/long words.
* **Code Coverage:** Target **> 90%** coverage for the Trie core using **JaCoCo**.

### 2. Performance Analysis
* **Benchmarking:** Accurate execution timing using **JMH** to verify $O(L)$ performance.
* **Big O Verification:** Ensuring that search time remains constant regardless of dictionary size growth.

---

## 🚀 How to Run
**COMMING SOON**
