# Contributing to rl-lang

Thanks for stopping by. Every repo in this org runs on the same loop:
small focused changes, verified before you push, lowercase terse commits.

If a repo has its own CONTRIBUTING.md (like `rl-lang` does), that file
wins for that repo. This one is the fallback for everywhere else.

## What goes where

- Language, stdlib, toolchain: [rl-lang](https://github.com/rl-lang/rl-lang)
- Docs and reference: [the-book](https://github.com/rl-lang/the-book)
- Small programs and snippets: [rl-examples](https://github.com/rl-lang/rl-examples)
- Editors, packaging, CI actions: their own repos (see the org profile)

If you are unsure, open the issue in `rl-lang` and we will move it.

## Before you push

1. `rl check` and `rl test` on anything you touched.
2. `rl format` on changed `.rl` files (Allman style, 4 spaces).
3. For `rl-lang` itself: `cargo test --all-features` plus clippy with
   `-D warnings`.
4. Plain ASCII in prose and comments. No emojis unless the task asks.

## Commits

- Lowercase, terse, one idea per commit (`add x`, `fix y`, `docs z`).
- Sign with `git commit -S`.
- One PR per idea; small PRs merge faster than big ones.

## Issues

Use the templates: bug reports need the RL version (`rl --version`),
the smallest reproducing file, and expected vs actual behavior.
Feature requests need the problem first and the shape second.

## License

By contributing you agree your work lands under the repo's license
(MIT or Apache 2.0 at the project's option). No per-file headers needed.
