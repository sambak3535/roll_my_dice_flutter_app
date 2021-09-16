# RollMyDice

The application is a game, where the Player can press a button to "Roll a dice", and get a Random result anywhere between 1 and 6, the Player gets 10 chances to play, and every time the result of the dice roll should get added to the Player's score. After 10 attempts the player's results should be logged into the leaderboard.


Run
Run the applications:

$ flutter run
Runs the app in the connected device or emulator.

Testing
Run unit tests:

$ flutter test
Execute all unit test of the project


1. Add required libraries from pub.dev
2. Connect project in firebase console.
3. We are using the auth with the phone number so first step of verifying the mobile number would be the same for sign up or sign in. Afterwards if the user has not 
entered the details then the screen "Add user details" will pop otherwise not. User can edit his/her details anytime.
4. We will follow bottom navigation so there will be three tabs namely "RollDice", "LeaderBoard" and "Account".
5. We are using this(https://stackoverflow.com/questions/60461109/dice-roll-animation-flutter) reference for creating the dice animation.
6. While using the dice animation we will not use provider package but instead we will use flutter_riverpod as it will be easier.
7. While using the firestore we will make the simple file structure so that it can be easier to maintain and scale. There are three files 
7a. firestore_service: this file contains the boilerplate code for CRUD operation on collection or documents.
7b. firesbase_path: different paths for leaderboard and user details.
7c. firestore_database: Different methods for specific CRUD operations in firestores.

