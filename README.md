# BenefitFinder

A CruzHacks 2025 project that helps students discover government aid, scholarships, and other benefits through a guided questionnaire and an AI-assisted application workflow.

**Best Beginner Hack — CruzHacks 2025** · [Project on Devpost](https://devpost.com/software/benefitfinder)

## What it does

- Collects a profile through a guided questionnaire.
- Organizes assistance into education, employment, housing, and healthcare.
- Uses Gemini to suggest relevant programs and follow-up questions.
- Explores form prefilling and PDF-based application workflows.

## Project structure

| Path | Purpose |
| --- | --- |
| `frontend/` | React, TypeScript, Vite, and Tailwind interface |
| `frontend/src/lib/` | Firebase integration, Gemini helpers, and profile utilities |
| `backend/` | Python services for benefits, eligibility, and forms |

## Run the frontend

```bash
git clone https://github.com/ggrantrichards/cruzhackies.git
cd cruzhackies/frontend
npm install
npm run dev
```

Configure your own Firebase project in the frontend integration and provide `VITE_GEMINI_API_KEY` in a local environment file for the Gemini features. The frontend's API calls currently run in the browser; Vite-prefixed environment values are visible to clients. A production deployment should move secret-bearing requests behind a backend.

```bash
npm run build
npm run preview
```

## Status

Hackathon prototype. Use fictional profiles for demos: the application workflow can send profile fields to Gemini. Recommendations and generated forms need review against the official program requirements; this is not an official benefits application service.

## Team

Glenn Grant-Richards, Surya, and Max, as credited in the original repository.
