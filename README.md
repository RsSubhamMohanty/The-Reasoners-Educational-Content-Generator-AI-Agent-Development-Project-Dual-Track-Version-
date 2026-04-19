# 🚀 The Reasoners: Educational Content Generator AI Agent Development Project (Dual Track Version)

An AI-powered educational tutor designed to transform study materials into smart learning resources. This application automatically generates **quizzes, flashcards, summaries, audio explanations, and interactive study tools** from uploaded content. It combines **Artificial Intelligence, educational technology, and content processing** to create a complete digital study companion that improves learning efficiency, personalization, and accessibility.

---

## 🌐 Live Demo

🔗 **Try the Application Here:**
https://aistudyassistant-phl9.onrender.com/

---

## 💻 Source Code Repository

📂 Full project source code is available here:

https://github.com/Dibyasha-Sahu/AIStudyAssistant.git

You can clone the repository and run the project locally on your system.

---

## 📌 Core Features

### 📂 Smart PDF Upload System

* Upload one or multiple PDF study materials
* Extract readable educational content automatically
* Supports academic notes, books, and study documents

### 🧠 AI Quiz Generator

* Automatically generate MCQs from selected topics
* User can choose number of questions
* Helps in self-assessment and revision

### 📘 Flashcard Review System

* Creates topic-based flashcards instantly
* Useful for quick memorization and active recall learning

### 📄 Summary Generator

* Converts long content into short and clear notes
* Saves time during exam preparation

### 🎧 Audio Learning Assistant

* Converts topic explanations into audio format
* Supports learning while multitasking

### 📊 Study Dashboard & Analytics

Tracks learning activity such as:

* Total study sessions
* Topics covered
* Daily / monthly progress
* Activity graph
* Study streak

### 📅 Study Planner

* Add study tasks with date and time
* Mark tasks as completed
* Manage learning schedule efficiently

### 📤 Export Functionality

* Download generated quizzes
* Save summaries
* Export study material outputs

---

# 🛠️ Technology Stack

| Component      | Technology |
| -------------- | ---------- |
| Frontend       | Streamlit  |
| Backend        | Python     |
| AI Model API   | Groq / LLM |
| Database       | SQLite     |
| PDF Processing | PyPDF2     |
| Charts         | Plotly     |
| Audio          | gTTS       |
| Data Handling  | Pandas     |

---

# ⚙️ System Requirements

Before running the project, install the following:

## 1️⃣ Python

* Python Version: **3.8 or above**
* Download from:

https://www.python.org/

---

## 2️⃣ Install Required Libraries

Run the following command in terminal:

```bash
pip install streamlit PyPDF2 groq gtts plotly pandas
```

---

## 3️⃣ API Key Setup

## Step 1: Create an Account

Visit the Groq developer platform:

https://console.groq.com/

Create a free account or sign in.


## Step 2: Generate API Key

After login:

Open Dashboard
Go to API Keys section
Click Create New Key
Copy the generated key

Example:

gsk_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx

⚠️ Copy it immediately and store it safely.

## Step 3: Install Groq Python Package

If not already installed, run:

pip install groq

Open the code and replace:

```python
client = Groq(api_key="your_api_key_here")
```

with your actual API key.

⚠️ Keep your API key private and never upload it publicly.

---

# ▶️ How to Run the Project Locally

## Step 1: Clone Repository

```bash
git clone https://github.com/Dibyasha-Sahu/AIStudyAssistant.git
```

## Step 2: Enter Project Folder

```bash
cd AIStudyAssistant
```

## Step 3: Run Streamlit App

```bash
streamlit run app.py
```

## Step 4: Open Browser

Streamlit will automatically run at:

```text
http://localhost:8501
```

---

# 📖 How to Use the Application

## Step 1: Upload Study Material

Upload one or more PDF files containing notes, syllabus, or study content.

## Step 2: Select Material

Choose the uploaded file from dropdown list.

## Step 3: Extract Topics

Click **Extract Topics** to detect important subjects/topics automatically.

## Step 4: Choose Topic

Select a topic from the generated list.

## Step 5: Select Learning Action

Choose any one:

* 🧠 Quiz
* 📘 Flashcards
* 📄 Summary
* 🎧 Audio

## Step 6: View Results

Generated content will appear instantly.

## Step 7: Download Output

Export quiz, summary, or notes if needed.

## Step 8: Use Dashboard

Track sessions, topics, progress graphs, and streak.

## Step 9: Use Study Planner

Add future study tasks and mark completed work.

---

# 📊 Database Used (SQLite)

SQLite is used as the internal lightweight database to store:

### History Table

Stores:

* Quiz generation history
* Flashcard usage
* Summary sessions
* Audio sessions
* Date/time activity logs

### Schedule Table

Stores:

* Topic name
* Study date
* Study time
* Task type
* Completion status

---

# ⚠️ Real Development Issues Faced & Solutions

## 1. PDF Text Extraction Problem

### Issue:

Some uploaded PDFs returned empty text.

### Cause:

Scanned or image-based PDFs.

### Solution:

Added validation checks and warning messages.

---

## 2. Streamlit UI Rendering Problem

### Issue:

Custom CSS caused black screen / broken layout.

### Cause:

Full-screen fixed overlays and CSS conflicts.

### Solution:

Removed unstable CSS and optimized UI layers.

---

## 3. Duplicate Button Key Error

### Issue:

`StreamlitDuplicateElementKey`

### Cause:

Multiple buttons used same key.

### Solution:

Assigned unique keys to each component.

---

## 4. Session State Resetting

### Issue:

Selections were lost after clicking buttons.

### Solution:

Managed values using `st.session_state`.

---

## 5. AI API Delay / Failure

### Issue:

Slow or failed responses.

### Solution:

* Added try–except handling
* Displayed clear error messages

---

## 6. Styling & Visibility Issues

### Issue:

White text on light boxes became invisible.

### Solution:

* Fixed CSS text colors
* Improved contrast ratios

---

## 7. Audio Generation Issue

### Issue:

Audio failed when content was empty.

### Solution:

Added content checks before generating speech.

---

# 🎯 Educational Purpose

This project is designed to:

* Improve learning productivity
* Provide AI-based personalized study tools
* Reduce manual note preparation time
* Increase engagement through interactive learning
* Support revision using multiple learning formats
* Improve accessibility with audio learning

---

# 📈 Final Project Outcome

Successfully developed a **production-ready AI Study Assistant** with:

* Smart automation
* Clean user interface
* Real-time AI content generation
* Educational productivity tools
* Modern responsive design

---

# 📢 Conclusion

AI Study Assistant demonstrates how Artificial Intelligence can transform traditional education into a smarter, faster, and more engaging experience. By combining automation, analytics, and personalized study tools, the system serves as a complete digital learning companion for modern students.
