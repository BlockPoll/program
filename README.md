# BlockPoll Solana on-chain program

This repository contains source code of BlockPoll on-chain program (smart contract).

- The program is deployed on Solana `devnet` cluster.
- Program Address: [GnS5xMqf5NaY7HgbwFneyLNktT8NNNKi4rA2JEmnYdzi](https://explorer.solana.com/address/GnS5xMqf5NaY7HgbwFneyLNktT8NNNKi4rA2JEmnYdzi?cluster=devnet)

---

## Build and deploy

Requires [Rust](https://www.rust-lang.org/) and [solana-cli](https://docs.solana.com/cli/install-solana-cli-tools) installed.

### Compile code

```sh
$ cargo build-bpf --manifest-path=./Cargo.toml --bpf-out-dir=./dist/program
```

### Deploy

```sh
$ solana program deploy dist/program/blockpoll.so
```

### Run tests

```sh
$ cargo test
```

---

## About BlockPoll

BlockPoll is a blockchain-based polling application where users can create polls, cast votes on polls, view poll results and share polls.

## Web Application

The application is live and hosted at [https://blockpoll.io](https://blockpoll.io).
Web application source code is available on [GitHub](https://github.com/BlockPoll/web).

## Author

Authored by [Rijul Gulati](https://github.com/RijulGulati)

# License

[MIT](https://github.com/BlockPoll/program)
