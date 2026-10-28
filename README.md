# Together – Less planning. More together.

Mobile-first web app that recommends family activities and guides parents through them step by step.

- Plan: ages, time, mood, materials, participants, location. "Find activities" or "Surprise us".
- Activity Mode: progress, hints, easier/exciting/variation, optional timer, pause, exit confirm, session restored after refresh.
- Memories: history with notes, favorites, repeat or remove.
- Family Preferences: same inputs plus constraints, and clear all data.

Recommendations are deterministic scoring over a curated library of 16 activities (see `rank()` in index.html). No AI model is connected. Data stays in localStorage. No accounts, no analytics.

Run: open `index.html`, or deploy on Vercel (Framework: Other, no build).
