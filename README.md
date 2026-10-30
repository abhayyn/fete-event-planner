# Fête – AI Celebration & Event Planner

PromptWars Challenge 05 submission. A GenAI planning assistant for weddings, birthdays, anniversaries, baby showers and community events.

## What it does
- Takes event type, name, city, date, guests, budget and vibe
- Generates a **budget breakdown**, a **countdown timeline**, a **vendor checklist** and **personalised ideas** using Gemini
- Interactive checklists with progress tracking, plan download and print
- Falls back to a built-in template plan if the AI is unavailable
- Accessible: skip link, labelled inputs, ARIA live regions, keyboard focus, dark mode, responsive

## Tech
Plain HTML/CSS/JS front end, one Vercel serverless function (`api/plan.js`) calling the Gemini API. The API key stays server-side.

## Run / deploy
1. Get a free key at https://aistudio.google.com
2. Import this repo into Vercel
3. Add environment variable `GEMINI_API_KEY` (optional: `GEMINI_MODEL`)
4. Deploy

Local: `npm i -g vercel && vercel dev`

## Structure
- `index.html` – the app
- `api/plan.js` – serverless AI endpoint
