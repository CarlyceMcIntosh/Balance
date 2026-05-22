# Balance – Student AI Support Platform

Balance is a full-stack AI web application designed to help students balance academic productivity and mental well-being through two interaction modes: **Reflect** and **Focus**.

Reflect Mode provides supportive, journaling-style responses for processing thoughts, stress, and planning needs. Focus Mode provides more direct, task-oriented academic assistance and can use Canvas LMS context to generate more personalized responses.

---

## Overview

Balance was built to explore how tone, intent, and context shape chat-based AI user experiences. Instead of offering one generic assistant, the app separates support into two modes:

- **Reflect Mode** — supportive, conversational responses for self-reflection and mental well-being
- **Focus Mode** — direct, task-oriented responses for academic productivity
- **Canvas LMS Integration** — optional course-aware context for more personalized academic support
- **Session Summaries** — calendar-based summaries that help users review activity across both modes
- **User Accounts** — authentication and per-user data handling through Supabase

---

## My Contributions

This was a collaborative academic project built with a partner. My main contributions included:

- Developed Reflect Mode logic and prompt design for journaling-style AI responses
- Contributed to backend routing and response handling for mode-specific AI behavior
- Implemented Supabase authentication and account flows
- Built frontend calendar features to display and organize session summaries from both modes
- Helped refine the user experience, project structure, and overall application flow

---

## Tech Stack

**Frontend**
- React
- TypeScript
- Tailwind CSS

**Backend**
- Node.js
- Express

**Auth & Data**
- Supabase

**AI**
- OpenAI API

**Integrations**
- Canvas LMS API

---

## Features

- Chat-based AI interface with switchable Reflect and Focus modes
- Mode-specific backend logic and prompt behavior
- Supabase authentication and account management
- Optional Canvas LMS connection using a user-provided API key
- Calendar-based session summary interface
- Shared frontend interface with different AI behavior depending on the selected mode

---

## Architecture

At a high level, Balance uses a React frontend, an Express/Node.js backend, Supabase for authentication and user data, and the OpenAI API for AI-generated responses.

```txt
React Frontend
   |
   | sends chat messages + selected mode
   v
Express / Node.js Backend
   |
   | routes request based on Reflect or Focus mode
   v
Mode-Specific AI Logic
   |
   | optionally uses Canvas LMS context for Focus Mode
   v
OpenAI API Response
   |
   v
Rendered in Chat UI
```
## Project Structure
frontend/
  ├── components/
  ├── pages/
  ├── auth/
  └── styles/

backend/
  ├── routes/
  ├── controllers/
  ├── services/
  └── app.js
## Current Status
- Core chat flow implemented
- Reflect and Focus modes separated through backend routing and prompt logic
- Supabase authentication and account flows implemented
- Canvas LMS integration available for course-aware Focus Mode responses
- Calendar summary interface built for organizing activity across both modes
- Long-term memory and production deployment features were outside the scope of this version
  
## Authors
Carlyce McIntosh
Julie Amon
## Disclaimer
