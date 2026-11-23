<img width="457" height="582" alt="Screenshot 2026-11-23 at 6 10 39 PM" src="https://github.com/user-attachments/assets/b414c746-717a-4a9c-969c-117de0e0ceba" /> # CS3SY26_ProjectProposal by Aline Teresa Mendoza from CS Unit of PSHS


## Project Proposal Template:
cvbbbc
### Project Title or Name of the Application	: BlackJack CHAGOAD edition
### Section			   	      : 9 - Rubidium
### Group Members			    : ABAD, Shan Mikael Jorelle R., CHAVEZ, Zachary Karl N., GO, Keith Ashton L.
### Date (Proposal Date)  : Nov 5, 2026

### Project Description: BlackJack CHAGOAD edition, a simple game of blackjack, this includes two players, the dealer which you have to go against for the closest or the exact number of a blackjack (21) . It is a different edition because it includes the CHAGOAD card which allows you to exchange one already held card for another random card from the deck.

- A brief summary of the project description and the need for it.

- Describes system components, features, and expected outputs clearly and logically. NOTE: Clearly described the elements(classes), their attributes and methods and how they will interact with each other.
Card class:
 Represents ordinary cards
  Attributes:
   suit: The suit of the card (Hearts, Diamonds, Clubs, Spades).
   rank: The rank of the card (Ace, 2–10, Jack, Queen, King).
   value: The numerical value of the card.
  Methods:
    display_card(): Displays the card's rank and suit.
    get_value(): Returns the numerical value of the card.

SpecialCard Class:
Represents the additional CHAGOAD Card, which has a unique ability that allows its holder to exchange one card in their hand for another card from the deck.
  Attributes:
    name: The name of the special card (CHAGOAD Card).
    value: Its numerical value, which is 0.
    effect: Describes its ability to exchange one card for another.
  Methods:
    activate_effect(): Activates the card's ability to exchange one card in the holder's hand.
    get_value(): Returns the card's numerical value.
    
Deck Class
 Manages all the ordinary cards and the special CHAGOAD Card.
 Attributes:
   cards: A list containing the 52 ordinary playing cards and the additional CHAGOAD Card.
 Methods:
   create_deck(): Creates a standard deck of 52 cards and adds the CHAGOAD Card.
   shuffle_deck(): Randomizes the order of all 53 cards.
   deal_card(): Removes and returns a card from the deck.
   
Player Class
  Represents the person playing against the dealer.
 Attributes:
   name: The player's name.
   hand: A list containing the cards currently held by the player.
   score: The total numerical value of the cards in their hand.
 Methods:
   draw_card(): Receives a card from the deck.
   calculate_score(): Calculates the total value of the cards in the player's hand.
   display_hand(): Displays the player's cards and current score.
   use_special_card(): Allows the player to activate the CHAGOAD Card's ability and exchange one card in their hand.
   
Dealer Class
   Represents the dealer who competes against the player.
 Attributes:
   hand: A list containing the cards currently held by the dealer.
   score: The dealer's total numerical card value.
 Methods:
   play_turn(): Allows the dealer to draw cards according to the game's rules.
   calculate_score(): Calculates the dealer's total card value.
   display_hand(): Displays the dealer's cards and current score.
   use_special_card(): Allows the dealer to activate the CHAGOAD Card's ability and exchange one card in their hand.
   
BlackjackGame Class
   Manages the overall gameplay and interactions between the player, dealer, and deck.
 Attributes:
   deck: The deck used for the current round.
   player: The player participating in the game.
   dealer: The dealer competing against the player.
   game_status: Indicates whether the game is ongoing, won, lost, or tied.
 Methods:
   start_game(): Initializes the game, shuffles the deck, and deals the starting cards.
   player_turn(): Allows the player to draw another card, stay, or use the CHAGOAD Card.
   dealer_turn(): Controls the dealer's actions according to the game's rules.
   determine_winner(): Compares the player's and dealer's scores to determine the outcome.
   end_game(): Displays the final results of the round.

Interaction Between Classes
The BlackjackGame class manages the entire game by creating the Deck, Player, and Dealer objects. The Deck contains the ordinary Card objects and the additional SpecialCard object. It distributes cards to the player and dealer through its deal_card() method.

The Player and Dealer classes keep their own hands and add their scores using the values provided by the Card and SpecialCard classes. When either draws the CHAGOAD Card, they may activate its special ability to exchange one card in their hand for a new card from the deck. The BlackjackGame class manages the turns and decides the winner based on the final scores.

Main Features
- Standard Blackjack gameplay against a dealer.
- A 53-card deck containing 52 ordinary cards and one CHAGOAD Card.
- A special card ability that allows its holder to exchange one card for another.
- Automatic score calculation.
- Bust detection when a hand exceeds 21.
- Winner determination based on the final scores.
- Display of the player's and dealer's cards and scores.
Expected Outputs
At the end of each round, the application will display:
- The player's cards and total score.
- The dealer's cards and total score.
- Whether the CHAGOAD Card was drawn and whether its ability was activated.
- Whether either participant went over 21.
- The final result: player wins, dealer wins, or a tie.

- Include the description as well of your target demographics as the user of your application.
  
The target users of Blackjack CHAGOAD Edition are students for statistics and casual card game players, particularly those who enjoy simple games with strategy, decision making, and probability understanding. The application is designed for beginners who want an easy to understand Blackjack experience with an additional gameplay feature.

- The description is then followed by the class diagram, depicting clearly what was described.
Google drive link to image of the class diagram:
https://drive.google.com/file/d/1DMB-_N42dn2fNdjuk_RaOZkhxRTR7NWI/view?usp=sharing


**Sample class Diagram from https://static.visual-paradigm.com/web/images/tutorials/class-diagram-tutorial/01-class-diagram-example.png:**

![Sample Diagram](https://static.visual-paradigm.com/web/images/tutorials/class-diagram-tutorial/01-class-diagram-example.png)

### Goals:

The long-term goal of Blackjack CHAGOAD Edition is to develop a fun type of Blackjack application that provides entertainment and learning while introducing a new gameplay mechanic using the CHAGOAD Card. The project’s goal is also to strengthen the developers' understanding of Object Oriented Programming by applying concepts such as classes, objects, attributes, methods, and relationships in a functional program.

Objectives:

Objective 1: Make a functional Blackjack game that allows a player to compete against a dealer using the standard rules of Blackjack.
Objective 2: To create a unique CHAGOAD Card ability that allows its holder to exchange one card in their hand for another card from the deck.
Objective 3: Create an application that can be applied to see how probability can work in real life action. The CHAGOAD card adds the feature of “with replacement” aspect of probability as well.
Objective 4: Make the application not only entertaining but also help students understand the actual rarity of certain events rather than it being displayed in just numbers or percentages.


[Click here for Rubrics and Sample projects](https://docs.google.com/document/d/1xKd1CqK6DcNWS2_oJPBNtY5n3I3Hqiw8FY3W295Iqfk/edit?usp=sharing)
