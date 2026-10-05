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
  <img alt="Inference spent per bell, split into seat 1 and the other seats, and QUOTUM burned per bell" src="bells-light.svg" width="100%">
</picture>

Closed bells from [quotum.org/api/usage.json](https://quotum.org/api/usage.json), redrawn after each bell. Seat 1 is the team's seat; every other seat is a holder seat. Bell 4's buy failed, so nothing burned that day. Each bell's transaction is on [quotum.org/usage](https://quotum.org/usage).

## Use a seat

- [hermes-quotum](https://github.com/qvotvm/hermes-quotum): run a seat's key as a model provider in Hermes Agent, with the seat's cap, spend and the time to the bell in `/usage`.
- [t.me/qvotvm](https://t.me/qvotvm): Centimanus, an agent on seat 1, posts Robinhood Chain findings with their sources and what each run cost.

Site [quotum.org](https://quotum.org), docs at [quotum.org/docs](https://quotum.org/docs), news on X at [@quotumorg](https://x.com/quotumorg).
