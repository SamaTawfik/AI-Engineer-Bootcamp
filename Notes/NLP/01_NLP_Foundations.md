# 🧠 Natural Language Processing (NLP)

A beginner-friendly guide to **Natural Language Processing (NLP)** covering its fundamental concepts, processing stages, pipeline, applications, challenges, and commonly used libraries.

Whether you're just starting your AI journey or reviewing NLP concepts, this repository provides a clear and organized overview of the field.

---

# 📚 Table of Contents

- [Introduction](#-introduction)
- [What is NLP?](#-what-is-nlp)
- [Natural Language Understanding vs Natural Language Generation](#-natural-language-understanding-vs-natural-language-generation)
- [NLP Stages](#-nlp-stages)
- [Applications of NLP](#-applications-of-nlp)
- [Challenges in NLP](#-challenges-in-nlp)
- [NLP Pipeline](#-nlp-pipeline)
- [Popular NLP Libraries](#-popular-nlp-libraries)
- [Resources](#-resources)

---

# 📖 Introduction

Natural Language Processing (**NLP**) is one of the most important fields of Artificial Intelligence.

It enables computers to process, understand, interpret, and generate human language in a way that is both meaningful and useful.

NLP powers many applications we use daily, including:

- Chatbots
- Virtual Assistants
- Machine Translation
- Search Engines
- Text Summarization
- Question Answering
- Sentiment Analysis
- Speech Recognition

---

# 🧠 What is NLP?

**Natural Language Processing (NLP)** is a branch of Artificial Intelligence (AI) that enables computers to understand, interpret, analyze, and generate human language.

**It combines techniques from:**
- Artificial Intelligence
- Machine Learning
- Deep Learning
- Computational Linguistics
to allow machines to communicate with humans using natural language.

NLP consists of two major components:

## Natural Language Understanding (NLU)
Natural Language Understanding focuses on converting unstructured human language into structured representations that computers can understand and process.

---

## Natural Language Generation (NLG)
Natural Language Generation converts structured information into natural, human-readable language.

---

# ⚙️ NLP Stages
NLP typically processes text through several stages.

---

## 1️⃣ Lexical Analysis

Lexical analysis is the first stage of NLP.
It converts raw text into smaller meaningful units called **tokens**.
This stage prepares the text for later processing.

### Tokenization

Splits text into words or sentences.

**Example**
Input
```
I love Natural Language Processing.
```
Output
```
["I", "love", "Natural", "Language", "Processing", "."]
```
---

### Lemmatization

Converts words into their **dictionary (base) form** while considering context and part of speech.

Examples
| Original | Lemma |
|----------|-------|
| running | run |
| studies | study |
| better | good |

---

### Stemming

Reduces words to their root by removing prefixes or suffixes.
Unlike lemmatization, stemming may produce words that do not exist in the dictionary.

Examples
| Original | Stem |
|----------|------|
| studies | studi |
| playing | play |
| connected | connect |

---

### Stop Word Removal

Removes very common words that carry little semantic meaning.

Examples of stop words:
```
the
is
a
an
of
to
and
```
Removing stop words reduces noise and improves processing efficiency.

---

## 2️⃣ Syntactic Analysis (Parsing)

Syntactic analysis examines the grammatical structure of a sentence.
Its goal is to determine how words relate to one another according to the grammar rules of a language.

It helps identify:
- Subject
- Verb
- Object
- Phrase Structure
- Dependency Relationships

Example:
```
The cat chased the mouse.
```
---

## 3️⃣ Semantic Analysis

Semantic analysis focuses on understanding the meaning of text.
Unlike syntax, which focuses on grammar, semantic analysis focuses on *meaning*.

Its goals include:
- Understanding sentence meaning
- Resolving ambiguity
- Identifying relationships between words
- Capturing user intent

One important task is:

### Word Sense Disambiguation (WSD)
Determining the correct meaning of a word depending on its context.

Example
```
I deposited money in the bank.
```
↓
Bank = Financial Institution

```
The boat reached the bank.
```
↓
Bank = River Side

---

## 4️⃣ Discourse Integration

Discourse Integration connects multiple sentences together.
Instead of analyzing each sentence independently, it considers previous sentences to preserve context.

Example
```
Sara bought a laptop.

She loves it.
```
This stage is particularly important in:
- Chatbots
- Dialogue Systems
- Document Summarization
- Machine Translation

---

## 5️⃣ Pragmatic Analysis

Pragmatic Analysis is the *final stage* of NLP.
It focuses on understanding the intended meaning rather than the literal meaning.

It considers:
**
- Context
- Speaker's intention
- Background knowledge
- Real-world knowledge**

Example
```
Can you open the window?
```
Literal meaning:
A question about your ability.

Actual meaning:
A polite request to open the window.

Pragmatic analysis also helps detect:
- Sarcasm
- Humor
- Irony
- Indirect requests

---

## 📌 Summary of NLP Stages

| Stage | Purpose |
|--------|---------|
| Lexical Analysis | Break text into tokens |
| Syntactic Analysis | Understand grammar |
| Semantic Analysis | Understand meaning |
| Discourse Integration | Connect sentences together |
| Pragmatic Analysis | Understand speaker intention |

---

# 🚀 Applications of NLP

Natural Language Processing is used in many real-world applications across different industries.

<p align="center">
<img width="700" alt="Applications of NLP" src="https://github.com/user-attachments/assets/e0aa23d1-6a51-4edc-9118-a6fcc57f0f7b">
</p>

Some common NLP applications include:

- 🤖 Chatbots
- 💬 Virtual Assistants (Siri, Alexa, Google Assistant)
- 🌍 Machine Translation
- 📄 Text Summarization
- 😀 Sentiment Analysis
- ❓ Question Answering Systems
- 🔍 Search Engines
- 📰 News Categorization
- 🏷️ Text Classification
- 🛒 Recommendation Systems
- 📝 Spell Checking & Grammar Correction
- 📧 Spam Email Detection
- 🎙️ Speech Recognition
- 🧾 Information Extraction

---

# ⚠️ Challenges in NLP

Although NLP has made significant progress, understanding human language remains a difficult task.

---

## 1. Ambiguity
Many words and sentences have multiple meanings depending on the context.

### Lexical Ambiguity
A single word may have different meanings.

### Syntactic Ambiguity
A sentence may have more than one grammatical interpretation.

---

## 2. Language Variability
People use language differently depending on:
Region,Culture,Age,Social Media,Informal Conversations

Models trained only on formal text may struggle with informal language.

---

## 3. Idioms and Sarcasm
Many expressions cannot be understood literally.
Example:
```
Kick the bucket
```
means
```
To die
```
not literally kicking a bucket.

Sarcasm is also difficult.
Example:
```
Great! Another exam...
```
The literal meaning is positive.
The intended meaning is negative.

---

## 4. Context Understanding

The meaning of words often depends on previous sentences.
---

## 5. Data Quality & Quantity

Poor-quality or biased datasets produce poor NLP systems.

---

## 6. Multilingual Challenges

Some languages have very limited datasets (Low-Resource Languages), making NLP more difficult.

---

## 7. Real-Time Processing

Balancing speed and performance remains a major challenge.

---

# 🔄 NLP Pipeline

The following figure illustrates a typical NLP pipeline.

<p align="center">
<img width="750" alt="NLP Pipeline" src="https://github.com/user-attachments/assets/8119841c-40cb-4fe2-83c8-52ecac215c74">
</p>

---

## Step 1: Sentence Segmentation

Split a document into individual sentences.

---

## Step 2: Tokenization

Split each sentence into individual words or tokens.

---

## Step 3: Stemming

Reduce words to their root form.

---

## Step 4: Lemmatization

Reduce words to their dictionary form.
Unlike stemming, lemmatization considers context and part of speech.

---

## Step 5: Stop Word Removal

Remove words that add little semantic value.-

---

## Step 6: Dependency Parsing

Analyze grammatical relationships between words.

---

## Step 7: Part-of-Speech (POS) Tagging

Assign a grammatical category to each word.

Example
| Word | POS |
|------|------|
| NLP | Noun |
| is | Verb |
| Amazing | Adjective |

POS tagging is widely used in:
- Parsing
- Information Extraction
- Named Entity Recognition

---

## Step 8: Named Entity Recognition (NER)

Identify important entities inside text.

---

## Step 9: Chunking (Shallow Parsing)

Chunking, also known as **Shallow Parsing**, groups individual words into meaningful phrases (chunks) such as **Noun Phrases (NP)**, **Verb Phrases (VP)**, and **Prepositional Phrases (PP)**.
Unlike **Dependency Parsing**, chunking does not identify grammatical relationships between words. Instead, it simply identifies phrase boundaries, making text easier to analyze.

### Example
Sentence:

```text
The beautiful little girl is reading a book.
```

After **POS Tagging**:
| Word | POS Tag |
|------|---------|
| The | DT |
| beautiful | JJ |
| little | JJ |
| girl | NN |
| is | VBZ |
| reading | VBG |
| a | DT |
| book | NN |

After **Chunking**:
```text
[NP The beautiful little girl]
[VP is reading]
[NP a book]
```
> **Note:** Chunking identifies phrase boundaries, while Dependency Parsing identifies the grammatical relationships between words.

---

# 🛠️ Popular NLP Libraries

Some of the most widely used NLP libraries are:
| Library | Description |
|----------|-------------|
| NLTK | Educational NLP toolkit |
| spaCy | Industrial-strength NLP library |
| Hugging Face Transformers | Pre-trained Transformer models |
| Gensim | Topic Modeling & Word Embeddings |
| TextBlob | Simple NLP library for beginners |
| Stanford CoreNLP | Java-based NLP toolkit |
| Flair | Contextual NLP framework |
| fastText | Word embeddings by Meta |

---

## 🎯 Conclusion
Natural Language Processing enables computers to understand and generate human language.
It combines linguistics, machine learning, and deep learning to build intelligent systems capable of performing tasks such as translation, summarization, sentiment analysis, question answering, and conversational AI.
As Large Language Models (LLMs) continue to evolve, NLP has become one of the most important fields in Artificial Intelligence.

---

# 🧹 Text Preprocessing

## 📖 What is Text Preprocessing?

Text preprocessing is one of the most fundamental steps in any **Natural Language Processing (NLP)** pipeline.
It transforms **raw, unstructured text** into a clean, consistent, and structured format that can be effectively processed by machine learning and deep learning models.
Preprocessing removes or standardizes these elements, making the text easier for NLP models to understand.

---

# 🎯 Why Do We Use Text Preprocessing?

### 1. Noise Reduction

Remove unnecessary information that does not contribute to the meaning of the text.
Examples include:
- HTML tags
- URLs
- Emojis
- Special characters
- Extra whitespace

---

### 2. Text Normalization
Standardize different forms of text into a consistent representation.

For example:
```text
Apple
APPLE
apple
```
↓
```text
apple
```

---

### 3. Improve Model Performance

Cleaner text allows NLP models to:
- Learn faster
- Generalize better
- Produce more accurate predictions

---

### 4. Feature Extraction

Preprocessing helps preserve meaningful words while removing irrelevant information, allowing models to extract more useful features.

---

# 🔄 Text Preprocessing Pipeline

There is **no universal preprocessing pipeline**.

The order of preprocessing steps—and even whether to include certain steps—depends on:
- The NLP task
- The dataset
- The model being used

For example:
- Sentiment Analysis may remove stop words.
- Machine Translation usually keeps stop words.
- Transformer models often perform tokenization internally.

A common preprocessing pipeline is shown below.

```text
Raw Text
    │
    ▼
Text Cleaning
    │
    ▼
Lowercasing
    │
    ▼
Tokenization
    │
    ▼
Stop Word Removal
    │
    ▼
Normalization
    │
    ▼
Processed Text
```

---

# ⚙️ Step 1: Text Cleaning (Noise Removal)

The first preprocessing step is removing unwanted information that does not contribute to the meaning of the text.
Typical cleaning operations include:
- Removing HTML tags
- Removing URLs
- Removing email addresses
- Removing mentions (@username)
- Removing hashtags (if unnecessary)
- Removing emojis
- Removing special characters
- Removing extra spaces
- Removing unnecessary punctuation

Cleaning helps reduce noise and improves text quality before further processing.

---

# ⚙️ Step 2: Lowercasing

Most NLP applications convert all text into lowercase to ensure consistency.
same word would be treated as multiple different words.

- Reduces vocabulary size
- Improves consistency
- Simplifies text analysis
> **Note:** Lowercasing is not always recommended. Tasks such as **Named Entity Recognition (NER)** often preserve capitalization because uppercase letters provide useful information.

## Code: 
```code
 # 1. Convert text to lowercase
    text = text.lower()

    # 2. Remove HTML tags
    text = re.sub(r'<[^>]+>', '', text)

    # 3. Remove URLs
    text = re.sub(r'https?://\S+|www\.\S+', '', text)

    # 4. Remove email addresses
    text = re.sub(r'\S+@\S+', '', text)

    # 5. Remove mentions (@username)
    text = re.sub(r'@\w+', '', text)

    # 6. Remove hashtag symbol but keep the word
    # Example: "#AI" -> "AI"
    text = re.sub(r'#', '', text)

    # 7. Remove emojis and non-ASCII characters
    text = text.encode("ascii", "ignore").decode("ascii")

    # 8. Remove punctuation
    text = text.translate(str.maketrans('', '', string.punctuation))

    # 9. Remove numbers
    text = re.sub(r'\d+', '', text)

    # 10. Remove extra whitespace, tabs, and newlines
    text = re.sub(r'\s+', ' ', text).strip()
```
---

# ⚙️ Step 3: Tokenization

Tokenization is the process of splitting text into smaller units called **tokens**.

Tokens can represent:

- Words
- Sentences
- Characters
- Subwords

It is one of the most important preprocessing steps because almost every NLP model expects tokenized input.

### Example

Input

```text
I love NLP.
```

Output

```text
["I", "love", "NLP", "."]
```

### Types of Tokenization

### Word Tokenization

```text
I love AI
```

↓

```text
["I", "love", "AI"]
```

---

### Sentence Tokenization

```text
Hello.

How are you?
```

↓

```text
Sentence 1

Sentence 2
```

---

### Subword Tokenization

Modern Transformer models (such as BERT and GPT) split unknown words into smaller meaningful units.

Example

```text
unbelievable
```

↓

```text
["un", "believ", "able"]
```

Subword tokenization is widely used because it can handle unseen words more effectively.

---

# ⚙️ Step 4: Stop Word Removal

Stop words are very common words in a language that usually carry little semantic meaning.

Examples include:

```text
the
is
a
an
of
to
and
in
on
at
```

Removing stop words helps the model focus on the most informative words in a sentence.

### Example

Input

```text
The cat is sitting on the table.
```

Output

```text
cat sitting table
```

### Advantages

- Reduces noise
- Reduces vocabulary size
- Improves computational efficiency
- Highlights meaningful words

> **Note:** Stop word removal is **task-dependent**. Some NLP tasks, such as **Machine Translation**, **Text Summarization**, and **Question Answering**, often benefit from keeping stop words because they contribute to sentence meaning and grammar.

---

# ⚙️ Step 5: Normalization

Normalization converts different forms of words into a consistent representation.

This helps reduce vocabulary size and ensures that words with the same meaning are treated as a single term.

The two most common normalization techniques are **Stemming** and **Lemmatization**.

---

## 🌱 Stemming

Stemming removes prefixes or suffixes to produce a root form (called a *stem*).

It uses simple rule-based algorithms without considering grammar or context.

### Example

| Original Word | Stem |
|--------------|------|
| playing | play |
| studies | studi |
| connected | connect |
| running | run |

### Advantages

- Very fast
- Simple implementation
- Reduces vocabulary size

### Disadvantages

- May produce invalid dictionary words
- Ignores context and grammar
- Less accurate

---

## 📚 Lemmatization

Lemmatization reduces a word to its **dictionary (base) form**, known as the **lemma**.

Unlike stemming, it considers:

- Context
- Vocabulary
- Part of Speech (POS)

As a result, it produces meaningful dictionary words.

### Example

| Original Word | Lemma |
|--------------|-------|
| running | run |
| studies | study |
| better | good |
| mice | mouse |

### Advantages

- Produces valid dictionary words
- More accurate than stemming
- Preserves word meaning

### Disadvantages

- Slower than stemming
- Requires linguistic knowledge

---

# 🔍 Stemming vs. Lemmatization

| Feature | Stemming | Lemmatization |
|---------|----------|---------------|
| Speed | Fast | Slower |
| Accuracy | Lower | Higher |
| Uses Vocabulary | ❌ | ✅ |
| Considers Context | ❌ | ✅ |
| Produces Valid Words | ❌ | ✅ |

**Rule of thumb:**

- Use **Stemming** when speed is more important.
- Use **Lemmatization** when accuracy and preserving meaning are more important.

---

# 🛠️ Popular Python Libraries for Text Preprocessing

Fortunately, you don't need to implement preprocessing algorithms from scratch. Python provides several powerful NLP libraries.

---

## NLTK (Natural Language Toolkit)

One of the oldest and most popular NLP libraries.

It is excellent for learning NLP fundamentals and provides implementations for:

- Tokenization
- Stop Word Removal
- Stemming
- Lemmatization
- POS Tagging
- Named Entity Recognition

**Best for:** Learning and academic projects.

---

## spaCy

spaCy is a modern, industrial-strength NLP library designed for production applications.

Features include:

- High performance
- Built-in NLP pipelines
- Accurate lemmatization
- POS tagging
- Dependency parsing
- Named Entity Recognition

**Best for:** Real-world NLP applications.

---

## Hugging Face Tokenizers

Modern Transformer models require specialized tokenizers.

The Hugging Face Tokenizers library provides efficient implementations of:

- Byte Pair Encoding (BPE)
- WordPiece
- SentencePiece

It is widely used with models such as:

- BERT
- GPT
- RoBERTa
- T5
- LLaMA

**Best for:** Deep Learning and Large Language Models (LLMs).

---

# 💡 Best Practices

- Always understand your dataset before preprocessing.
- There is **no one-size-fits-all preprocessing pipeline**.
- Different NLP tasks require different preprocessing techniques.
- Avoid removing useful information unless necessary.
- Modern Transformer models often handle tokenization internally.

---

# 📌 Key Takeaways

- Text preprocessing prepares raw text for NLP models.
- The preprocessing pipeline depends on the task and dataset.
- Tokenization is one of the most essential preprocessing steps.
- Stemming is faster but less accurate than lemmatization.
- Lemmatization preserves the actual meaning of words.
- Popular preprocessing libraries include **NLTK**, **spaCy**, and **Hugging Face Tokenizers**.



