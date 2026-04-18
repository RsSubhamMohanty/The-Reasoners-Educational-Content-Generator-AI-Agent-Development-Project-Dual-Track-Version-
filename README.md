# The-Reasoners-Educational-Content-Generator-AI-Agent-Development-Project-Dual-Track-Version-
An AI-powered educational tutor that automatically creates quizzes, flashcards, audio summaries, and interactive materials from various content. It integrates ed-tech and content processing to build a comprehensive study companion, enhancing personalized learning and accessibility.

---

## 📌 Features

* 📂 Upload PDF study materials
* 🧠 Generate quizzes (MCQs)
* 📘 Create flashcards for revision
* 📄 Generate short summaries
* 🎧 Convert content to audio explanations
* 📊 Study dashboard (sessions, topics, streak, graph)
* 📅 Study planner with schedule management
* 📤 Export generated content

---

## 🛠️ Requirements

Before running the project, install the following:

### 1. Python

* Version: Python 3.8 or above
* Download: https://www.python.org/

---

### 2. Install Required Libraries

Run this command:

```bash
pip install streamlit PyPDF2 groq gtts plotly pandas
```

---

### 3. API Setup

This project uses an AI API (Groq/OpenAI).

Add your API key in the code:

```python
client = Groq(api_key="your_api_key_here")
```

⚠️ Keep your API key private.

---

## ⚙️ How to Run the Project

```bash
streamlit run app.py
```

Then open in browser:

```
http://localhost:8501
```

---

## 📖 How to Use

1. Upload PDF files
2. Select study material
3. Click **Extract Topics**
4. Choose a topic
5. Select an action:

   * Quiz
   * Flashcards
   * Summary
   * Audio
6. View generated content
7. Download results if needed
8. Use Study Planner to schedule tasks
9. Track progress in Dashboard

---

## 📊 Database Used

SQLite is used to store:

* Study history (quiz, summary, etc.)
* Study planner schedules
* Analytics data for dashboard

---

## ⚠️ Issues Faced During Development 

### 1. PDF Text Extraction Issue

* Some PDFs returned no text
* Cause: scanned/image-based PDFs
* Solution: Added validation and warning messages

---

### 2. Streamlit UI Rendering Issue

* Custom CSS caused layout break (black screen)
* Cause: full-screen fixed elements
* Solution: Removed unsafe CSS and simplified UI

---

### 3. Duplicate Button Key Error

* Error: `StreamlitDuplicateElementKey`
* Cause: same key used multiple times
* Solution: used unique keys for each button

---

### 4. Session State Issues

* Data was resetting on every click
* Solution: used `st.session_state` properly

---

### 5. API Delay / Failure

* AI responses sometimes slow or failed
* Solution:

  * Used try–except blocks
  * Added error messages

---

### 6. Styling Issues (Invisible Text)

* Text became invisible due to CSS conflicts
* Solution:

  * Fixed colors using CSS overrides
  * Improved contrast

---

### 7. Audio Generation Issue

* Audio failed when text was empty
* Solution:

  * Added condition checks before generating audio

---

## 🎯 Educational Purpose

This project is designed to:

* Improve student learning efficiency
* Provide interactive AI-based study tools
* Reduce manual effort in note-making
* Help students stay consistent with study plans

---

## 📢 Conclusion

AI Study Assistant demonstrates how artificial intelligence can enhance education by making learning smarter, faster, and more interactive.







  



