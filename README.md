# WHS-Handicap-Calculator-simulator
# GolfPal WHS (World Handicap System) Calculator

GolfPal WHS Calculator is a client-side web application designed to help users understand and simulate World Handicap System calculations. It allows users to manage golf courses, golfer profiles, and scores, and automatically calculates Handicap Indexes based on WHS rules.

## Key Features

*   **Course Management (`index.html`):**
    *   Add, view, edit, and delete golf courses and their specific tees.
    *   Includes a large predefined database of Kenyan golf courses and their ratings.
    *   Manual entry for custom courses, including Course Rating, Slope Rating, Par, and hole-by-hole details (Par, Stroke Index).
    *   Support for 18-hole and 9-hole (Front, Back, Complete 9) rounds.
*   **Golfers & Scores Management (`golfers.html`):**
    *   Add and manage golfer profiles (name, handicap index, gender, home club).
    *   Enter new scores, including date, course, tee, and hole-by-hole gross scores.
    *   View, edit, and delete scores through an intuitive modal interface.
    *   Automatic recalculation of Handicap Index (HI) after any score entry or modification.
    *   Implements core WHS calculation logic:
        *   Adjusted Gross Score (AGS) calculation (including Net Double Bogey).
        *   Score Differentials.
        *   Handicap Index (HI) calculation (best 8 of last 20 differentials).
        *   WHS Safeguards: Soft Cap, Hard Cap, Exceptional Score Reduction (ESR).
        *   Simulated Playing Conditions Calculation (PCC) adjustment (manual input).
    *   Detailed calculation log to trace HI changes.
*   **Handicap Overview (`overview.html`):**
    *   Displays a sortable table of all golfers with their current Handicap Index, number of scores, last played date, and Lowest Handicap Index (LHI).
    *   Detailed view for each golfer showing:
        *   Current HI, LHI.
        *   Reasons for any cap or ESR adjustments.
        *   Comprehensive score history table highlighting contributing scores.
        *   Expandable hole-by-hole scores for each round.
*   **Help & FAQ (`help.html`):**
    *   Provides detailed explanations of WHS terms, calculations, and simulator-specific functionalities.
    *   Accordion UI for easy navigation of help topics.

## Technologies Used

*   **HTML5:** For the basic structure of the web pages.
*   **Tailwind CSS:** For utility-first styling and rapid UI development.
*   **Vanilla JavaScript (ES6+):** For all client-side logic, DOM manipulation, WHS calculations, and interactions.
*   **Browser Local Storage:** Used to persist all user-entered data (courses, golfers, scores) directly in the user's browser.

## How to Use

1.  Clone or download the repository.
2.  Since this is a client-side application, no special build process or server is required.
3.  Open the `index.html` file (for Course Management) or any of the other HTML files (`golfers.html`, `overview.html`, `help.html`) directly in your web browser to start using the application.

## Project Structure

The application is organized into four main HTML files, each serving a distinct purpose:

*   `index.html`: Course and Tee Management.
*   `golfers.html`: Golfer profiles, score entry, and WHS calculations.
*   `overview.html`: Handicap overview and detailed score history for all golfers.
*   `help.html`: Help, FAQ, and explanations of WHS concepts.

Each HTML file contains its own embedded JavaScript and CSS (primarily Tailwind utility classes and some shared custom styles) to manage its specific functionality.

## Notes & Limitations

*   This application is designed primarily for educational and simulation purposes to explore the World Handicap System.
*   All data is stored locally in the user's browser. Clearing browser data will remove all saved courses, golfers, and scores.
*   The Playing Conditions Calculation (PCC) is a manual input in this simulator, as it typically requires data from a wider set of scores played on a given day.

## Contributing

(Details to be added if the project will be open to contributions)

## License

(Details to be added if a specific license is chosen)
