# 🎮 Hangman Game

A classic word-guessing game built with Python and Pygame. Test your vocabulary skills by guessing letters to reveal the hidden word before the hangman is fully drawn!

## 🌟 Features

- **Visual Hangman Drawing**: Watch the hangman get drawn piece by piece with each wrong guess
- **Large Word Database**: Over 2,000 words of varying difficulty levels
- **Interactive GUI**: Clean, colorful interface built with Pygame
- **Real-time Feedback**: Immediate visual feedback for correct and incorrect guesses
- **Game State Display**: Track your progress with guessed letters and wrong attempts

## 🎯 How to Play

1. **Start the Game**: Run the program to begin a new game
2. **Guess Letters**: Press any letter key to make a guess
3. **Watch the Progress**: 
   - Correct letters will appear in their positions in the word
   - Wrong letters will be displayed in the "Wrong" section
   - Each wrong guess adds a body part to the hangman
4. **Win or Lose**:
   - **Win**: Guess all letters before the hangman is complete
   - **Lose**: The hangman is fully drawn (6 wrong guesses) and the secret word is revealed

## 🕹️ Game Controls

- **Any Letter Key**: Make a letter guess
- **Close Window**: Exit the game

## 📋 Requirements

- Python 3.6 or higher
- Pygame library

## 🚀 Installation & Setup

1. **Clone the repository**:
   ```bash
   git clone https://github.com/RhythmPahwa14/Hangman-Game.git
   cd Hangman-Game
   ```

2. **Install Pygame**:
   ```bash
   pip install pygame
   ```

3. **Run the game**:
   ```bash
   python hangman.py
   ```

## 🎮 Gameplay Screenshots

The game features:
- A gallows structure drawn in black
- Hangman figure drawn in light yellow/cream color
- Brown background for a classic feel
- Green instructions text
- Blue text for the current word progress
- Red text for wrong guesses

### Game Elements:
- **Gallows**: Base, pole, top beam, and noose
- **Hangman Parts** (drawn in order):
  1. Head (circle)
  2. Body (rectangle)
  3. Left arm (line)
  4. Right arm (line)  
  5. Left leg (line)
  6. Right leg (line)

## 📁 File Structure

```
Hangman-Game/
├── hangman.py          # Main game file with Hangman class
├── word.txt            # Word database (2,000+ words)
├── word.yaml           # Additional word data (if needed)
└── README.md           # This file
```

## 🔧 Game Mechanics

### Word Selection
- Words are randomly selected from `word.txt`
- Contains words of various lengths and difficulties
- Words are converted to lowercase for consistency

### Scoring System
- **Win Condition**: Guess all letters before 6 wrong attempts
- **Lose Condition**: 6 wrong guesses complete the hangman drawing

### Visual Elements
- **Window Size**: 400x500 pixels
- **Font**: Courier New, size 20
- **Frame Rate**: 60 FPS for smooth gameplay
- **Color Scheme**: 
  - Background: Brown (155, 120, 70)
  - Gallows: Black (0, 0, 0)
  - Hangman: Light cream (255, 253, 175)

## 🛠️ Technical Details

The game is built using object-oriented programming with a single `Hangman` class that handles:
- Game initialization and state management
- Word loading and selection
- User input processing
- Graphics rendering
- Game logic (win/lose conditions)

### Key Methods:
- `__init__()`: Initialize game state and graphics
- `_gallow()`: Draw the gallows structure  
- `_man_pieces()`: Draw hangman parts based on wrong guesses
- `_guess_taker()`: Process letter guesses
- `_right_guess()`: Handle correct letter guesses
- `_wrong_guess()`: Handle incorrect letter guesses
- `_message()`: Display win/lose messages
- `main()`: Main game loop

## 🤝 Contributing

Contributions are welcome! Here are some ways you can help:
- Add more words to the word database
- Improve the graphics and visual design
- Add sound effects
- Implement difficulty levels
- Add a scoring system
- Create additional game modes

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🎉 Enjoy Playing!

Have fun testing your vocabulary skills with this classic word game! Can you guess the word before the hangman is complete?