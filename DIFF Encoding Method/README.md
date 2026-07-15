# Text Vectorization Techniques

## 1. One-Hot Encoding
One-Hot Encoding converts each unique word into a binary vector. Each word gets its own position in the vocabulary. The value is **1** for the corresponding word and **0** for all other positions.

**Example:**
- people → [0, 0, 0, 1, 0]
- movie → [0, 0, 1, 0, 0]

**Pros:**
- Simple and easy to understand.
- Works well for small vocabularies.

**Cons:**
- Creates large sparse vectors.
- Does not capture the relationship between words.

---

## 2. Bag of Words (BoW)
Bag of Words represents a document by counting how many times each word appears. It ignores the order of words and focuses only on word frequency.

**Example:**
"people watch movie" → people = 1, watch = 1, movie = 1

**Pros:**
- Easy to implement.
- Useful for text classification and sentiment analysis.

**Cons:**
- Ignores word order and context.
- Common words may dominate the representation.

---

## 3. TF-IDF (Term Frequency – Inverse Document Frequency)
TF-IDF measures how important a word is in a document compared to the entire collection of documents. Frequently used words across all documents receive lower importance, while unique words receive higher importance.

**Idea:**
- High score → Important word.
- Low score → Common word.

**Pros:**
- Highlights meaningful words.
- Reduces the impact of very common words.

**Cons:**
- Still ignores word order and context.
- Cannot understand the meaning of words.

---

## Summary

| Technique | Represents | Considers Frequency | Considers Importance | Keeps Word Order |
|-----------|------------|---------------------|----------------------|------------------|
| One-Hot Encoding | Binary vectors | ❌ | ❌ | ❌ |
| Bag of Words | Word counts | ✅ | ❌ | ❌ |
| TF-IDF | Weighted word scores | ✅ | ✅ | ❌ |

### Conclusion
- **One-Hot Encoding** represents words as binary vectors.
- **Bag of Words** represents documents using word counts.
- **TF-IDF** gives higher weight to important words and lower weight to common words, making it more informative than Bag of Words.   
