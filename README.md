# Midadium - An Intelligent AI-Powered E-Learning Platform

<div align="center">

<!-- [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) -->
[![Backend: Node.js](https://img.shields.io/badge/Backend-Node.js-blue?logo=nodedotjs)](https://nodejs.org/)
[![Frontend: Flutter](https://img.shields.io/badge/Frontend-Flutter-blue?logo=flutter)](https://flutter.dev/)
[![Database: MongoDB](https://img.shields.io/badge/Database-MongoDB-blue?logo=mongodb)](https://www.mongodb.com/)

</div>

<p align="center">
  <br />
  <em>A full-stack, AI-driven e-learning platform designed to deliver a scalable, personalized, and deeply intelligent educational experience for both students and teachers.</em>
  <br />
</p>

This is the **overview** repo for the Midadium Educational Platform.

- 🔗 **Frontend** (Flutter UI):  
  https://github.com/leenimad/Midadium-Frontend

- 🔗 **Backend** (Node.js APIs):  
 https://github.com/leenimad/Midadium-Backend

<!-- 
    HIGHLY RECOMMENDED: Create a short GIF (using a tool like Giphy Capture or ScreenToGif) showcasing your app's main features and add it here.
    It dramatically increases engagement.
-->
<!-- 
<p align="center">
  <img src="path/to/your/demo.gif" alt="Midadium App Demo" width="800"/>
</p> 
-->

---

## 🚀 About The Project

Midadium is not just another learning management system. It was built from the ground up to solve the core challenges of modern online education: the lack of personalization and the immense manual effort required to create engaging content.

This project leverages a sophisticated, multi-stage AI engine to transform static video lessons into dynamic, interactive learning experiences. By integrating multiple specialized AI models, Midadium automates content creation, provides intelligent discovery tools, and offers data-driven evaluation assistance, creating a smarter ecosystem for everyone.

---

## ✨ Key Features

### Core Platform Features
- **Role-Based Authentication:** Secure JWT-based authentication for Students, Teachers, and Admins.
- **Course & Lesson Management:** Full CRUD functionality for courses and lessons, including video and PDF uploads.
- **Student Enrollment & Progress Tracking:** Detailed tracking of lesson completion, quiz scores, and worksheet submissions.
- **Real-Time Notifications:** Instant updates for students and teachers using **Socket.IO**.
- **Secure Payment Integration:** Seamless course and package purchasing powered by **Stripe**.

### 🧠 Intelligent AI Features
Midadium's power comes from its strategic AI integrations:

- **Automated Video-to-Text Pipeline:**
  - Uses **FFmpeg** to extract audio from video lessons.
  - Employs **AssemblyAI**'s Speech-to-Text model to generate highly accurate transcripts, which become the foundation for all subsequent AI features.

- **AI Content Generation (powered by Google Gemini):**
  - **Summaries:** Automatically generates concise summaries and key takeaways for any lesson.
  - **Flashcards:** Creates sets of key terms and definitions.
  - **Quizzes:** Generates interactive multiple-choice quizzes with answers.
  - **Worksheets:** Produces critical-thinking questions and guidelines.

- **AI Discovery & Personalization Engine (RAG Architecture):**
  - **Semantic Course Search:** Allows users to find courses using natural language queries (e.g., "I want to build a mobile app").
  - **Personalized Recommendations:** Suggests relevant courses based on a student's enrollment history and interests.
  - **AI-Generated Learning Roadmaps:** Creates structured, multi-phase learning paths to help students achieve their goals using the platform's course catalog.

- **AI Evaluation & Analytics Suite:**
  - **AI-Assisted Submission Rating:** Automatically grades student assignments against lesson content, providing a score and constructive feedback.
  - **AI Course Review Analysis:** Performs sentiment and thematic analysis on all student reviews to provide teachers with actionable insights on strengths and areas for improvement.

---

## 🛠️ Tech Stack & Architecture

This project uses a modern MERN-like stack with a Flutter frontend and a sophisticated AI backend.

| Category                | Technologies                                                                                  |
| ----------------------- | --------------------------------------------------------------------------------------------- |
| **Frontend**            | `Flutter`, `Dart`                                                                             |
| **Backend**             | `Node.js`, `Express.js`, `REST APIs`                                                          |
| **Database**            | `MongoDB`, `Mongoose`                                                                         |
| **AI / Machine Learning** | `Google Gemini API`, `AssemblyAI API`, **Retrieval-Augmented Generation (RAG)**               |
| **Core Infrastructure** | `JWT Authentication`, `bcrypt.js`, `Socket.IO` (Real-Time), `Stripe API` (Payments), `FFmpeg` |
| **DevOps & Tools**      | `Git`, `GitHub`, `Postman`, `VS Code`                                                         |

---

## ⚙️ Getting Started

To get a local copy up and running, follow these simple steps.

### Prerequisites

Make sure you have the following installed on your machine:
- [Node.js](https://nodejs.org/en/) (v16 or later)
- [Flutter SDK](https://flutter.dev/docs/get-started/install)
- [MongoDB](https://www.mongodb.com/try/download/community)
- [FFmpeg](https://ffmpeg.org/download.html) (Ensure it's accessible in your system's PATH)

### Installation & Setup

1.  **Clone the repository:**
    ```sh
    git clone https://github.com/[YOUR_GITHUB_USERNAME]/midadium.git
    cd midadium
    ```

2.  **Backend Setup:**
    ```sh
    cd backend
    npm install
    ```
    - Create a `.env` file in the `backend` directory by copying the example:
      ```sh
      cp .env.example .env
      ```
    - Open the `.env` file and add your secret keys and configuration:
      ```env
      MONGO_URI=your_mongodb_connection_string
      JWT_SECRET=your_jwt_secret_key
      GEMINI_API_KEY=your_google_gemini_api_key
      ASSEMBLY_AI_API_KEY=your_assemblyai_api_key
      STRIPE_SECRET_KEY=your_stripe_secret_key
      # Optional: Add FFMPEG_PATH if it's not in your system's PATH
      # FFMPEG_PATH=/path/to/your/ffmpeg/executable 
      ```

3.  **Frontend Setup:**
    ```sh
    cd ../frontend # Or your flutter project folder name
    flutter pub get
    ```
    - Make sure your Flutter code (e.g., in a `lib/config/constants.dart` file) is pointing to your local backend server address (e.g., `const String API_BASE_URL = "http://localhost:5000";`).

### Running the Application

1.  **Start the Backend Server:**
    - Navigate to the `backend` directory and run:
      ```sh
      npm run dev
      ```
    - The server should now be running on `http://localhost:5000` (or your configured port).

2.  **Run the Flutter App:**
    - Navigate to the `frontend` directory.
    - Select your target device (emulator, Chrome, or physical device).
    - Run the app:
      ```sh
      flutter run
      ```

---

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.

---

## 📬 Contact

[Leen Imad Batta] - [www.linkedin.com/in/leen-batta-697558343] - [leeni.batta@gmail.com]

Project Link: [https://github.com/leenimad/Midadium](https://github.com/leenimad/Midadium)