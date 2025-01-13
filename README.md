# RPS-AI-Showdown-Server

RPS-AI-Showdown-Server is the backend server for the RPS-AI-Showdown application which can be found here: https://github.com/GChana/RPS-AI-Showdown,
facilitating AI string responses for the outcome of the Rock-Paper-Scissors game.

## Installation

To set up the project locally, follow these steps:

1. **Clone the repository**:

   ```bash
   git clone https://github.com/GChana/RPS-AI-Showdown-Server.git
   cd RPS-AI-Showdown-Server
   ```
2. Install dependencies:

Ensure you have Node.js installed. Then, run:

``` bash
npm install
```

3. Start the server:

``` bash
npm start
```

The server should now be running, ready to handle requests from the RPS-AI-Showdown application.

## Usage
This server is designed to work in conjunction with the RPS-AI-Showdown frontend application. Ensure the frontend is configured to communicate with this server's address and port.

## API Endpoints

The server exposes the following endpoints:

GET /revenge: Generates a string response where the AI opponent has lost a game of rock, paper, scissors and vows revenge
GET /taunt: Generates a string response where the AI opponent has won a game of rock, paper, scissors and taunts the player
GET /welcome: Generates a string response where the AI opponent welcomes the player to the game

- Request body:

```json
  `${API}/revenge/${currentOpponentFormatted}?userName=${encodeURIComponent(
        userName
      )}`
```

- Response:

```json
  `By the beard of Zeus ${userName}, your scissors have defeated my paper` 
```


##Contributing
Contributions are welcome! To contribute:

1. Fork the repository.

2. Create a new branch:

```bash
git checkout -b feature/YourFeatureName
```

3. Make your changes.

4. Commit your changes:

```bash
git commit -m 'Add some feature'
```

5. Push to the branch:

```bash
git push origin feature/YourFeatureName
```

6. Open a Pull Request.

Contact
For questions or feedback, please reach out to https://github.com/GChana.
