# AI-Powered Receipt Ingredient Detector

## Overview
This project is an AI-powered receipt scanner that detects ingredients from uploaded images and suggests meal ideas with recipe links. The system utilizes computer vision to recognize ingredients visually, without relying solely on text extraction.

This project was developed during **ConUHacks IX**.

## Features
- Upload images of receipts or ingredients.
- AI detects ingredients visually and extracts text when necessary.
- Retrieve recipe suggestions based on detected ingredients.
- Integrated with Google Cloud Vision API for image processing.

## Demo
Watch the YouTube demo: [AI-Powered Receipt Scanner Demo](https://youtu.be/yrHQ3jAXDcE)

## Tech Stack
- **Frontend**: React (JavaScript/TypeScript)
- **Backend**: FastAPI (Python)
- **Cloud Services**: Google Cloud Vision API
- **Communication**: REST API

## Installation & Setup
### Prerequisites
Ensure you have the following installed:
- **Node.js** (for running the frontend)
- **Python 3.x** (for running the backend)
- **Google Cloud Vision API credentials**

### Backend (FastAPI)
1. Navigate to the backend directory:
   ```sh
   cd backend
   ```
2. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```
3. Start the FastAPI server:
   ```sh
   uvicorn main:app --reload
   ```

### Frontend (React)
1. Navigate to the frontend directory:
   ```sh
   cd frontend
   ```
2. Install dependencies:
   ```sh
   npm install
   ```
3. Start the React development server:
   ```sh
   npm start
   ```
4. Open the application in your browser at:
   ```
   http://localhost:3000
   ```

## API Endpoints
| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/upload` | Upload an image for ingredient detection |
| GET | `/ingredients` | Retrieve detected ingredients |
| GET | `/recipes?ingredients=...&meal_type=...` | Get meal ideas based on ingredients |

## Usage Restrictions
Please note that this project is not openly available for public use, as API calls to the Google Cloud Vision API incur significant costs. If you wish to use or test this project, please contact the developer.


