# 🎮 Game Glitch Investigator: The Impossible Guesser

## 🚨 The Situation

You asked an AI to build a simple "Number Guessing Game" using Streamlit.
It wrote the code, ran away, and now the game is unplayable. 

- You can't win.
- The hints lie to you.
- The secret number seems to have commitment issues.

## 🛠️ Setup

1. Install dependencies: `pip install -r requirements.txt`
2. Run the broken app: `python -m streamlit run app.py`

## 🕵️‍♂️ Your Mission

1. **Play the game.** Open the "Developer Debug Info" tab in the app to see the secret number. Try to win.
2. **Find the State Bug.** Why does the secret number change every time you click "Submit"? Ask ChatGPT: *"How do I keep a variable from resetting in Streamlit when I click a button?"*
3. **Fix the Logic.** The hints ("Higher/Lower") are wrong. Fix them.
4. **Refactor & Test.** - Move the logic into `logic_utils.py`.
   - Run `pytest` in your terminal.
   - Keep fixing until all tests pass!

## 📝 Document Your Experience

### ✅ Game Purpose
The purpose of the game is to guess a randomly generated number within a given range. The game provides hints ("higher" or "lower") after each guess to guide the player. If the player guesses the correct number within the allowed attempts, they win; otherwise, they lose. The game also includes different difficulty levels that adjust the range and challenge.

---

### 🐞 Bugs Found

- The difficulty levels were not properly aligned with the number ranges, making the game inconsistent in challenge.
- The hint logic was reversed:
  - When the guess was lower than the secret number, the game incorrectly suggested going lower.
  - When the guess was higher than the secret number, the game incorrectly suggested going higher.

---

### 🔧 Fixes Applied

- Corrected the hint logic so that it accurately tells the player to go higher or lower based on their guess.
- Updated the difficulty levels to reflect the appropriate number ranges properly, ensuring a balanced gameplay experience.

---

## 📸 Demo

![Game Screenshot](./Screenshot%202026-03-21%20at%209.24.22%E2%80%AFPM.png)


## 🚀 Stretch Features

- [ ] [If you choose to complete Challenge 4, insert a screenshot of your Enhanced Game UI here]
