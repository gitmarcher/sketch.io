# Sketch.io 🎨

<div align="center">

![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![NodeJS](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white)
![Express.js](https://img.shields.io/badge/Express.js-404D59?style=for-the-badge)
![Socket.io](https://img.shields.io/badge/Socket.io-010101?style=for-the-badge&logo=socket.io&logoColor=white)

</div>

Sketch.io is a collaborative drawing and guessing game where users can create rooms, invite friends, and play a game similar to *Scribble.io*. The main objective is for one player to draw a chosen word while other players guess the word through chat. Unique features include reconnection support and a points retention system to enhance the gaming experience.

## Features

- **Create and Join Rooms**: Set up a private room and invite friends to play
- **Drawing and Guessing Game**: The drawer selects a word from three options and sketches it on a canvas; other players guess the word in real-time
- **Intelligent Chat Feedback**: Guesses appear in the chat with color indicators based on closeness to the correct word; correct guesses are hidden for suspense
- **Reconnection Support**: If a player disconnects, they have 2 minutes 30 seconds to reconnect without losing points

## Tech Stack

- **Frontend**
  - React
  - Tailwind CSS
  - HTML5 Canvas (for drawing)
- **Backend**
  - Node.js
  - Express.js
  - Socket.IO (for real-time communication)

## Installation

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/sketch.io.git
cd sketch.io
```

### 2. Install Dependencies
```bash
# Backend
cd backend
npm install

# Frontend
cd ../frontend
npm install
```

### 3. Environment Setup
Set up the `.env` files in both `backend` and `frontend` directories with the necessary environment variables, such as server URLs and API keys.

### 4. Run the Application
- Start the backend server:
  ```bash
  cd backend
  npm start
  ```
- Start the frontend server:
  ```bash
  cd ../frontend
  npm start
  ```
- Open [http://localhost:3000](http://localhost:3000) to play the game locally

## How to Play

1. **Create or Join a Room**
   - The host creates a room and shares the room ID with friends

2. **Game Start**
   - The host starts the game
   - One player becomes the drawer and picks a word to draw

3. **Guessing**
   - Players guess the word in the chat
   - Chat colors guide them on the closeness of their guesses

4. **Reconnection Support**
   - If disconnected, players have 2 minutes 20 seconds to reconnect without losing their score
