# EcoLearn — Smart Sustainability Learning Platform

EcoLearn is a responsive React + TypeScript demo that combines bite-sized sustainability lessons, knowledge checks, daily eco-challenges, SDG exploration, gamified progress and illustrative college analytics.

## What works in this MVP

- **Student dashboard:** points, level, streak display, weekly activity visualization and recommended lessons.
- **Learning library:** six short lessons across waste, renewable energy, climate, water, biodiversity and responsible consumption.
- **Interactive lessons:** multi-part content, key takeaways, completion state and points.
- **Knowledge check:** five multiple-choice questions, scoring, explanations and topic suggestions for incorrect answers.
- **Daily challenges:** complete actions, earn points, and prevent duplicate rewards for the same challenge on the same calendar day.
- **My impact:** local activity history and transparent explanation of what is and is not measured.
- **SDG explorer:** connections to UN Sustainable Development Goals 4, 6, 7, 12, 13, 14 and 15.
- **College analytics:** charts and summaries that clearly identify illustrative data as demo data.
- **Local persistence:** demo profile, preferences, quiz scores, points and activity stored in browser LocalStorage.
- **Responsive UI:** desktop sidebar, mobile navigation, accessible labels, reduced-motion support and interactive chart tooltips.

## Technology

- React 18 and TypeScript
- Vite
- Tailwind CSS configuration plus a custom responsive design system
- Lucide icons
- Recharts for data visualizations
- Browser LocalStorage for demo progress

No backend, external AI service, or institutional database is connected. Recommendations are transparent rule-based matches using the learner's selected interests. Environmental outcomes are not presented as verified savings; activity counts are self-reported, and college charts are clearly illustrative.

## Run locally with Visual Studio Code

1. Install **Node.js LTS** from https://nodejs.org/ and **Visual Studio Code** from https://code.visualstudio.com/.
2. Open this repository in VS Code: https://github.com/Sajeel588/ecolearn2
3. Open **Terminal → New Terminal**.
4. Install packages:
   ```bash
   npm install
   ```
5. Start the development server:
   ```bash
   npm run dev
   ```
6. Open the local URL Vite prints in the terminal (usually http://localhost:5173).
7. Stop the server with **Ctrl+C** in the terminal.

For a production build:
```bash
npm run build
npm run preview
``

## Deploy to GitHub Pages

A GitHub Actions workflow builds the app and publishes the `dist` folder when changes are pushed to `main`.

1. In the repository, open **Settings → Pages**.
2. Under **Build and deployment**, choose **GitHub Actions** as the source.
3. Push a commit to `main` or manually run the **Deploy EcoLearn to GitHub Pages** workflow from the Actions tab.
4. Wait for the workflow to finish, then open the Pages URL shown in Settings → Pages.

The Vite configuration uses a relative asset base for repository Pages compatibility.

## Demo notes and limitations

- LocalStorage is browser- and device-specific. This is not a multi-user account system, and clearing browser data resets saved progress.
- The demo starts with sample points and a sample streak so the dashboard is ready to present. Clearing the `ecolearn-v1` LocalStorage key resets the demo to its starter state.
- The weekly chart and campus engagement figures are illustrative. College metrics are not real institution results.
- Eco-points are participation rewards, not a measure of environmental benefit.
- No live AI API or backend is configured.
- For a production launch, add authentication, a secure database, consent and privacy flows, validated environmental impact assumptions, and automated tests.

## Suggested hackathon demo flow

1. Show the dashboard and personalized lesson cards.
2. Open a lesson, move through its sections and complete it.
3. Take the knowledge check and review explanations.
4. Complete a daily challenge and show points/activity update.
5. Refresh the browser to demonstrate LocalStorage persistence.
6. Open SDG Explorer and College Analytics, explaining the difference between local activity and illustrative sample data.
