# Memory Match Challenge Game

A Flask-based memory matching game where players test their memory by matching pairs of icons after a brief preview period.

## Project Structure

```
memory_match/
│
├── app.py                    # Main Flask application
├── static/                   # Static assets
│   ├── css/
│   │   └── style.css         # CSS styling
│   └── js/
│       └── game.js           # Game logic
│
└── templates/                # HTML templates
    ├── index.html            # Home page
    └── game.html             # Game page
```

## Features

- Configurable board size (5x5 to 10x10)
- Memory challenge with preview period equal to board size
- Track time, revisits, and matches
- Drag-and-drop matching functionality
- Performance rating system
- Responsive design for different screen sizes

## Setup Instructions

1. **Create a new directory for your project**

```bash
mkdir memory_match
cd memory_match
```

2. **Create a virtual environment and activate it**

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. **Install Flask**

```bash
pip install Flask
```

4. **Create the necessary directories**

```bash
mkdir -p static/css static/js templates
```

5. **Create all the files with the provided code**

Copy the code from each artifact into the appropriate file:
- `app.py` in the root directory
- `static/css/style.css`
- `static/js/game.js`
- `templates/index.html`
- `templates/game.html`

6. **Run the application**

```bash
python app.py
```

7. **Access the application**

Open your web browser and go to: `http://127.0.0.1:5000/`

## How to Play

1. Select a board size on the home page
2. Memorize the icons displayed on the board (you have 2×N seconds for an NxN board)
3. After the memorization phase, the icons will be hidden
4. Click on cards to reveal them
5. Match pairs either by:
   - Clicking on two cards with the same icon consecutively
   - Clicking on one card and dragging it to another matching card
6. Try to complete the game with minimal revisits and in the shortest time possible
7. The center tile will always display a brain icon

## Game Mechanics

- **Preview Phase**: All icons are visible for a number of seconds equal to double the board size
- **Matching Phase**: Find all pairs of matching icons
- **Drag and Drop**: You can click a card to reveal it, then drag it to another card you think matches
- **Scoring**: Performance is measured by time taken and number of revisits

Enjoy the game!
