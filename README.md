# Concentration
Play a game of Concentration with a standard 52-card deck

Cards are cleared when the user flips two cards on the board and the selected cards 
have the same color suit and the same numeric value.

class Card {
  int value;
  String suit;

  Card(int v, String s) {
    this.value = v;
    this.suit = s;
  }
  
  Decks are represented through an ArrayList<Card>.
   ArrayList<Card> makeDeck(ArrayList<Integer> list1, ArrayList<String> list2) {

    ArrayList<Card> cards = new ArrayList<Card>();

    for (int i = 0; i < list1.size(); i = i + 1) {
      for (int j = 0; j < list2.size(); j = j + 1) {
        cards.add(new Card(list1.get(i), list2.get(j)));
      }
    }
    return cards;
  }
