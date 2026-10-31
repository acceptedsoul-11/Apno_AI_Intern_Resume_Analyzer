# ApnoAI
# Vercel link: https://sai-resumeanalyzer.vercel.app
# 🚀 AI Career Copilot – AI-Powered Resume Analyzer
# Note:Use your own API Key
# Screenshots are included below

An intelligent, AI-powered career assistance platform that helps job seekers improve their resumes, evaluate their compatibility with job descriptions, and prepare for interviews.

AI Career Copilot uses Google's Gemini AI to analyze resumes, identify missing skills and keywords, suggest improvements, refine resume content, and generate interview preparation questions — all through a simple, interactive web interface.

---

## 📌 Table of Contents

1. [Overview](#-overview)
2. [Problem Statement](#-problem-statement)
3. [Objectives](#-objectives)
4. [Features](#-features)
5. [Technology Stack](#-technology-stack)
6. [Application Workflow](#-application-workflow)
7. [Project Structure](#-project-structure)
8. [Getting Started](#-getting-started)
9. [How to Use](#-how-to-use)
10. [AI Integration](#-ai-integration)
11. [Data Storage](#-data-storage)
12. [PDF Export](#-pdf-export)
13. [Security Considerations](#-security-considerations)
14. [Limitations](#-limitations)
15. [Future Enhancements](#-future-enhancements)
16. [Contributing](#-contributing)
17. [License](#-license)

---

## 🌟 Overview

Finding a suitable job is not just about having a resume. Candidates must ensure that their resumes communicate relevant skills, experience, and achievements in a way that matches the requirements of a particular job.

AI Career Copilot addresses this challenge by providing an AI-based platform that evaluates a resume against a given job description.

The application provides:

- An ATS-style resume compatibility score.
- An AI-generated resume summary.
- Identification of strengths and relevant qualifications.
- Detection of missing skills and keywords.
- Actionable resume improvement suggestions.
- AI-powered resume refinement.
- Personalized interview preparation.
- Analysis history management.
- PDF export functionality.

The application is designed as a lightweight, browser-based tool with a single HTML file.

---

## 🎯 Problem Statement

Job seekers often struggle to determine whether their resumes adequately match the requirements of a job posting.

Common challenges include:

- Not knowing which keywords recruiters and applicant tracking systems may look for.
- Difficulty identifying missing technical and professional skills.
- Writing resumes that do not effectively highlight relevant experience.
- Lack of personalized feedback on resume content.
- Insufficient preparation for interviews based on a specific job description.
- Repeatedly modifying resumes without understanding what needs improvement.

Traditional resume review processes can be time-consuming and may not provide immediate, job-specific feedback.

**AI Career Copilot aims to simplify this process using generative AI.**

---

## 🎯 Objectives

The primary objectives of this project are:

1. Develop an AI-powered resume analysis platform.
2. Compare resume content against a target job description.
3. Generate an ATS-style compatibility score.
4. Identify relevant and missing keywords.
5. Provide actionable recommendations for improving resumes.
6. Generate refined resume content using AI.
7. Create interview questions based on the candidate's resume and target role.
8. Maintain a history of previous resume analyses.
9. Allow users to export analysis reports as PDF documents.
10. Provide a responsive and user-friendly interface.

---

## ✨ Features

### 1. 📊 ATS Resume Analysis

The core functionality of the application is its AI-powered resume analysis system.

Users can provide:
- Their existing resume.
- The job description for the position they are applying for.

The AI evaluates the resume in relation to the job description and generates a structured analysis.

<img width="1912" height="858" alt="image" src="https://github.com/user-attachments/assets/566e8f32-f1ef-4744-9366-c82c72b63ae1" />

**Analysis includes:**

| Component | Description |
|---|---|
| ATS Compatibility Score | An estimated compatibility score based on the resume and job description. |
| Resume Summary | A concise overview of the candidate's profile. |
| Strengths | Relevant skills, qualifications, and experience identified in the resume. |
| Missing Keywords | Relevant terms or skills that appear to be absent from the resume. |
| Improvement Suggestions | Recommendations to make the resume more relevant and effective. |

The results are presented through an organized dashboard.
<img width="1517" height="886" alt="Screenshot 2026-10-31 090144" src="https://github.com/user-attachments/assets/0eb617b5-4859-406d-adee-6c6bc5aae818" />
Analysis of 3 resumes

> Note: The ATS score is an AI-generated estimate, not an actual score from a company's applicant tracking system.

### 2. ✍️ AI Resume Refiner

The Resume Refiner helps users improve the wording and presentation of their existing resume content.
<img width="700" height="381" alt="Screenshot 2026-10-31 090623" src="https://github.com/user-attachments/assets/cbc81f90-0bf2-415b-bd0b-6a1b84ec9b76" />
<img width="1427" height="550" alt="Screenshot 2026-10-31 090604" src="https://github.com/user-attachments/assets/4bf471d7-7619-4832-89ba-37afb5b8f970" />

It uses the provided resume and job description to generate more relevant resume content.

It aims to:
- Improve sentence clarity.
- Strengthen professional language.
- Highlight relevant skills and experience.
- Improve the presentation of achievements.
- Align resume content more closely with the target position.

The generated content should always be reviewed by the candidate to ensure that it accurately represents their real experience and qualifications.

### 3. 🎤 AI Interview Preparation

Preparing for an interview requires understanding both the job requirements and the candidate's own experience.

The Interview Prep feature uses the resume and job description to generate relevant interview preparation material.

It can help candidates:
- Practice technical interview questions.
- Prepare for role-specific questions.
- Understand topics related to their listed skills.
- Prepare for questions about projects and experience.
- Identify areas that may require additional preparation.

This feature helps users prepare for interviews with context relevant to their target role.

### 4. 📚 Analysis History
<img width="1767" height="813" alt="Screenshot 2026-10-31 091030" src="https://github.com/user-attachments/assets/107cf8c6-ccdc-4fda-bdee-b4fe3d24ed31" />

The application includes a history feature that allows users to revisit previously generated resume analyses.

Users can:
- Save analysis results locally.
- View previous analyses.
- Reopen saved results.
- Delete individual history entries.

The history is maintained using browser `localStorage`.

This means the saved information remains available in the same browser unless the browser's site data is cleared or the user removes the entries.

### 5. 📄 PDF Export

Users can export their analysis results into PDF format.

The generated report can include:

- ATS compatibility score.
- Resume summary.
- Identified strengths.
- Missing keywords.
- Improvement suggestions.
- Resume refinement output, when available.
- Interview preparation output, when available.

PDF export makes it easier to save, review, and share the generated feedback.

### 6. 🎨 User Interface

The application uses a modern, responsive interface designed to keep the resume analysis process straightforward.

Interface highlights include:

- Vibrant purple and pink gradient styling.
- Clean dashboard layout.
- Organized content cards.
- Subtle hover effects and animations.
- Loading indicators during AI operations.
- Responsive layout for different screen sizes.
- Clear separation between analysis, refinement, and interview preparation.

---

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| HTML5 | Application structure and content. |
| CSS3 | Styling, layout, animations, and responsive design. |
| JavaScript | Application logic and user interactions. |
| Google Gemini API | AI-powered resume analysis, refinement, and interview preparation. |
| Browser Fetch API | Communication with the Gemini API. |
| LocalStorage | Saving analysis history in the browser. |
| jsPDF | Generating downloadable PDF reports. |

### Architecture

The application follows a lightweight client-side architecture.

- **Frontend:** HTML, CSS, and JavaScript.
- **AI Service:** Google Gemini API.
- **Local Persistence:** Browser localStorage.
- **PDF Generation:** jsPDF library.

No dedicated application server or database is required in the current implementation.

---

## 🔄 Application Workflow

The application follows this general workflow:

1. The user opens AI Career Copilot in a web browser.
2. The user enters their resume content.
3. The user pastes the target job description.
4. The application sends the information to the Gemini API.
5. Gemini processes the input and generates structured feedback.
6. The application displays the analysis results.
7. The user can refine their resume or generate interview preparation material.
8. The results can be saved in analysis history.
9. The user can export the generated report as a PDF.

### Workflow Diagram

```text
             START
               |
               v
       Open AI Career Copilot
               |
               v
       Enter Resume Content
               |
               v
       Enter Job Description
               |
               v
       Submit for AI Analysis
               |
               v
        Gemini API Request
               |
               v
        Process AI Response
               |
               v
        Display Analysis
               |
       +-------+--------+
       |       |        |
       v       v        v
    Refine   Interview  View
    Resume    Prep     Results
       |       |        |
       +-------+--------+
               |
               v
       Save Analysis History
               |
               v
          Export PDF
               |
               v
              END
```

---

## 📁 Project Structure

The current implementation is intentionally maintained as a single-file application.

```text
AI-Career-Copilot/
│
├── AI_Career_Copilot_With_History_PDF.html
│
└── README.md
```

### File Description

| File | Description |
|---|---|
| `AI_Career_Copilot_With_History_PDF.html` | Main application containing the HTML structure, CSS styling, and JavaScript functionality. |
| `README.md` | Project documentation and setup instructions. |

The application does not require separate CSS or JavaScript files.

---

## ⚙️ Getting Started

### Prerequisites

Before running the application, ensure that you have:

- A modern web browser such as Google Chrome, Microsoft Edge, or Firefox.
- An active internet connection.
- A Google Gemini API key.

### Step 1: Clone the Repository

```bash
git clone https://github.com/your-username/AI-Career-Copilot.git
```

Navigate to the project directory:

```bash
cd AI-Career-Copilot
```

### Step 2: Configure the Gemini API Key

The application uses the Google Gemini API for AI functionality.

1. Visit [Google AI Studio](https://aistudio.google.com/).
2. Generate an API key.
3. Open the main HTML file.
4. Locate the API key configuration in the JavaScript section.
5. Configure your API key as required by the application.

**Important:** Never publish a real API key in a public GitHub repository. A browser-based application exposes its API key to users. For a production deployment, move API calls to a secure backend and store the key in environment variables.

If the key has already been exposed, revoke it and generate a replacement.

### Step 3: Run the Application

Since the project is a standalone HTML application, no build process is required.

You can simply:

1. Open the project folder.
2. Locate the main HTML file.
3. Double-click the file.
4. Open it in your browser.

Alternatively, use the VS Code Live Server extension to serve the HTML file locally.

### Step 4: Start Using the Application

Once the application loads, enter a resume and a job description to begin analyzing your resume.

---

## 🧑‍💻 How to Use

### Step 1: Analyze Your Resume

- Open the application.
- Enter or paste your resume content.
- Paste the job description.
- Start the analysis.

### Step 2: Review the Results

Examine the generated:
- ATS compatibility score.
- Resume summary.
- Strengths.
- Missing keywords.
- Improvement suggestions.

### Step 3: Refine Your Resume

Use the Resume Refiner feature to generate improved resume content based on the target job description.

Review the output carefully before using it in an actual job application.

### Step 4: Prepare for Interviews

Open the Interview Prep feature to generate questions and preparation material relevant to the target role.

### Step 5: Save Your Results

Use the analysis history feature to revisit previous results.

### Step 6: Export Your Report

Use the PDF export functionality to download your analysis report.

---

## 🤖 AI Integration

Google Gemini is used as the generative AI engine for the application.

The application communicates with the Gemini API using JavaScript's Fetch API.

### AI Tasks

| AI Task | Input | Expected Output |
|---|---|---|
| Resume Analysis | Resume and job description | ATS-style score and detailed feedback. |
| Resume Refinement | Existing resume and job description | Improved resume content. |
| Interview Preparation | Resume and job description | Relevant interview preparation questions and guidance. |

### General API Workflow

```text
JavaScript Application
        |
        v
Prepare User Input
        |
        v
Construct Gemini API Request
        |
        v
Send HTTP Request
        |
        v
Google Gemini API
        |
        v
Receive Generated Response
        |
        v
Process Response
        |
        v
Display Results in UI
```

### Error Handling

The application includes retry handling for selected temporary API errors, including:

- HTTP 429 – Too Many Requests.
- HTTP 500 – Internal Server Error.
- HTTP 502 – Bad Gateway.
- HTTP 503 – Service Unavailable.
- HTTP 504 – Gateway Timeout.

Retry handling can help with temporary service issues, but it cannot resolve exhausted API quotas, invalid credentials, or persistent service outages.

---

## 💾 Data Storage

The current implementation uses browser `localStorage` to maintain analysis history.

### What Is Stored?

The application can store generated analysis information, including:

- Resume analysis results.
- ATS compatibility score.
- Resume summary.
- Strengths.
- Missing keywords.
- Improvement suggestions.
- Generated refinement and interview preparation content.

### Important Characteristics

- Data is stored locally in the user's browser.
- No cloud database is configured in the current version.
- History is associated with the browser and its local site storage.
- Clearing browser site data can remove saved history.
- History is not automatically synchronized between devices.

---

## 📄 PDF Export

PDF generation is implemented using the jsPDF library.

The application uses the library to convert generated analysis information into a downloadable report.

The PDF report is intended to provide a convenient record of the resume evaluation and related AI-generated recommendations.

The PDF library is loaded through a CDN, so an internet connection is required for that functionality.

---

## 🔐 Security Considerations

Security is particularly important because resumes may contain personal information such as:

- Full name.
- Email address.
- Phone number.
- Educational details.
- Employment history.
- Project information.

The current implementation is a client-side application.

### Important Security Notes

1. **API Key Exposure:** API keys embedded in frontend JavaScript can be viewed through browser developer tools. This approach is suitable only for controlled experimentation, not secure production deployment.

2. **Resume Privacy:** Resume content is transmitted to Google's Gemini API for processing. Users should avoid submitting sensitive information unnecessarily and review the provider's applicable privacy and data-handling terms.

3. **Local Storage:** Analysis history is stored in browser storage and may be accessible to anyone using the same browser profile.

4. **Third-Party Libraries:** The application depends on external services and libraries, including Gemini and jsPDF.

### Recommended Production Improvements

- Introduce a secure backend API.
- Store API keys in server-side environment variables.
- Add authentication and authorization.
- Implement secure session management.
- Provide user-controlled data deletion.
- Apply appropriate input validation.
- Review third-party data-processing requirements.

---

## ⚠️ Limitations

The current implementation has the following limitations:

1. ATS scores are AI-generated estimates and do not guarantee compatibility with real ATS platforms.
2. Analysis quality depends on the completeness and clarity of the resume and job description.
3. AI-generated suggestions may occasionally be inaccurate or irrelevant.
4. The application requires internet connectivity for Gemini API requests.
5. API usage may be restricted by quotas, rate limits, or service availability.
6. Analysis history is stored locally and is not synchronized across devices.
7. The application does not currently provide user authentication.
8. The application does not connect directly to job portals or recruitment platforms.
9. The current single-file architecture is convenient for development but is not ideal for a large-scale production system.

---

## 🚀 Future Enhancements

Several improvements can be introduced in future versions.

### 1. User Authentication
- User registration and login.
- Individual user profiles.
- Secure access to saved analyses.

### 2. Cloud-Based History
- Integrate MongoDB or another database.
- Store resume analyses securely.
- Synchronize history across devices.

### 3. Multiple Resume Formats
- Upload PDF resumes.
- Upload DOCX resumes.
- Extract text automatically.
- Support multiple resume versions.

### 4. Advanced ATS Analysis
- More detailed keyword matching.
- Section-wise resume evaluation.
- Skill relevance analysis.
- Formatting and readability checks.

### 5. Personalized Interview Simulator
- Interactive mock interviews.
- AI-generated follow-up questions.
- Answer evaluation.
- Feedback on technical and behavioral responses.

### 6. Job Recommendation System
- Recommend relevant job opportunities.
- Match user profiles with job descriptions.
- Identify skill gaps for target roles.

### 7. Resume Version Management
- Save multiple resume versions.
- Compare improvements between versions.
- Track changes in compatibility scores.

### 8. Enhanced Reporting
- More detailed PDF reports.
- Visual comparison charts.
- Skill gap reports.
- Progress tracking.

---

## 🤝 Contributing

Contributions, suggestions, and improvements are welcome.

To contribute:

1. Fork the repository.
2. Create a new branch.

```bash
git checkout -b feature/your-feature-name
```

3. Make your changes.
4. Commit your changes.

```bash
git commit -m "Add: your feature description"
```

5. Push the branch.

```bash
git push origin feature/your-feature-name
```

6. Open a Pull Request describing your changes.

Please ensure that API keys and other sensitive credentials are not included in commits.

---

## 📜 License

This project can be distributed under the MIT License.

If you choose the MIT License, add a `LICENSE` file containing the appropriate license text to the repository.

---

## 👨‍💻 Project Information

**Project Name:** AI Career Copilot

**Category:** Artificial Intelligence / Generative AI / Career Development

**Primary AI Engine:** Google Gemini

**Frontend:** HTML, CSS, JavaScript

**Application Type:** Browser-Based Web Application

**Core Purpose:** AI-powered resume analysis, resume refinement, and interview preparation.

---

## ⭐ Acknowledgements

- [Google Gemini](https://ai.google.dev/) – For generative AI capabilities.
- [jsPDF](https://github.com/parallax/jsPDF) – For PDF generation.
- [MDN Web Docs](https://developer.mozilla.org/) – For web development references.

---

**If you find this project useful, consider giving the repository a ⭐ on GitHub!**
