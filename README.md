# Menagerie

A generalized Trading/Collectible Card Game or a group of exotic animals kept in
captivity for exhibition.

## Thoughts

Cards are components

The game should offer to support a single simple ownership model.

## Component ownership model

*A way to have a stable card price*
A card owner is one who has sent more than X DAI into the cards bond
* The card always costs 10 DAI, but if you buy early you get more bond tokens.
* Maybe if a player sells some amount of those tokens, they "sell" the card.
* Maybe When a card is baught, an NFT is created with a base price locked to the
  price at the time. If the owner ever sells any of their bond tokens at or
  below that price, they've "sold" the card. They can sell all but their last
  base token above that price and still keep the card.

*Simpler ownership model*
* for each multiple of x of the bond you hold you own one copy of the card

*Simple and stable*
* Card ownership is buying an NFT for a fixed DAI price
* the NFT contract buys and burns some fixed value of bond tokens when minting
  an NFT
* Or the NFT contract buys and holds the bond tokens and will exchange
  them for the NFT at any time

*A way to sell packs*
Probaby sell packs of formats, the utility of packs is both gambling
(how?) and drafting game modes. A magic drafting format needs a list
of cards and a set of rarities. Cards should be able to be rare in
some formats but common in others, this shoudl be specified in the
format configuration

* Packs as NFT.
* A contract to exchange NFTs for cards.
  * The NFT contract buys some fixed amount of the cards bond when
    those cards show up in packs.
  * Or the contract buys an equal portion of the entire formats cards.
  * Should probably also buy some of the foramt itself

## Game licence model

same as component ownership model?

## Game design

Should strive to capture the magic of the classic TCGs.

Should have room to design cards for Tammy, Jenny, and Spike.

The philosophy of fire should apply

## Player interaction/interruption

Hearthstone secrets are juvinial
Magic instants are infeasible

What's something that's feasible and interesting?

*Prediction is fun*
The theory is that guessing right and gaining advantage feels good.
It also punishes booring rote play, and encourages variety in play and
deckbuilding

On your turn you can save mana, and set conditions on a reaction card that will
automatically be played if and when those conditions are met by your opponent.

for example:
* Play this when they play anything
* Play this when they play a creature
* Play this when they attack with an elf
* Play this when they destroy my wall
* Play this on the second reaction they play

### Expectations

*Bluffing*
* Holding back mana for a counter when you don't have it

*Creature combat*
* Attacking (and defending?)

*Combos*
* What fundamental game rules make it possible to develop formats with
  combos?
  * Triggered events
  * The ability for a definition to increase any resource, including
    actions, cards in hand, etc.
* Tools to limit combos
  * hooks to limit the above
  * like slay the spire "draw 4, you cannot draw more cards this turn"
    or "gain 2 energy, you can only draw 3 cards this turn"

*Resource management*
* typed Mana
* typed Cards
* Attacks/phases per turn
* typed counters (poison, +1/+1, Foobar)
  * How can these be designed by players after the game is built?

*Named Abilities*
Like First Strike, Infect, Exalted, etc. How can these be designed by
players after the game is built? are these a second component type? If
so format designers would need to make sure they had exactly one
definiton of each named ability any of the cards in their format
mentioned. This named abstraction is probably a general pattern that
lots of games will want.

*Zones*
* Deck
* Hand
* In play
* Discard
* Removed from the game

*Player interaction*
* interruption
* reaction
* bluffing
* descruction
* offence vs defence
