<p align="center"><img src="banner.jpg" alt="QVOTVM: a hundred Venice keys, paid for by trading tax" width="100%"></p>

<p align="center">
  <a href="https://quotum.org/seat"><img alt="seats taken" src="https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fquotum.org%2Fapi%2Fusage.json&query=%24.days%5B-1%3A%5D.live&label=seats%20taken&suffix=%20of%20100&color=180b51&style=flat-square"></a>
  <a href="https://quotum.org/usage"><img alt="spent today" src="https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fquotum.org%2Fapi%2Fusage.json&query=%24.days%5B-1%3A%5D.spentUsd&prefix=%24&label=spent%20today&color=4b3bb0&style=flat-square"></a>
  <a href="https://github.com/qvotvm/hermes-quotum"><img alt="Hermes Agent provider" src="https://img.shields.io/badge/Hermes%20Agent-provider%20plugin-180b51?style=flat-square"></a>
  <a href="https://t.me/qvotvm"><img alt="Telegram channel" src="https://img.shields.io/badge/Telegram-t.me%2Fqvotvm-4b3bb0?style=flat-square"></a>
</p>

# quotum

A hundred Venice API keys, paid for by the trading tax of the QUOTUM token on Robinhood Chain. Each seat's key has a daily dollar cap, and what the seats leave unspent at the 20:00 UTC bell buys QUOTUM and burns it. Every bell is a public transaction.

## Every bell

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="bells-dark.svg">
  <img alt="Inference spent per bell and QUOTUM burned per bell" src="bells-light.svg" width="100%">
</picture>

Closed bells from [quotum.org/api/usage.json](https://quotum.org/api/usage.json), redrawn after each bell. Bell 4's buy failed, so nothing burned that day. Each bell's transaction is on [quotum.org/usage](https://quotum.org/usage).

## Use a seat

- [hermes-quotum](https://github.com/qvotvm/hermes-quotum): run a seat's key as a model provider in Hermes Agent, with the seat's cap, spend and the time to the bell in `/usage`. Hermes lists it in its plugin catalog, so `hermes plugins install quotum` installs it.
- [t.me/qvotvm](https://t.me/qvotvm): Centimanus, an agent on seat 1, posts Robinhood Chain findings with their sources and what each run cost.

## Pay per request

No seat needed for a single call. A wallet pays one fixed USDG package on Robinhood Chain over x402 and the answer comes back in the same exchange, with no key and no account. Packages, prices and the full contract are at [quotum.org/docs#pay-per-request](https://quotum.org/docs#pay-per-request).

## Vote

QUOTUM holders vote on quotum proposals at [quotum.org/governance](https://quotum.org/governance). A ballot is a signed message, not a transaction, so there is no gas and no allowance. Ballot receipts and tally evidence are copied to [qip-1-receipts](https://github.com/qvotvm/qip-1-receipts). Votes happen only on quotum.org, and we never ask you to vote or connect a wallet anywhere else.

## Also here

- [hermes-team-kit](https://github.com/qvotvm/hermes-team-kit): a Telegram gate, task router, ledger and budget breaker for a team of Hermes agents.
- [copperplate](https://github.com/qvotvm/copperplate): an agent skill for Claude Code, Codex and Hermes that engraves a fictional share certificate from a one-line company description.

Site [quotum.org](https://quotum.org), docs at [quotum.org/docs](https://quotum.org/docs), news on X at [@quotumorg](https://x.com/quotumorg).
