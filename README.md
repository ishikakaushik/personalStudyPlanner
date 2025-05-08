📚 Personalized Study Planner

A Streamlit application that generates a detailed, customized study plan based on your course load, deadlines, and personal study preferences using the Cohere AI API.

Features

Dynamic Course & Deadline Entry: Add multiple courses with deadlines on the fly.

Personal Preferences: Specify your study habits (e.g., morning sessions, session length).

AI-Generated Study Plans: Leverage Cohere’s command-xlarge-nightly model to craft a structured study schedule.

Calendar View: See your deadlines in a weekly calendar format.

Summary View: Review your AI-generated study plan at a glance.

Prerequisites

Python 3.7 or later

A Cohere API key (sign up at https://cohere.ai)

Internet connection to call the Cohere API

Installation

Clone the repository

git clone https://github.com/your-username/study-planner.git
cd study-planner

Create and activate a virtual environment

python -m venv venv
source venv/bin/activate      # macOS/Linux
venv\\Scripts\\activate     # Windows

Install dependencies

pip install streamlit cohere pandas

Configuration

Set up Streamlit secrets

Create a file at .streamlit/secrets.toml with the following contents:

[cohere]
api_key = "YOUR_COHERE_API_KEY"

Verify

Ensure st.secrets["cohere"]["api_key"] is correctly loaded by the app.

Usage

Run the Streamlit app:

streamlit run app.py

Open the URL shown in your terminal (usually http://localhost:8501).

Click Add Course to start listing your courses and deadlines.

Enter your personal study preferences in the text area.

Click Generate Study Plan to view your calendar and AI-crafted study guide.
