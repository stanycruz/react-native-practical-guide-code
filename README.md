# Guess My Number

A React Native game built with Expo as part of the **React Native - The Practical Guide** course.

The goal of the game is simple: the player chooses a number between **1 and 99**, and the device tries to guess it. After each guess, the player indicates whether the correct number is higher or lower until the device finds the selected number.

## Features

- Number selection and validation
- Custom reusable UI components
- Custom primary buttons with press feedback
- Higher and lower guess controls
- Random number generation with dynamic boundaries
- Guess validation to prevent contradictory hints
- Game round tracking
- Scrollable guess history with `FlatList`
- Game over screen with round summary
- Restart game flow
- Multiple screens controlled through React state
- Native alerts for invalid input and game feedback
- Safe area support with `react-native-safe-area-context`
- Linear gradient and image backgrounds
- Custom fonts with `expo-font`
- Splash screen handling with `expo-splash-screen`
- Vector icons with `@react-native-vector-icons`
- Reusable colors and shared styling constants

## Concepts Practiced

This project was focused on practicing fundamental React Native and React concepts, including:

- Core React Native components
- Component composition
- Reusable UI components
- Props and `children`
- React state with `useState`
- Side effects with `useEffect`
- Conditional rendering
- Controlled inputs
- Flexbox layouts
- Platform-specific styling concepts
- Styling with `StyleSheet`
- Custom fonts
- Images and image backgrounds
- Linear gradients
- Lists with `FlatList`
- Native alerts
- Custom buttons with `Pressable`

## Project Structure

```text
.
├── assets/
│   ├── fonts/
│   └── images/
├── components/
│   ├── game/
│   │   ├── GuessLogItem.js
│   │   └── NumberContainer.js
│   └── ui/
│       ├── Card.js
│       ├── InstructionText.js
│       ├── PrimaryButton.js
│       └── Title.js
├── constants/
│   └── colors.js
├── screens/
│   ├── GameOverScreen.js
│   ├── GameScreen.js
│   └── StartGameScreen.js
├── App.js
└── index.js
```

## Game Flow

```text
StartGameScreen
       ↓
Select a number
       ↓
   GameScreen
       ↓
Higher / Lower
       ↓
Device finds the number
       ↓
 GameOverScreen
       ↓
Start New Game
```

## Running the Project

Install the dependencies:

```bash
npm install
```

Start the Expo development server:

```bash
npx expo start
```

Then run the application on an Android emulator, iOS simulator, or compatible development device.

## Purpose

This project was created for learning and practicing React Native fundamentals.

It intentionally focuses on core concepts before introducing more advanced navigation, responsive layouts, device orientation handling, and platform-specific adaptations in later sections of the course.
