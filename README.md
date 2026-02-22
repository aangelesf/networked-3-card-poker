# Networked 3 Card Poker (JavaFX)

This project is a networked implementation of Three Card Poker built
using JavaFX and Java sockets. The application follows a client-server
architecture where the server manages all game logic, including
shuffling, dealing cards, comparing hands, and calculating winnings.
Clients connect to the server over TCP sockets and communicate using
serialized PokerInfo objects.

## System Architecture
The server runs on its own process and handles each client connection
on a separate thread. Core game logic is encapsulated in a ThreeCardLogic
class, while supporting classes such as Deck, Card, and PokerInfo manage
state and data transfer. The client and server are structured as
separate Maven projects.

## User Interface
The client uses JavaFX and consists of three scenes: a welcome screen
for entering the server IP and port, a gameplay screen for placing bets
and viewing cards, and a result screen that displays win/loss outcomes
and total winnings.

## Tools & Concepts Used
- Java
- JavaFX (multi-scene GUI)
- TCP sockets and object serialization
- Client-server architecture
- Multithreading
- UML-based design
