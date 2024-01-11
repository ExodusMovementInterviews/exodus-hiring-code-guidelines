# Code and Process Guidelines

For reference, see the below guidelines we use for peer code review at Exodus. You can follow this checklist when evaluating a code challenge submission.

## Grading

See points in parentheses before each item. Negative points mean the candidate can only lose points for that item. The expected Total Score:

- Candidates should score a total of >15 points if they use PRs, >10 otherwise
- Colleagues should score a total of >20 points

## Code

> [!IMPORTANT]
> GRADING (SECTION SCORE)
>
> - Everyone should score at least 10 points

### Functionality

- [ ] (1) All task requirements are fully implemented
- [ ] (1) Not obviously broken
- [ ] (1) No dubious functionality on top of the spec
- [ ] (1) Not over-engineered, e.g., doesn’t prematurely optimize at the expense of complexity

### Code Quality

- [ ] (2) Code is readable: linted, prettified, and written in a consistent style
- [ ] (1) Code is self-documenting: semantic variables names, function names describe implemented function
- [ ] (1) Code is as simple as possible and modular
  - Small single-purpose functions are preferred to giant functions that do 10 things
  - Code is logically separated (e.g., no giant utils folders)
- [ ] (2) Author uses objects, arrays, inheritance, closures, callbacks, promises expertly, and is up to date with the language/technology, e.g., async/- [ ] await > promise chains > callbacks for code after 2019
- [ ] (1) Tests are included and:
  - Are readable (intent is clear)
  - Cover happy path
  - Cover edge cases

### Documentation

- [ ] (2) Clear instructions for project setup
- [ ] (-1) Clear code comments, but _only when necessary_. Comments are for the why, not the what

## Git Hygiene

> [!IMPORTANT]
>
> - Candidates should score at least 5 points in this section (or skip if not working with Pull Requests, e.g. in the context of a code challenge)
> - Colleagues should score at least 10 points in this section

- [ ] (1) Commits tend towards atomic (take care of a single thing)
- [ ] (1) Commit messages are descriptive and follow the [seven rules of a great Git commit message](https://chris.beams.io/posts/git-commit/)

If using Pull Requests:

- [ ] (1) Pull requests are atomic (take care of a single thing) and functional (don’t leave the program in a half-functioning state)
- [ ] (1) Pull requests have proper description, mentioning the what and the why and (infrequently and if complex) the how, and include detailed test plans (steps + expected outcome)
- [ ] (1) Knows how to rebase commits
- [ ] (1) Knows how and when to squash/fixup commits
- [ ] (1) Pull requests follow the Pull Request template in the repo (if one is present)
- [ ] (1) Knows how to create and maintain (through rebasing) a chain of related pull requests for easier review and merging (Bonus for candidates, requirement for colleagues)

## Code Reviews

_Note: naturally, this is only relevant if you're reviewing Pull Requests_

> [!IMPORTANT]
>
> Everyone should score at least 3 points in this section

- [ ] (2) Interaction between peers (author and reviewers) is civil, timely and open to suggestions
- [ ] (1) Does not nit-pick too much, or about things that should be covered by automated tools (like linters, formatters, etc.)
- [ ] (1) Aims to review the entire pull request and submit all comments at once instead of stopping at the first issue. If this is not possible, lets the author know that the review is a partial one (watch out, as this could be a sign that the PR is too big)
- [ ] (2) Correctly assesses whether the suggested changes are blocking or can be made in a separate pull request
