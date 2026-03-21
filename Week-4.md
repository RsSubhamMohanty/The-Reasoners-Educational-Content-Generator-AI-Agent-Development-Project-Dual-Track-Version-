## 📌 Overview


This project is an AI-powered Study Assistant built using the Groq API and LangChain tools.

It helps students to:

        Generate quizzes
        Create flashcards
        Summarize study material

## 🚀 Features

✅ Quiz Generator

       - Automatically creates multiple-choice questions from study content
       
✅ Flashcards Generator

       - Converts study material into easy-to-learn Q&A flashcards
       
✅ Summary Generator

        - Produces short and clear bullet-point summaries

## ⚙️ Installation

Run the following commands in your environment:

       !pip install groq
       !pip install langchain-core
       !pip install langchain
       !pip install langchain-community

## 🔑 Setup

       from groq import Groq
       
       client = Groq(api_key="YOUR_API_KEY")

## 🧠 Core Functions

Agent Controller

<img width="768" height="312" alt="Screenshot 2026-03-21 145120" src="https://github.com/user-attachments/assets/3a8b506b-f555-464c-8587-b9ae91e639a4" />


## Flashcards Generator

<img width="1410" height="699" alt="Screenshot 2026-03-21 145044" src="https://github.com/user-attachments/assets/2d2f8c52-90d4-4128-a1e7-e18ef9aeaff2" />

## Summary Generator

<img width="1438" height="762" alt="Screenshot 2026-03-21 145027" src="https://github.com/user-attachments/assets/dea1f229-5ce4-4015-9344-583cc1d78da6" />

## Quiz Generator

<img width="1177" height="654" alt="Screenshot 2026-03-21 145112" src="https://github.com/user-attachments/assets/a7fcf00c-a312-47e1-8aac-992934216c73" />


## 📌 How It Works

     User provides study material (context)
     Selects a task (quiz / flashcards / summary)
     Agent processes the request
     Groq LLM generates the output




https://github.com/user-attachments/assets/d2dff19a-91db-4694-8e5d-c862473305ab


