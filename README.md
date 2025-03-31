# Word Unscramble Game

## Description

This is a simple, interactive single-file web application (HTML, CSS, JS) designed to help users, particularly children, learn positive phrases and moral values.

Sentences related to moral values are presented with the letters within each word jumbled, while maintaining the original word order in the sentence. Users can drag and drop the letters or type directly into the provided text box below each word to unscramble it and reconstruct the original phrase. The game provides immediate feedback on correctness and includes options to show the solution or reset the game.

## Demo

The game displays several sentences, each on its own line within a card-like container. Each word in the sentence appears as a set of jumbled letter tiles above an input box. Users can:

-   Drag and drop the orange letter tiles within a word's container to reorder them.
-   Type the unscrambled word directly into the input box below the tiles (typing will also attempt to reorder the tiles above).
-   Click the "Check Answers" button to see which words are correct (highlighted green and locked) and incorrect (highlighted red).
-   Click the "Show Solution" button for a specific sentence to reveal the answer and lock that sentence.
-   Click the Reset icon (🔄) in the header to reload the game.

## Features

-   **Interactive Unscrambling:** Drag & drop letter tiles or type answers.
-   **Sentence Structure:** Maintains the original order of words within sentences.
-   **Instant Feedback:** Typing in the input box rearranges letters above.
-   **Validation:** "Check Answers" button highlights correct (green) and incorrect (red) words.
-   **Locking:** Correctly answered words become non-interactive.
-   **Hints:** "Show Solution" button reveals the answer for a specific sentence.
-   **Reset:** Easily restart the game.
-   **Responsive Design:** Adapts layout for different screen sizes (desktops, tablets, mobiles).
-   **Single File:** All HTML, CSS, and JavaScript are contained within one `.html` file for easy deployment and sharing.
-   **Customizable Content:** Easily change the sentences by editing the `originalSentences` array in the JavaScript code.

## How to Use

1.  Download the `.html` file.
2.  Open the file in any modern web browser (like Chrome, Firefox, Edge, Safari).
3.  Look at the jumbled words in each sentence line.
4.  **To unscramble:**
    -   Click and drag the orange letter tiles within a single word's area to arrange them correctly.
    -   _Alternatively_, click into the text box below a word and type the correct spelling (letters above will rearrange).
5.  Click the **"Check Answers"** button at the bottom to see your progress. Correct words will turn green and become locked. Incorrect words will be highlighted in red.
6.  If you are stuck on a particular sentence, click the **"Show Solution"** button below it.
7.  To start over completely, click the **Reset icon** (🔄) next to the main title.

## Tech Stack

-   HTML5
-   CSS3
-   Vanilla JavaScript (ES6+)
-   [SortableJS](https://github.com/SortableJS/Sortable) Library (for drag-and-drop)

## Customization

To change the sentences used in the game:

1.  Open the `.html` file in a text editor.
2.  Locate the `<script>` section near the end of the file.
3.  Find the `originalSentences` array:
    ```javascript
    const originalSentences = [
        "LOVE ALL SERVE ALL",
        "LIFE IS A GAME PLAY IT",
        // Add or modify sentences here
    ];
    ```
4.  Edit, add, or remove strings within the square brackets `[...]`. Ensure each sentence is enclosed in double quotes (`"`) and separated by commas.
5.  Save the file. The game will now use your updated sentences.

---

Created by - `Ashwin Narayanan S` (with Gemini-2.5-pro assistance)

Date - `March 2025`
