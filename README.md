# MoodPalette-Daily-Mood-Tracker

Description
A simple and visually appealing web app that allows users to log their daily moods and view them as a colorful calendar heatmap.

## Tech Stack
- React

## Requirements
- Mood selection interface (use emoji or color buttons for mood selection)
- Calendar heatmap display (map moods to colors and show them on a monthly grid)
- Local storage persistence (save moods locally so data stays after refresh)

## Installation
1. Clone the repository:
   bash
   git clone https://github.com/your-username/MoodPalette-Daily-Mood-Tracker.git
   cd MoodPalette-Daily-Mood-Tracker
   
2. Install dependencies:
   bash
   npm install
   
3. No additional environment variables are required.

## Usage
1. Start the development server:
   bash
   npm start
   
2. Open your browser and navigate to `http://localhost:3000`.
3. Click on an emoji or colored button to log today’s mood.
4. View your mood history in the calendar heatmap.

## Implementation Steps
1. Initialize the project using Create React App:
   bash
   npx create-react-app moodpalette
   cd moodpalette
   
2. Create a `MoodSelector` component featuring emoji or color buttons. Use React state to track the selected mood.
3. Create a `CalendarHeatmap` component that:
   - Reads saved mood entries from `localStorage`.
   - Maps each date to a background color based on the mood.
   - Renders a month-by-month grid.
4. Implement a `storage.js` utility module to handle saving and retrieving mood data from `localStorage`.
5. In `App.js`, integrate `MoodSelector` and `CalendarHeatmap`, passing props and handler functions to update state and persist data.
6. Add CSS styles (or a CSS-in-JS solution) to:
   - Style the mood buttons with clear emoji/color indicators.
   - Lay out the calendar grid responsively.
   - Apply hover and active states for better UX.
7. Test across browsers and edge cases (e.g., no data for a given month) and refine UX interactions.

(Optional) ## API Endpoints
This project uses only local storage for persistence; no external API endpoints are required.