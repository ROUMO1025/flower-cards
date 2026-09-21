# Flower Cards V3.0 — Single-card climbing

## Setup and objective
2–4 players act clockwise, with a random starting player. The 42 action cards are A–10 in four suits plus the Big and Small Jokers. The 12 role cards are J/Q/K in four suits; each player has one public role and only its suit matters. Deal 24 action cards one at a time, starting with the first player: 12/8/6 per player in a 2/3/4-player game. The other 18 form the shared discard/reserve pool.

Play at most one main card per action. The first player with no cards AFTER all mandatory effects wins immediately. There is no automatic draw, attached discard, bonus discard, matching-rank response, draw result, or official turn limit.

## Climbing
Every ordinary card must strictly exceed the most recent ordinary main card in the current sequence. A=1; 10 is highest. Equal ranks cannot be played. Opening or reopening a sequence has no rank restriction.

Jokers may always be played alone for their skills. They do not change the ordinary reference rank or its owner. After a Joker, the next ordinary card must still beat that reference. With no ordinary reference yet, any ordinary rank is allowed.

If no legal card (including a Joker) is available, keep your hand and pass. Other players still try in order. If everyone else fails to play a higher ordinary card, the last highest ordinary card's owner leads again and the rank restriction clears. A suppressed turn counts as failing to beat the reference. Passing voluntarily when a legal card exists is forbidden.

## Effects relative to your role
Red suits: hearts/diamonds. Black suits: spades/clubs.

- Same color, different suit: simply play one card.
- Native (exactly the same suit): choose ONE of changing the next player's role or, if eligible, suppressing that next player.
- Opposite color: after playing, draw 1 for an odd rank or 2 for an even rank. A is odd. This is mandatory.

Changing the next role affects only the next clockwise player. Choose a different suit with an available role card. Take the first card of that suit from the role deck and return the old role to the end. This does not exchange hands.

Suppression is legal only if the next player's role color, at the instant of play, is opposite to the native main card. That player skips their next entire action and recovers. Suppression does not also change their role, allow a matching-rank response, or stack. The marker belongs to the player and never moves with exchanged hands.

Draw uniformly at random from the shared pool. If insufficient, take all available cards; an empty pool gives zero. The main card is pending and cannot be drawn back during its own effect. Check for victory only after drawing.

## Jokers
Big Joker: remove it first, then exchange your entire remaining hand with an opponent who has the fewest cards. Choose among tied opponents. Do not exchange roles, seats, turn ownership or suppression markers. The Joker itself is not exchanged. If it was your only card before playing, do not exchange: you win normally.

Small Joker: remove it, then change your own role to an available different suit using the same role replacement procedure. It grants no additional discard or draw. Even as your last card, complete the role change before checking victory.

## Resolution and information
Choose a legal main card and all required choices → move it to pending → resolve draw, role change or hand exchange → check victory → recycle the main card → if no winner, advance clockwise, consume suppression skips and check for a new lead.

You cannot undo after seeing random results. Drawn cards append to the right. Sorting is allowed and does not consume an action or trigger effects. A whole-hand exchange preserves each hand's current order.

Hands + pool + pending always contain exactly 42 unique action cards. Active roles + role deck always contain exactly 12 role cards, never mixed with actions. Recent cards and the climbing reference are records, not additional physical piles.

Roles, hand counts, available role counts, pool size, climbing reference, suppression and action logs are public. Opponent hands and the pool's contents are hidden. Local heuristic AI receives only its own hand and public information; reveal-all debugging does not expand its access.

## Version notes
V3 replaces attached discards with single-card climbing, adds native role-change/conditional next-player suppression, requires odd/even opposite-color draws, and permits sorting. V2 target-any-player suppression and matching-rank responses are removed. Save format remains version 6; old rule saves require their matching old prototype. Language switching changes presentation only. Simulation limits are test timeouts, never a game draw rule.
