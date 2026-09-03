# ChessCoach

A browser-based beginner chess coach focused on **learning the reasoning behind a move**, not simply winning the game.

## V2

V2 introduces:

- Reliable legal chess rules through `chess.js`.
- No take-backs after a player's move.
- A rank for the move the player actually made.
- Up to five ranked alternative moves.
- A plain-English reason for each candidate.
- Beginner concepts such as checks, captures, threats, centre control and development.
- A thinking checklist after the coach's reply.
- A hint that encourages the player to discover the idea rather than blindly reveal a move.
- A simple local teaching evaluator that considers material, centre control, development, mobility and tactical features.

## Important limitation

This is intentionally the **first learning iteration**, not a replacement for Stockfish. The UI and analysis pipeline are designed so that the next version can add Stockfish MultiPV and use its evaluations to rank 3–5 candidates accurately.

The current HTML imports `chess.js` from jsDelivr, so this version requires an internet connection when opened directly. For the original no-internet goal, bundle the dependency locally in the next packaging step.

## Run

Open `chess_coach.html` in a modern browser.

## Product direction

The long-term goal is a coach for complete beginners that gradually teaches a repeatable decision process:

1. What is my opponent threatening?
2. Are there checks, captures or forcing moves?
3. Which of my pieces is doing least?
4. What does my candidate move improve?
5. What can my opponent do immediately after it?

Future iterations should add Stockfish MultiPV, tactical classification, opening/position lessons, mistake patterns, progress tracking, adaptive difficulty, and an end-of-game learning report.
