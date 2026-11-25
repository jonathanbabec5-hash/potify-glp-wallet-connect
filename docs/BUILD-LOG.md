# November 25, 2026 · Green Light Pay Wallet Connection

**Question.** Help wallet developers reproduce the address-and-balance step in a mobile payment experience.

**Source and change.** green-light-wallet-525239 at `06dcf95384b2e07cc021226e627ace5e3ebb5227`. Standalone wallet reader and its embedded shipped HTML.

**Observed result.** The public entry page returned HTTP 200 and rendered local content in Chromium at a 390 × 844 viewport.

```sh
node tests/wallet.test.cjs
node tests/embed.test.cjs
```

**Next acceptance check.** Run the provider fixtures, then record an opt-in physical-phone connection and disconnect as a separate test.

**Owner and decision.** Chance coordinates public materials. The GLP project owner must confirm any commercial agreement. A mock connection does not establish native compatibility. This component neither signs nor settles a payment.

This dated record describes the developer package. Verify remote commit and tree in the publication receipt before announcing a GitHub release.
