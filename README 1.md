# Together: Less planning. More together.

A mobile-first web app that helps busy parents find and run meaningful activities with their children.

**Live site:** https://together-liard-iota.vercel.app

## The problem
Busy parents want quality time with their kids but lose it to planning: what to do, with which materials, in how much time, for which ages.

## What it does
- **Plan:** a short pop-up flow asks six questions (ages, time, mood, materials, who is joining, indoors or outdoors), then recommends three activities. "Surprise us" picks one for you.
- **Activity Mode:** step-by-step guidance with a progress bar, Back and Next, Pause, and an exit confirmation. Hints, "make it easier", "make it more exciting" and variations are available for each activity, and some have an optional timer. Progress survives a refresh.
- **Memories:** completed activities with ratings and notes, plus favorites you can repeat or remove.
- **Family Preferences:** edit all answers at once, set constraints (quiet, low mobility), or clear all saved data.

## How recommendations work
A curated library of 16 activities is filtered by age, time, location and constraints, then ranked by mood match, time fit, mixed-age fit, past ratings and recent repeats. Each card explains why it fits. The logic is in `rank()` in `index.html`.

**No AI model is connected.** The structure allows a recommendation service to be added later through a backend, without exposing API keys in the browser.

## Privacy and safety
- No accounts, no analytics, no names, birth dates, photos or recordings.
- Data stays in the browser (localStorage) and is never sent anywhere.
- Every activity has a safety note and assumes adult supervision.
- This prototype has not had a legal or privacy-compliance review.

## Tech
Plain HTML, CSS and JavaScript in a single `index.html`. No build step. Deployed on Vercel.

## Run locally
Open `index.html` in a browser.

## Roadmap
AI-powered recommendations through a backend, an installable PWA, more activities, and testing with real families. A longer-term vision is a physical AI family companion.
