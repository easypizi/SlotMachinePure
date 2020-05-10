Create a slot machine simulation web-app running under Google Chrome.

_Detailed description_
Slot machine page has following interface elements: 1. reels

2. pay-table
3. balance indicator (text-box)
4. SPIN button. 5. Debug area

_Reels_
Slot machine has 3 reels, each having following 5 symbols in order: 3xBAR, BAR, 2xBAR, 7, CHERRY
Only part of the reel is visible to user. There are horizontal win-lines on visible part of reel: top, center, bottom.

A reel can stop only in fixed positions. A stopped reel has either:

1. a symbol on center win line
2. symbols on top and bottom win-line positions
   Note, that if center win-line has a symbol, bottom/top parts of peer symbols must be still visible.

_Pay-table_
Pay-table must indicate winning combinations and payouts as: 3 CHERRY symbols on top line | 2000
* 3 CHERRY symbols on center line | 1000
* 3 CHERRY symbols on bottom line | 4000
* 3 7 symbols on any line | 150
* Any combination of CHERRY and 7 on any line | 75
* 3 3xBAR symbols on any line | 50
* 3 2xBAR symbols on any line | 20
* 3 BAR symbols on any line | 10
* Combination of any BAR symbols on any line | 5

When a particular win happens the winning sum on pay-table must start blinking.
Also, the win-line on reels must be marked (for example a red line).

_Balance area_
Players current balance is shown on balance text-box. For debugging purposes, it is permitted player enter integer to balance box in range 1...5000.

_Spin button_
Press on SPIN button start spinning of all three reels. Each spin costs player 1 coin. During the reel spinning player can not do anything else than wait. The spinning must last 2 seconds, after that reels start to sop one by one (starting from left) having 0.5 sec delay between landings.

_Debug area_
It must be possible use the slot machine in two modes: random and fixed. In case of random mode, the reels must land random positions. For fixed mode, the player must able enter two parameters for each reel. These input parameters are:

1. a symbol from set {BAR, 2xBAR, 3xBAR, 7, CHERRY}
2. landing position of the symbol from set {top, center, bottom}
   If fixed mode is active, the reels must land as specified by tester.

_General guidelines_
If you find any unspecified aspect in the description, you are welcome to solve using common sense and mention it in your release comments. The visual implementation must definitely have a spinning reel effect. Note, that the requirements above are MINIMAL ones and you are free to add features for exposing your skills on wider range. You can use any external frameworks/libraries and CSS techniques as long the application works under Google Chrome. We value code legibility/sustainability over optimization/quick hacks.

_Provided assets_
You must use the reel symbol graphics provided with the task. Though, you are free to modify/combine the files as needed.

_Packaging requirements_
The release must contain
• index.html as main launch-page of the application
• readme.txt with general comments/design principles or whatever seems important
• _.js/_.css/\*.png/etc files of whatever needed for the app

---

HARDCORE MODE:

---

1. use as less code as you can, try to build abstractions.
2. OOP patterns high priority.
3. 5 reels and cross-diagonal combinations.
4. Animations effects on the win.
5. Infinite recurse.
6. Canvas use or any external library.
7. No frameworks, Vanilla js only.
8. ES6 > (f.e. use generator functions if u need or spread and etc).

---
