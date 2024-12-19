# Prompty

## Description
Prompty is a web-based prompt engineering trainer designed to help users practice and improve their prompt engineering skills. The goal of the game is to get the AI to say specific phrases as quickly as possible while adhering to certain rules and avoiding penalties.

## Features
- Interactive game interface
- AI-generated responses using OpenAI's GPT-3.5-turbo model
- Leaderboard to track high scores
- Real-time feedback and time tracking

## Installation
1. Clone the repository:
    ```sh
    git clone https://github.com/Captainexpo-1/Prompty.git
    cd Prompty
    ```

2. Install the dependencies:
    ```sh
    npm install
    ```

3. Create a `.env` file in the root directory and add your OpenAI API key:
    ```env
    OPENAI_API_KEY=your_openai_api_key
    PORT=3000
    ```

## Usage
1. Start the server:
    ```sh
    npm start
    ```

2. Open your browser and navigate to `http://localhost:3000` to start playing the game.

## How to Play
1. Click the "start" button to begin the game.
2. Type your prompts in the input area and press Enter.
3. The AI will respond to your prompts. Try to get the AI to say the target phrases listed on the right side of the screen.
4. Avoid using the target phrases in your prompts and avoid triggering penalty phrases to minimize your time.
5. Once all target phrases are found, enter your name to save your score to the leaderboard.

## Leaderboard
- The leaderboard displays the top scores in descending order.
- Scores are formatted as minutes and seconds.

## API Endpoints
- `GET /generate-text`: Generates AI responses based on previous messages.
- `GET /leaderboard/get`: Retrieves the current leaderboard data.
- `GET /leaderboard/add`: Adds a new score to the leaderboard.
- `GET /leaderboard/remove`: Removes a score from the leaderboard.
