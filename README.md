# InfraScan
### AI-Powered Crack & Damage Assessment for Civil Infrastructure

InfraScan is an AI-based infrastructure inspection project designed to identify visible cracks and damage from images of roads, bridges, and other civil structures.

## Tech Stack

Frontend: React.js, Vite

Backend: Python, FastAPI

Database: PostgreSQL

Image Processing: Pillow, NumPy

AI/Deep Learning: TensorFlow/Keras or a suitable object detection model

Version Control: Git, GitHub

Code Editor: Visual Studio Code

## Features

- User authentication and role-based access
- Infrastructure asset management
- Inspection image upload and storage
- Image preprocessing for AI analysis
- AI-based crack and damage assessment
- Assessment result management
- Dashboard for viewing inspection information

## System Workflow

1. User logs in to the application.
2. User selects or creates an infrastructure asset.
3. Inspection images are uploaded and validated.
4. Images are preprocessed for analysis.
5. The AI model analyzes the images.
6. Assessment results are stored and displayed for review.

## Datasets

- **RDD2022** — Planned primary dataset for road damage detection.
- **Concrete Crack Images for Classification** — Cracked and non-cracked concrete images.
- **CrackForest (CFD)** — Road crack images.
- **SDNET2018** — Concrete images of bridge decks, walls, and pavements.
- **Crack500** — Road crack images.

## Project Structure

```text
InfraScan/
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── services/
│   │   └── App.jsx
│   └── package.json
│
├── backend/
│   ├── app/
│   │   ├── routes/
│   │   ├── models/
│   │   ├── schemas/
│   │   ├── services/
│   │   └── main.py
│   └── requirements.txt
│
├── docs/
├── datasets/
├── .env.example
├── .gitignore
└── README.md
```

## Database Design

The initial database design consists of four tables:

- **Users** — user accounts and roles
- **Infrastructure_Assets** — infrastructure asset details
- **Uploaded_Images** — uploaded image metadata and file paths
- **Damage_Assessments** — AI assessment and review details

## Setup

### Prerequisites

- Node.js and npm
- Python
- PostgreSQL
- Git

### 1. Clone the repository

```bash
git clone <repository-url>
cd InfraScan
```

### 2. Set up the backend

```bash
python -m venv .venv
```

Activate the virtual environment and install dependencies:

```bash
pip install -r backend/requirements.txt
```

### 3. Set up the frontend

```bash
cd frontend
npm install
npm run dev
```

### 4. Configure the database

Create a PostgreSQL database and configure the connection using environment variables. Apply the project's database setup or migration scripts before running the backend.

*Update the commands above to match the actual repository structure and application entry point.*

## Project Status

Currently under development.

