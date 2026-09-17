# Guessing Game

This is a simple guessing game implemented in Rust. The player has to guess a randomly generated number

Its part of the [Rust programming language's learning resources](https://doc.rust-lang.org/book/ch02-00-guessing-game-tutorial.html#setting-up-a-new-project) and is designed to help beginners understand basic concepts such as variables, loops, conditionals, and user input.

## Requirements

A Rust toolchain (edition 2024, so Rust 1.85 or newer). If you don't have it yet, install it with [rustup](https://rustup.rs):

```sh
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

## Running the game

From the project root:

```sh
cargo run
```

Cargo downloads the `rand` dependency, builds the project, and starts the game.

For an optimised build:

```sh
cargo run --release
```

## How to play

The game picks a secret number between 1 and 100 and keeps asking for a guess until you get it right:

```
Guess the number!
Please input your guess.
50
You guessed: 50
Too big!
Please input your guess.
25
You guessed: 25
Too small!
Please input your guess.
37
You guessed: 37
You win!
```

Anything that isn't a whole number is ignored and the game simply asks again. Press `Ctrl+C` to quit early.

## Other useful commands

```sh
cargo build   # compile without running
cargo check   # type-check quickly, without producing a binary
cargo fmt     # format the source
```
