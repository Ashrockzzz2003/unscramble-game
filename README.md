# Interactive Unscramble Games: Quotes & Ashtothram

## Description

This project contains two simple, interactive single-file web applications (HTML, CSS, JS), each designed for a specific learning purpose:

1.  **`index.html` (Quotes/Phrases):** Helps users, particularly children, learn positive phrases and moral values by unscrambling words within sentences.
2.  **`ashtothram.html` (Ashtothram Game):** Helps users learn the [Sathya Sai Ashtothram (108 Names)](https://sairhythms.sathyasai.org/song/ashtothram-108-names-bhagawan-sathya-sai-baba) by unscrambling words within randomly selected lines.

In both games, sentences/lines are presented with the letters within each word jumbled, while maintaining the original word order. Users can drag and drop the letters or type directly into the provided text box below each word to unscramble it. The games provide immediate feedback on correctness and include options to show the solution or reset.

## Demo

Each game displays several sentences/lines, each within its own card-like container. Words appear as a set of jumbled orange letter tiles above an input box. Users can:

-   Drag and drop the letter tiles within a word's container to reorder them.
-   Type the unscrambled word directly into the input box below the tiles (typing will also attempt to reorder the tiles above).
-   Click the **"Check Answers"** button to see which words are correct (highlighted green and locked) and incorrect (highlighted red).
-   Click the **"Show Solution"** button for a specific sentence/line to reveal the answer and lock that sentence/line.
-   Click the **Reset/Randomize icon** (🔄) in the header:
    -   In `ashtothram.html`, this loads a new random set of 5 lines.
    -   In `index.html` (it would restart the fixed set of sentences (or simply reload the page). Currently, the simplest reset for both is a page reload.

## Features

-   **Two Distinct Games:** Separate files for general quotes and the Ashtothram.
-   **Interactive Unscrambling:** Drag & drop letter tiles or type answers.
-   **Specific Content:**
    -   `index.html`: Uses a configurable set of general sentences/quotes.
    -   `ashtothram.html`: Uses the 108 names; loads 5 random consecutive lines.
-   **Structure Preservation:** Maintains the original order of words within sentences/lines.
-   **Instant Feedback:** Typing in the input box rearranges letters above.
-   **Validation:** "Check Answers" button highlights correct (green) and incorrect (red) words.
-   **Locking:** Correctly answered words become non-interactive.
-   **Hints:** "Show Solution" button reveals the answer for a specific sentence/line.
-   **Reset/Randomize (`ashtothram.html`):** "Pick Random" button (🔄) loads a new random set of lines.
-   **Responsive Design:** Adapts layout for different screen sizes (desktops, tablets, mobiles).
-   **Single File per Game:** All HTML, CSS, and JavaScript for each game are contained within their respective `.html` files for easy deployment and sharing.
-   **Customizable Content:** Easily change the sentences/lines by editing the relevant array in each file's JavaScript code.

## How to Use Locally

1.  Download the project files (including `index.html` and `ashtothram.html`).
2.  Open **either** file in any modern web browser (like Chrome, Firefox, Edge, Safari):
    -   Open `index.html` for the general quotes game.
    -   Open `ashtothram.html` for the Ashtothram game.
3.  For `ashtothram.html`, a random set of 5 lines will load initially. You can get a new set by clicking the "Pick Random" (🔄) button.
4.  Look at the jumbled words in each sentence/line.
5.  **To unscramble:**
    -   Click and drag the orange letter tiles within a single word's area to arrange them correctly.
    -   _Alternatively_, click into the text box below a word and type the correct spelling (letters above will rearrange).
6.  Click the **"Check Answers"** button at the bottom to see your progress. Correct words will turn green and become locked. Incorrect words will be highlighted in red.
7.  If you are stuck on a particular sentence/line, click the **"Show Solution"** button below it.
8.  To start over completely (or get a new random set in `ashtothram.html`), click the **Reset/Randomize icon** (🔄).

## Tech Stack

-   HTML5
-   CSS3
-   Vanilla JavaScript (ES6+)
-   [SortableJS](https://github.com/SortableJS/Sortable) Library (for drag-and-drop)

## Customization

To change the sentences/lines used in the games:

1.  Open the desired `.html` file (`index.html` or `ashtothram.html`) in a text editor.
2.  Locate the `<script>` section near the end of the file.
3.  **For `index.html` (Quotes):**
    -   Find the `originalSentences` array (or equivalent if named differently).
        ```javascript
        const originalSentences = [
            "BE KIND ALWAYS",
            // Add or modify sentences here
        ];
        ```
    -   Edit, add, or remove strings within the square brackets `[...]`. Ensure each sentence is enclosed in double quotes (`"`) and separated by commas.
4.  **For `ashtothram.html`:**
    -   Find the `ashtothram` array.
        ```javascript
        const ashtothram = [
            "OM SRI SAI SATHYA SAI BABAYA NAMAH",
            "OM SRI SAI SATHYASWAROOPAAYA NAMAH",
            // Add or modify lines here
        ];
        ```
    -   Edit, add, or remove strings within the square brackets `[...]`. Ensure each line is enclosed in double quotes (`"`) and separated by commas. The range selection and random picking will automatically adapt to the total number of lines.
5.  Save the modified file.

---

Created by - `Ashwin Narayanan S` (with Gemini-2.5-pro assistance)
