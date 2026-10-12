# PRD: Word Scramble Game

## 1. Overview
This document defines the requirements for creating a single-file Word Scramble game similar in style to the memory game. The goal is to build a simple browser game that runs without any external dependencies and is playable directly in a browser.

## 2. Product Goal
Create a fun and engaging word-based game where the player unscrambles letters to form a real word. The game should be easy to understand, responsive, and fully playable from a single HTML file.

## 3. Problem Statement
Users want a lightweight, childhood-style word game that can be built quickly in a browser without frameworks or extra setup. The game should feel polished enough to play immediately while remaining simple to maintain.

## 4. Objective
Build a Word Scramble game with random word selection, scrambled letters, answer checking, scoring, and game reset behavior, all within a single HTML file.

## 5. User Stories
- As a player, I want to see a scrambled word so I can try to guess the correct word.
- As a player, I want to type my answer and submit it to check if I am correct.
- As a player, I want to see my score update after each successful answer.
- As a player, I want a new word to appear when I finish a round.
- As a player, I want to restart the game when I want to play again.

## 6. Functional Requirements

### 6.1 Game Setup
- The game shall display a scrambled word to the user.
- The word shall be selected from a predefined list of words.
- The word shall be shuffled before each round.
- The same word shall not repeat consecutively if possible.

### 6.2 User Input
- The app shall provide a text input field for entering the guess.
- The user shall be able to submit the guess with a button or Enter key.
- Empty submissions shall be ignored or show a validation message.

### 6.3 Answer Checking
- The game shall compare the user’s guess with the original word.
- Correct answers shall increase the score.
- Incorrect answers shall show a feedback message and may reduce lives or attempts.

### 6.4 Game Progression
- After a correct answer, a new scrambled word shall load.
- The game should continue until the user resets or reaches the game-end condition.
- A round counter or total score should be displayed.

### 6.5 Game End Condition
- The game shall end when the user runs out of attempts or lives.
- A game-over message shall be displayed.
- The player shall be able to restart the game.

### 6.6 Score and Feedback
- A score display shall show the player’s current score.
- Feedback messages shall appear such as: correct, incorrect, game over, or next word.

## 7. UX Requirements
- The game should be visually clean and easy to read.
- Buttons and input should be large enough for simple interaction.
- Messages should be clear and immediate.
- The layout should work on desktop and mobile screens.

## 8. Accessibility Requirements
- Input should be keyboard accessible.
- Buttons should be focusable and clickable with keyboard.
- Text should have good contrast against the background.
- The page should remain readable and usable when resized.

## 9. Technical Requirements
- The game shall be implemented in a single HTML file.
- CSS shall be embedded in the same file.
- JavaScript shall handle all word logic, score tracking, and UI updates.
- No external libraries or dependencies should be required.

## 10. Acceptance Criteria
1. A scrambled word is displayed at the start of the game.
2. The user can type a guess and submit it.
3. Correct answers increase the score.
4. Incorrect answers trigger a visible response.
5. A new word loads after a successful answer.
6. The player can restart the game.
7. The game works on a standard browser without errors.
8. The game remains playable on a smaller screen.

## 11. Edge Cases to Validate
- Empty answer submission
- Same word repeated in consecutive rounds
- Duplicate letters in a word
- Users pressing Enter instead of clicking Submit
- Wrong answer when lives are low
- Restarting the game mid-round

## 12. Risks and Considerations
- Word selection should avoid repeated repetitions when possible.
- Long words may be harder to scramble visually.
- Difficulty balancing matters for player engagement.
- UI should not hide feedback messages behind other elements.

## 13. Proposed Implementation Notes
- Store word lists in a JavaScript array.
- Use a shuffle function to randomize letters.
- Maintain game state variables such as score, attempts, current word, and round.
- Render updates through DOM manipulation only.
- Use simple CSS for a polished but lightweight interface.

## 14. Exit Criteria
The game is complete when it is playable, responsive, and works without errors in a browser. The user can start a round, submit guesses, receive feedback, and restart the game with full functionality.
