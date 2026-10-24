# Satchel Math

Event bakery pretzel satchel, week, cost and time arithmetic. The 485 pretzels at 15 pretzels a satchel take 33 satchels, the last satchel holding 5 pretzels.

## Named constants

None. Every number is the owner's own entry.

## What it computes

- **The satchels truth** - the pretzels (1 to 1000000) divided by the pretzels a satchel (1 to 1000), rounded up, with what the last satchel holds.
- **The weeks truth** - the pretzels divided by the pretzels used a week (1 to 100000), with the pretzels left for the next week.
- **The cost truth** - the satchels (1 to 100000) times the satchel price ($0.01 to $999.99) to the cent, and spread over the pretzels, half rounded up.
- **The time truth** - the pretzels divided by the pretzels packed a minute (1 to 100), rounded up, in minutes and in hours and minutes.

## Boundary

Arithmetic only. Counting applied as written. It has not seen any pretzel, satchel or venue and does not know whether pretzels will really stay fresh, a supplier will run out or a price will hold, and it gives no verdict that a satchel is worth its price or a pretzel is right for an event. Every number is the owner's own entry.

## Files

- `index.html` - landing page with the boundary and starting examples.
- `app.html` - the calculator; every satchel recomputes on each keystroke.
- `engine.js` - the four truths, shared by the page and the tests.
- `oracle.py` - an independent Python re-implementation; writes `expected.json`.
- `test.js` - runs the engine against `expected.json` (99 cases, 20 error cases).

## Tests

```
python3 oracle.py
node test.js
```
