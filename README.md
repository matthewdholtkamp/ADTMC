# ADTMC Triage Assistant

The **ADTMC Triage Assistant** (Algorithm-Directed Troop Medical Care) is a single-page web application designed to assist medics and healthcare providers in triaging patients based on established medical protocols.

## Features

-   **Comprehensive Protocols**: Covers A-M categories of medical complaints, including:
    -   Ear, Nose, and Throat
    -   Musculoskeletal
    -   Gastrointestinal
    -   Cardiorespiratory
    -   Genitourinary
    -   Neuropsychiatric
    -   Constitutional
    -   Eye Complaints
    -   Gynecological
    -   Dermatological
    -   Environmental Injuries
    -   Miscellaneous
-   **Step-by-Step Decision Trees**: Guides the user through a series of questions and checks to determine the appropriate disposition.
-   **Red Flags Detection**: Prominently checks for "Red Flags" (critical symptoms) at the beginning of each protocol to ensure immediate escalation when necessary.
-   **Disposition Generation**: automatically determines the final disposition:
    -   Provider Now
    -   Advanced Enlisted Medic (AEM) Now
    -   MCP (Medical Care Protocol - Self/Home Care)
    -   Specialty Referral
-   **Encounter Summary**: Generates a formatted text summary of the triage path, subjective findings, and assessment plan, ready to be copied and pasted into an Electronic Health Record (EHR).
-   **Search Functionality**: Quickly find protocols by chief complaint.
-   **Responsive Design**: Built with Tailwind CSS to work on various screen sizes.

## Usage

This application is built as a **Single Page Application (SPA)** contained entirely within `index.html`.

1.  **Download**: Clone this repository or download the `index.html` file.
2.  **Run**: Open `index.html` in any modern web browser (Chrome, Edge, Firefox, Safari). No server or installation is required.

## Architecture

-   **Single File**: The entire application logic, data (`adtmcProtocols` JSON), and UI structure are contained within `index.html`.
-   **Styling**: Uses [Tailwind CSS](https://tailwindcss.com/) via CDN.
-   **Logic**: Vanilla JavaScript handles the state management, navigation, and summary generation.

## PWA Support

The code contains references to Service Worker (`sw.js`) and Web App Manifest (`manifest.json`) to enable Progressive Web App (PWA) capabilities (offline access, installability).

*Note: As of now, `sw.js` and `manifest.json` are not included in this repository. To fully enable PWA features, these files need to be added.*

## Contributing

Contributions are welcome! If you find a bug in the logic or want to update a protocol, please edit the `adtmcProtocols` object within `index.html`.
