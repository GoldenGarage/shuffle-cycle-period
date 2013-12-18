shuffle-cycle-period
====================

A simple Node.js tool that calculates the "shuffle cycle period" for a specified number of cards.

    shuffle-cycle-period {numberOfCards}

Calculate the Shuffle Cycle Period for a specific number of cards.

  * `{numberOfCards}` - the number of cards in the deck to be shuffled.

The Shuffle Cycle is defined as

While holding the deck:
  - step 1. Take the top card off the deck and set it on the table.
  - step 2. Take the next card off the top and put it on the bottom of the deck in your hand.
  - step 3. Continue steps 1 and 2 until all cards are on the table.  This is a round.

The Shuffle Cycle Period is the number of rounds required to return to the original order.

  - step 4. Pick up the deck from the table and repeat steps 1-3 until the deck is in the original order.

This command line tool shuffles a deck with the specified `{numberOfCards}` once. And then, counts how many times
it takes *using the same shuffle pattern* to return the deck of cards to its original order.
