# Word Scramble Game Check List

Use this list to validate that the game works correctly after implementation.

## Basic Gameplay
- [ ] Page loads without errors
- [ ] A scrambled word is displayed on load
- [ ] User can type a guess in the input box
- [ ] Submit button works
- [ ] Enter key works as a valid submission

## Correctness
- [ ] Correct answer increases the score
- [ ] Wrong answer shows a failure message
- [ ] Correct word is checked case-insensitively if needed
- [ ] Game continues with a new word after a correct answer
- [ ] Wrong answer does not accidentally count as success

## Game State
- [ ] Score updates correctly
- [ ] Attempts/lives reduce appropriately if implemented
- [ ] Game-over state appears when the game ends
- [ ] Restart button resets the game completely
- [ ] Repeated or duplicate words do not break the game

## UI and Design
- [ ] Layout is readable and centered
- [ ] Buttons look clickable and styled correctly
- [ ] Message area updates properly
- [ ] Page remains usable on mobile screens
- [ ] No overlapping text or broken styling

## Browser Validation
- [ ] Open the HTML file directly in a browser
- [ ] Refresh the page and verify it still loads
- [ ] Confirm there are no JavaScript errors in the console
- [ ] Try more than one round to confirm progression works

## Optional Enhancements
- [ ] Score persists using localStorage
- [ ] Difficulty levels work
- [ ] Timer is shown and counts correctly
- [ ] Hint/category feature functions as expected
