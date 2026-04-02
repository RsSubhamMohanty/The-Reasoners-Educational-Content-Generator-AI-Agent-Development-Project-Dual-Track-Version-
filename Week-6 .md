## 🎯 Goal of Week 6: Domain Specialization

In Week 6, the system evolves into a complete domain-specific learning assistant with features like analytics, scheduling, and smart recommendations.

---

## 🎯 Goal of Week 6
To transform the application into a smart and interactive learning platform by integrating:

- SQLite database for data management
- Topic-based quiz generation
- Study planner with scheduling
- Performance analytics
- AI-driven learning features

---

## ⚙️ Features

### 📄 AI-Based Content Generation
- Upload PDF files
- Extract content automatically
- Generate:
  - 📝 Quiz (MCQs)
  - 🧠 Flashcards
  - 📌 Summary
  - 🎧 Audio Explanation

---

### 🧠 Topic Detection
- Automatically detects topics from uploaded content
- Allows topic-wise learning
- Improves accuracy of AI-generated results

---

### 🗂️ Database Integration (SQLite)
- Stores user activity
- Tracks learning history
- Saves study schedules

Tables used:
- `history` → Stores Quiz, Summary, Flashcard activity
- `schedule` → Stores study planning data

---

### 📅 Study Planner
- Add study tasks with:
  - Topic
  - Date
  - Time
  - Task type (Read, Practice, Revise, Quiz)
- Helps in structured learning

---

### 📊 Performance Analytics
- Displays user activity using graphs
- Tracks usage of different features
- Helps analyze learning progress

---

### 🎬 YouTube Learning
- Provides topic-based video links
- Enhances understanding through visual learning

---

### 🤖 AI-Based Recommendations
- Generates content based on selected topic
- Improves learning experience using context

---

## 🏗️ Tech Stack

- Frontend: Streamlit  
- Backend: Python  
- AI Model: Groq (LLaMA 3.1)  
- Database: SQLite  
- Visualization: Matplotlib  
- Audio: gTTS  
- PDF Processing: PyPDF2  

---

## 🔄 Workflow

1. Upload PDF
2. Extract content
3. Detect topics
4. Select topic
5. Generate:
   - Quiz / Flashcards / Summary / Audio
6. Store activity in database
7. Plan study schedule
8. View analytics

---




https://github.com/user-attachments/assets/f33ad71f-04b2-4ce1-a9dc-1176224e9c73

