# 3D Reaction Timer

A fun, interactive reaction time game built with **Three.js** and vanilla JavaScript. Test your reflexes by clicking a 3D shape as quickly as possible when it turns blue.

## Features

- **3D Graphics**: Beautiful rotating dodecahedron rendered with Three.js
- **Smooth Animations**: Color transitions, scaling pulses, and shake effects
- **Game States**: Idle, waiting, ready, result, and error states with visual feedback
- **Performance Tracking**: Tracks attempts, best time, and average reaction time
- **Responsive Design**: Works seamlessly on desktop and mobile devices
- **Modern UI**: Clean, dark-themed interface with smooth transitions

## How to Play

1. Click the **"Start Game"** button
2. Wait for the shape to turn blue and see the **"CLICK NOW!"** message
3. Click the shape as fast as you can to measure your reaction time
4. Your reaction time is displayed at the top right of the game area
5. Click **"Play Again"** to try again and improve your score

⚠️ **Note**: Clicking before the shape turns blue counts as an early click and shows an error message

## Game Mechanics

### Game Phases
- **Idle**: Initial state, waiting for the player to start
- **Waiting**: Waiting period (2-5 seconds) before the stimulus appears
- **Ready**: Shape is blue and ready for clicking
- **Result**: Shows reaction time after a successful click
- **Error**: Triggered when clicking too early

### Shape States
- **Gray** (Waiting): Neutral color while waiting for the stimulus
- **Blue** (Ready): Ready to click - this is when you should click
- **Green** (Success): Confirmation of successful reaction with pulse animation
- **Red** (Error): Visual feedback for early clicks with shake animation

### Statistics
- **Attempts**: Total number of tries
- **Best Time**: Your fastest reaction time
- **Average**: Average reaction time across all attempts

## Technical Stack

- **HTML5**: Structure and layout
- **CSS3**: Styling with modern features (grid, flexbox, transitions)
- **JavaScript (Vanilla)**: Game logic and state management
- **Three.js**: 3D rendering and animation
- **Fonts**: Inter and JetBrains Mono from Google Fonts

## Browser Requirements

- Modern browser with WebGL support
- JavaScript enabled
- Minimum screen width of 320px (mobile responsive)

## File Structure

```
reaction-game/
├── index.html       # Complete game implementation (HTML, CSS, JavaScript)
└── README.md        # This file
```

## Key Implementation Details

### Three.js Setup
- Perspective camera with 16:9 aspect ratio
- Dodecahedron geometry with wireframe overlay
- Multiple lighting sources for depth and visual interest
- Smooth animation loop with requestAnimationFrame

### Game State Management
- Centralized state object tracking game phase, timing, and statistics
- Event-driven architecture with clear separation of concerns

### Color Animation
- Smooth easing transitions between shape colors
- Different animation speeds based on game state

### Responsive Design
- Adaptive canvas size based on viewport
- Mobile-optimized layout with adjusted typography
- Touch-friendly click targets

## Performance Considerations

- Efficient requestAnimationFrame-based animation loop
- Debounced window resize handling
- Optimized Three.js rendering with proper aspect ratio management
- Hardware acceleration via WebGL

## Future Enhancements

- Local storage for persistent high scores
- Sound effects for game events
- Difficulty levels (multiple shapes, time pressure)
- Leaderboard functionality
- Different shape options
- Multiplayer comparison mode

## License

Feel free to use, modify, and share this project!
