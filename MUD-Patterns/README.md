MUD Patterns Homework - Singleton & Adapter

Overview

This project demonstrates the use of Singleton and Adapter design patterns in the context of a MUD (Multi-User Dungeon) game. The implementation includes:

ConfigurationManager (Singleton): Ensures a single instance of the configuration manager for global settings.

ChatServiceAdapter (Adapter): Integrates a legacy chat system with a new chat interface.

Project Structure 
MUD-Patterns
│── src
│   ├── config
│   │   ├── ConfigurationManager.java
│   │   ├── ConfigManagerDemo.java
│   ├── chat
│   │   ├── LegacyChatService.java
│   │   ├── ChatService.java
│   │   ├── ChatServiceAdapter.java
│   │   ├── ChatAdapterDemo.java
│── README.md
│── .gitignore
Part 1: Global Configuration Manager (Singleton)

Implementation

The ConfigurationManager class:

Loads a set of hardcoded key-value pairs as configuration settings.

Ensures only one instance exists using lazy initialization.

Provides methods to retrieve and print configuration settings.
Example Data 
maxPlayers → "100"
defaultLanguage → "en"
gameDifficulty → "medium"
 Expected Output 
 maxPlayers: 100
defaultLanguage: en

All Configurations:
maxPlayers → 100
defaultLanguage → en
gameDifficulty → medium
Part 2: Chat Service Adapter (Adapter)

Implementation

The ChatServiceAdapter class:

Wraps the LegacyChatService.

Adapts the method sendMessage(String message) to call sendLegacyMessage(String msg) from the legacy system.
Expected Output 
Legacy Chat: Hello world! 
Setup & Run Instructions

Clone the Repository
git clone https://github.com/YOUR_GITHUB_USERNAME/MUD-Patterns-Homework.git
cd MUD-Patterns
Contribution

Feel free to fork the repository and submit pull requests.

License

This project is open-source and free to use
