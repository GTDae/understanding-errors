# Understanding Errors — MDN Troubleshooting Exercise

The Odin Project, Foundations, [Understanding Errors](https://www.theodinproject.com/lessons/foundations-understanding-errors) lesson.

Real starter file pulled from MDN's own repo ([`number-game-errors.html`](https://github.com/mdn/learning-area/blob/main/javascript/introduction-to-js-1/troubleshooting/number-game-errors.html)) — a number-guessing game with four intentional bugs. Each bug gets its own commit: baseline broken file first, then one fix per commit, in the order MDN's guide walks through them.

## The four bugs
1. `guessSubmit.addeventListener(...)` — method name wrong case (should be `addEventListener`)
2. `document.querySelector("lowOrHi")` — missing the `.` class selector, so it never matches the `<p class="lowOrHi">` element
3. `resetButton.addeventListener(...)` — same case bug as #1, on the reset button
4. `Math.floor(Math.random()) + 1` — `Math.random()` always floors to 0 before the `+ 1`, so the "random" number is always `1`. Needs `Math.random() * 100` first.
