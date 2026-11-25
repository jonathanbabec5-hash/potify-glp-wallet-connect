# Green Light Pay Wallet Connection

[Complete repository directory tree](docs/DIRECTORY.md)

**Application source.** Help wallet developers reproduce the address-and-balance step in a mobile payment experience.

### Setup and usage

Use Node.js 24 for the included checks. Use Python 3 for the local static preview.

```sh
python3 -m http.server 8000 --bind 127.0.0.1 --directory dist
```

Run the mock wallet suite. Open http://127.0.0.1:8000/ in a browser. 

### Developer entry points

The adapter discovers providers, requests connection and reads balances. Its embedded browser version has mock-provider regression coverage. Explore `tests/` in the full tree.

### Verification

The public entry page returned HTTP 200 and rendered local content in Chromium at a 390 × 844 viewport.

```sh
node tests/wallet.test.cjs
node tests/embed.test.cjs
```

### Release scope

A mock connection does not establish native compatibility. This component neither signs nor settles a payment. green-light-wallet-525239 at `06dcf95384b2e07cc021226e627ace5e3ebb5227`. Standalone wallet reader and its embedded shipped HTML.

[Technical whitepaper](docs/WHITEPAPER.md) · [Marketing and sales plan](docs/MARKETING.md) · [Dated developer log](docs/BUILD-LOG.md)

Existing asset and code terms remain applicable. Public access to a recording, illustration, brand or manuscript does not itself grant commercial reuse rights.
