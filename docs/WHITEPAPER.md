# Green Light Pay Wallet Connection
## Whitepaper · public developer edition

**November 25, 2026 · Application source**

### Goal and audience

Help wallet developers reproduce the address-and-balance step in a mobile payment experience. The immediate audience is solana wallet integrators.

### Design and implementation

The adapter discovers providers, requests connection and reads balances. Its embedded browser version has mock-provider regression coverage. A wallet address identifies the connected account for a balance read. Authentication and payment authorization are separate product decisions.

### What a contributor can establish

The public entry page returned HTTP 200 and rendered local content in Chromium at a 390 × 844 viewport. Mock provider tests are repeatable. Record phone model, wallet version, connect, switch and disconnect separately before naming a supported device.

### Evidence and outstanding work

A mock connection does not establish native compatibility. This component neither signs nor settles a payment. The next acceptance case is concrete. Run the provider fixtures, then record an opt-in physical-phone connection and disconnect as a separate test.

### Place in POTIFY

Qualify one wallet-integration support request for a future fixed-scope GLP engagement. The marketing plan gives the test window and the evidence for a commercial outcome.

[Source provenance](source.json) · [Build log](BUILD-LOG.md) · [Marketing plan](MARKETING.md)
