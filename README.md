# EduPulse-AI-
Intelligent Student Engagement &amp; Performance Monitoring System


EduPulse AI is an AI-powered full-stack web application designed to help educational institutions, training organizations, and bootcamps monitor student engagement, track learning progress, and identify at-risk students through intelligent analytics and personalized recommendations.

📌 Problem Statement
In educational environments, instructors often spend significant time manually tracking attendance, monitoring assignment/demo submissions, reviewing daily stand-up updates, and identifying students who require additional support.

As the number of students increases, it becomes increasingly difficult to detect disengagement early, resulting in:

Reduced student participation
Delayed interventions
Poor learning outcomes
Increased dropout risk

Existing solutions primarily focus on basic tracking and reporting, lacking intelligent insights that help educators make data-driven decisions.

Our Solution

EduPulse AI provides a centralized platform where students can manage their learning activities while instructors gain AI-powered insights into student engagement, performance trends, and risk prediction.

🎯 Objectives
Improve student engagement and learning outcomes.
Automate attendance and progress tracking.
Identify at-risk students using AI.
Generate personalized learning recommendations.
Provide actionable insights for instructors.
Reduce manual administrative effort.

✨ Key Features
🔐 Authentication & Authorization

Student
Register Account
Login
Secure JWT Authentication
Instructor
Login
Role-Based Dashboard Access
👨‍🎓 Student Dashboard

Students can:

✅ Mark Attendance
Daily attendance tracking
📝 Submit Daily Stand-up
Today's Work
Blockers
Tomorrow's Plan
💻 Submit Demo/Project Updates
Demo Name
GitHub Repository Link
Completion Status

📈 Track Progress
Attendance Percentage
Demo Completion Rate
Engagement Score
👨‍🏫 Instructor Dashboard

Instructors can:

📊 View Student Analytics
Attendance Trends
Demo Submission Statistics
Student Participation Reports

🚨 Monitor At-Risk Students
Low Engagement Detection
Missing Demo Identification
Attendance Deficiency Alerts


📄 Generate Reports
Daily Summary
Weekly Engagement Report


AI Recommendations
🤖 AI Features
1. Engagement Score Analysis

The system calculates a student's engagement score based on:

Attendance Consistency
Demo Completion
Stand-up Participation
Activity Frequency
Example Output
Engagement Score: 85/100
Status: Highly Engaged

2. Student Risk Prediction

AI categorizes students into:

🟢 Low Risk

Regular participation and good performance.

🟡 Medium Risk

Occasional absenteeism or pending demos.

🔴 High Risk

Low attendance and minimal activity.

3. Personalized Recommendations

Example:

Your attendance is excellent.

You currently have two pending demo submissions.

Focus on completing pending projects and
maintaining daily stand-up consistency.

4. Instructor AI Summary

Example:

Today's Summary:

• Total Students: 50
• Attendance Rate: 88%
• Pending Demos: 7
• High Risk Students: 3


🛠️ Tech Stack

Frontend
React.js
Tailwind CSS
React Router
Axios
Chart.js

Backend
Node.js
Express.js
Database
MongoDB Atlas


Authentication
JWT
bcrypt
AI Integration
Gemini API


Deployment
Vercel (Frontend)
Render (Backend)


Project Structure
EduPulse-AI/
│
├── frontend/
│   ├── src/
│   ├── pages/
│   ├── components/
│   └── services/
│
├── backend/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── middleware/
│   └── config/
│
├── docs/
│
├── README.md
│
└── package.json

🗄️ Database Schema
Users
{
  "_id": "",
  "name": "",
  "email": "",
  "password": "",
  "role": "student"
}
Attendance
{
  "_id": "",
  "studentId": "",
  "date": "",
  "status": "Present"
}
Standups
{
  "_id": "",
  "studentId": "",
  "todayTask": "",
  "blockers": "",
  "tomorrowPlan": ""
}
Demos
{
  "_id": "",
  "studentId": "",
  "demoName": "",
  "githubLink": "",
  "status": "Completed"
}

⚙️ Installation

Clone Repository
git clone https://github.com/yourusername/EduPulse-AI.git
cd EduPulse-AI
Backend Setup
cd backend
npm install

Create .env

PORT=5000
MONGODB_URI=your_mongodb_uri
JWT_SECRET=your_secret_key
GEMINI_API_KEY=your_api_key

Run Backend

npm start
Frontend Setup
cd frontend
npm install
npm run dev


🚀 Future Enhancements
AI Chat Assistant
n8n Workflow Automation


