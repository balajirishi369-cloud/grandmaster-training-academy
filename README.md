# Personal Grandmaster Training Academy

## Run it

Double-click `Open in Chrome.bat` to open `index.html` in Chrome. You can also open the HTML file directly. For installable PWA support and service-worker caching, serve this folder over HTTPS (or localhost), then use the browser's **Install app** option. No build step is required. A GitHub Pages workflow is included under `.github/workflows/pages.yml`; it expects these files at the repository root and the `main` branch to be the publishing source.

## Included in this delivery

- Responsive training workspace with a 64-square interactive chessboard.
- Mouse drag, touch tap-to-select/tap-to-move, legal move filtering, check indication, castling, en passant, promotion, board rotation, undo/redo, FEN import/export, and basic PGN import/export.
- A two-step Italian Game starter lesson: 1. e4, then 2. Nf3, followed by 3. Bc4. The coach supplies 1...e5 and 2...Nc6.
- 20-minute countdown, session report, same-day resume, and local browser persistence.
- Installable web-app manifest and service worker for offline caching.

## Scope still requiring source material or integration

This is a working starter application, not the complete specification. The licensed Lichess puzzle archive is available under CC0, but it has not been imported or validated for this app, so no puzzle positions have been fabricated and no tactics curriculum is claimed. Stockfish is not integrated; engine evaluations are not displayed or simulated. The advanced calculation, tactical, endgame, visualization, mixed challenge, analysis-tree, and long-term progress curricula are not populated. Progress is stored in this browser's local storage; data export/backup is not implemented. The manifest has no app icon assets.

The board's move generator covers standard legal moves and common special moves, but has not been certified against a comprehensive chess rules test suite. Treat this delivery as a functional foundation pending the full acceptance suite from the specification.

## Data storage

Session state is stored under `gta-state` in browser local storage. Clearing site data removes it. FEN can be copied from the FEN dialog as a simple position backup.
