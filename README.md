<h1 align="center">0xkiko</h1>

<p align="center">
  <b>Solidity Developer · Foundry · Security-focused</b><br>
  <sub>Remote · GMT+3 · Available 30+ hrs / week · Open to contract & full-time</sub>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Solidity-0.8.x-363636?style=flat-square&logo=solidity" alt="Solidity">
  <img src="https://img.shields.io/badge/Foundry-Forge-orange?style=flat-square" alt="Foundry">
  <img src="https://img.shields.io/badge/OpenZeppelin-Contracts-4E5EE4?style=flat-square&logo=openzeppelin" alt="OpenZeppelin">
  <img src="https://img.shields.io/badge/Tests-unit%20%C2%B7%20fuzz%20%C2%B7%20invariant-success?style=flat-square" alt="Tests">
</p>

---

### About

Solidity developer building access-controlled smart contracts with full Foundry test coverage — including **fuzz and invariant tests, not only unit**. Security-mindset from architecture to commits: CEI pattern, custom errors, role separation, OpenZeppelin primitives.

Code-first portfolio — every project below is open for review.

---

### Featured Projects

#### 🗂️ [inventory-orders-solidity](https://github.com/kiko21213/inventory-orders-solidity)

Production-style marketplace system in Solidity (815+ lines across **3 contracts** communicating through interfaces). Strict on-chain accounting with inventory, order lifecycle and fee orchestration.

- **Three-contract architecture** — `Inventory` + `OrderRegistry` + `MarketPlace`, isolated via interfaces
- **MarketPlace** — configurable BPS fees, VIP seller discounts, VIP buyer cashback, promo codes, pull payments
- **Accounting invariant** verified by handler-based invariant tests with ghost variables: `contract balance == userBalances + platformBalance`
- **Reserve / release / finalize** pattern for safe item locking, packed `Item` struct (`uint128 + uint128 + bool`)
- **State machines** — Inventory: `Active` / `Frozen` / `Closed`; Order: `Created` → `Paid` → `Shipped` / `Cancelled`
- **Static analysis** with [Slither](https://github.com/crytic/slither)

**Stack:** Solidity ^0.8.29 · Foundry · OpenZeppelin · Slither

---

#### 🔄 [BetterSwap](https://github.com/kiko21213/BetterSwapDEX) — *actively developed*

Uniswap-V2-style AMM in Solidity / Foundry — built from scratch.

- **LiquidityPool** — constant-product curve, `MINIMUM_LIQUIDITY` burn pattern, ReentrancyGuard, SafeERC20
- **Swap implemented** and verified by fuzz test asserting `k = x * y` constant-product invariant holds after every trade
- **PoolFactory.createPool** for paired tokens
- ERC-20 LP token (OpenZeppelin), geometric-mean initial mint, proportional subsequent mints
- Currently expanding: Router (multi-hop), fee mechanism, price oracle / TWAP

**Stack:** Solidity ^0.8.29 · Foundry · OpenZeppelin

---

### Tech Stack

```
Solidity        ^0.8.29
Framework       Foundry — Forge, Cast, Anvil
Libraries       OpenZeppelin — ERC-20, ERC-721, ReentrancyGuard, SafeERC20, AccessControl
Security        CEI, custom errors, RBAC, state machines, packed structs, pull payments
Testing         Foundry — unit, fuzz, invariant
Tooling         Git · Conventional Commits · GitHub Actions · ethers.js · Python
```

---

### Specialization

- Token contracts — ERC-20 / ERC-721 with custom logic
- Vesting, staking, airdrop systems
- Access control & role-based contract architecture
- State-machine and lifecycle-driven systems
- Foundry test design — unit, fuzz, invariant
- Solidity refactoring & modernization (custom errors, OZ v5)

---

### Contact

- 📨 **Email:** feras221vladimir@gmail.com
- 💬 **Telegram:** [@engineer_web3](https://t.me/engineer_web3)

<sub><i>Languages: English (fluent, async-friendly) · Russian (native)</i></sub>
