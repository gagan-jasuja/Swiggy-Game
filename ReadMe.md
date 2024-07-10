# Swiggy Game

Swiggy Game is a simple game where players fight in turns using their health, strength, and attack attributes. The game is implemented using Spring Boot.

## Requirements

- Java 22
- Maven

## Installation

1. Clone the repository:
   ```sh
   git clone github.com:gagan-jasuja/Swiggy-Game.git
   cd SWIGGY-GAME
2. Build the project: mvn clean install
3. Run the application: mvn spring-boot:run

Usage
Once the application is running, you can interact with it using cURL or any REST client like Postman.

### Creating Players

1. Create Player A:
    ```sh 
    curl -X POST http://localhost:8080/players -H "Content-Type: application/json" -d '{"health":50,"strength":5,"attack":10}'

2. Create Player B:
    ```sh
    curl -X POST http://localhost:8080/players -H "Content-Type: application/json" -d '{"health":100,"strength":10,"attack":5}'

3. Starting the Game: Start a game between Player A (ID 1) and Player B (ID 2):
    ```sh 
    curl -X GET http://localhost:8080/players/start/1/2

### POST /players
Request Body:

    {
       "id":1,
       "health": 50,
       "strength": 5,
       "attack": 10
    }

For more examples and results 
Check Some Output folders.


