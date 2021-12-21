# Code Guidelines
For reference, see the below guidelines we use for peer code review at Exodus.

## Git Hygiene
- Commits tend towards atomic (take care of a single thing)
- Commit messages are descriptive and follow the [seven rules of a great Git commit message](https://chris.beams.io/posts/git-commit/)
- Pull requests are atomic (take care of a single thing) and functional (don’t leave the program in a half-functioning state)
- Pull requests have proper description, mentioning the what and the why and (infrequently and if complex) the how, and include detailed test plans (steps + expected outcome)

## Functionality
- All task requirements are fully implemented, tradeoffs made are documented, explanations are provided for any missing pieces
- Not obviously broken
- No dubious functionality on top of the spec
- Not over-engineered, e.g., doesn’t prematurely optimize at the expense of complexity

## Quality
- Code is self-documenting: semantic variables names, function names describe implemented function
- Code is as simple as possible and modular
- Small single-purpose functions > giant functions that do 10 things
- Code is logically separated (e.g., no giant utils folders)
- Author uses objects, arrays, inheritance, closures, callbacks, promises expertly, and is up to date with the language/technology, e.g., async/- await > promise chains > callbacks for code after 2019
- Tests are included and:
    - Are readable (intent is clear)
    - Cover happy path
    - Cover edge cases