<p align="center"><img src="banner.png" alt="quotum: a hundred seats of private inference on the Venice API, paid for by trading tax" width="100%"></p>

<p align="center">
  <a href="https://quotum.org/seat"><img alt="seats taken" src="https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fquotum.org%2Fapi%2Fusage.json&query=%24.days%5B-1%3A%5D.live&label=seats%20taken&suffix=%20of%20100&color=180b51&style=flat-square"></a>
  <a href="https://quotum.org/usage"><img alt="spent today" src="https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fquotum.org%2Fapi%2Fusage.json&query=%24.days%5B-1%3A%5D.spentUsd&prefix=%24&label=spent%20today&color=4b3bb0&style=flat-square"></a>
  <a href="https://github.com/qvotvm/hermes-quotum"><img alt="Hermes Agent provider" src="https://img.shields.io/badge/Hermes%20Agent-provider%20plugin-180b51?style=flat-square"></a>
  <a href="https://t.me/qvotvm"><img alt="Telegram channel" src="https://img.shields.io/badge/Telegram-t.me%2Fqvotvm-4b3bb0?style=flat-square"></a>
</p>

# quotum

A hundred seats of private inference on the Venice API, paid for by the trading tax of the QUOTUM token on Robinhood Chain. A seat is taken by staking QUOTUM. Each seat has a daily dollar cap, and what the seats leave unspent buys and burns QUOTUM at the 20:00 UTC bell when the price guard allows. Every bell is a public transaction.

## Every bell

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="bells-dark.svg">
  <img alt="Inference spent per bell and QUOTUM burned per bell" src="bells-light.svg" width="100%">
</picture>

Closed bells from [quotum.org/api/usage.json](https://quotum.org/api/usage.json), redrawn after each bell. Bell 4's buy failed, so nothing burned that day. Each bell's transaction is on [quotum.org/usage](https://quotum.org/usage).

## Use a seat

- [hermes-quotum](https://github.com/qvotvm/hermes-quotum): run a seat's key as a model provider in Hermes Agent. Install with `hermes plugins install qvotvm/hermes-quotum --enable`; `hermes usage` then shows the seat's cap, spend, what is left and the time to the bell.
- [t.me/qvotvm](https://t.me/qvotvm): Centimanus, an agent on seat 1, posts Robinhood Chain findings with their sources and what each run cost.

## Pay as you go

No seat needed. A wallet prepays USDG on Robinhood Chain, and revocable project keys with model and daily limits spend it through an OpenAI-compatible endpoint, with a receipt for every charge. It is a pilot that needs an invite or a funding wallet holding at least 0.1% of QUOTUM supply. Check the intake status before sending USDG; x402 per-request intake for inference is closed. The x402 facilitator for other projects' USDG payments is a separate pilot: [quotum.org/facilitator](https://quotum.org/facilitator). Terms and status at [quotum.org/docs#payg](https://quotum.org/docs#payg).

## Vote

QUOTUM holders vote on quotum proposals at [quotum.org/governance](https://quotum.org/governance). A ballot is a signed message, not a transaction, so there is no gas and no allowance. Ballot receipts and tally evidence are copied to [qip-1-receipts](https://github.com/qvotvm/qip-1-receipts). Votes happen only on quotum.org, and we never ask you to vote or connect a wallet anywhere else.

## Also here

- [hermes-team-kit](https://github.com/qvotvm/hermes-team-kit): a Telegram gate, task router, ledger and budget breaker for a team of Hermes agents.
- [copperplate](https://github.com/qvotvm/copperplate): an agent skill for Claude Code, Codex and Hermes that engraves a fictional share certificate from a one-line company description.

Site [quotum.org](https://quotum.org), docs at [quotum.org/docs](https://quotum.org/docs), news on X at [@quotumorg](https://x.com/quotumorg).
