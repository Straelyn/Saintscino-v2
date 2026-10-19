# The Saintscino · Debris — Smart Storage Unit slot machine for EVE Frontier

The Debris sister site of [The Saintscino](https://github.com/Straelyn/Saintscino): identical, except the only bet is **Debris**.

A slot machine that runs on a **Smart Storage Unit** in EVE Frontier (Stillness).
Bet **Debris**, win **SOF-40** and **EU-40 Fuel**. Every spin is a transaction on the
Sui blockchain, so the odds are enforced by the contract, not by the website.

**Play / dApp:** https://straelyn.github.io/Saintscino-v2/

---

## How to play

1. Fly to a storage unit running the casino and open its dApp window.
2. **Connect EVE Wallet** (top right).
3. Drag your stake into **your own slot** in the unit (the STORAGE UNIT panel).
   Accepted: **Debris**.
   The page shows what's in your slot.
4. Pick the material and a bet size (**1**, **5** or **10**), then press **Pull** and approve in your wallet.
5. Pushes and winnings land in your slot. Drag them out whenever you like.

Each spin costs a tiny amount of SUI for gas (about 0.001 SUI).

## Payouts (standard table)

Three of a kind pays:

| Symbols | Result | Chance | Paid in |
|---|---|---|---|
| Rift - Wild ×3 | 50× bet | 0.2% | SOF-40 Fuel |
| EVE Core ×3 | 40× bet | 0.5% | SOF-40 Fuel |
| LUX Split ×3 | 30× bet | 1.5% | SOF-40 Fuel |
| Asteroid ×3 | 20× bet | 5% | EU-40 Fuel |
| Feral Bar ×3 | Push | 15% | your stake back |
| anything else | Lose | 77.8% | — |

Wins are multiples of your bet: a 50× win pays 50 fuel on a 1-unit bet, 250 on a 5-unit bet and 500 on a 10-unit bet.
Each casino's owner can choose SOF-40 or EU-40 per win tier, so check the
**Three of a kind pays** list on the page for the casino you're at.

## Is it fair?

- The result comes from Sui's on-chain random number generator, inside the contract.
  The website only shows the result; it can't pick or change it.
- The contract can't be called in a way that lets anyone "roll, look, and cancel if they lose".
- If the house can't cover a win, the spin is cancelled and you keep your stake.

## Run a casino on your own storage unit

Anyone can run one on any storage unit they own:

1. In game, set your storage unit's dApp URL to `https://straelyn.github.io/Saintscino-v2/` and open its dApp window
   (or open that link in a browser that has your EVE wallet).
2. Connect your EVE wallet. The page lists your storage units: pick the one to use.
3. Press **Set up a casino on this unit**. One approval creates your casino (you're its admin),
   installs the slots extension (it replaces any other extension on the unit) and sets the unit's
   dApp URL to include the unit's id, so players always land on the right casino.
4. Stock the prizes in the unit's **main inventory**: with the standard payouts, at least **500 SOF-40** and **200 EU-40**
   covers the biggest wins on 10-unit bets (the panel recalculates if you change payouts).
5. Under **Accepted bets**, choose **Debris only** (new casinos start on the 3 materials).
6. Choose SOF-40 / EU-40 per tier under **Payouts**, then press **Open casino**.

Notes for owners:
- You can't play at your own unit: your drag-ins go to the bankroll, not a personal slot.
- Stakes collect in the unit's main inventory. Move them out now and then to keep space free.
- If a unit changes hands, the new owner presses **Claim this casino** to take over.
- If you move to a new storage unit, set the new unit up the same way; a casino belongs to one unit.

## On chain (Stillness, Sui testnet)

| | ID |
|---|---|
| Slots package (original) | `0xb67a0bf51d3374811c5b60ca30a32385924c1164e9e35a9ba30b4b07a13710c1` |
| Slots package (latest, v3) | `0xc8d6e5def6d1eb9abd2e2701aa7c16b202ed5ef4264f62922ac6c061a7233bcf` |
| EVE Frontier world | `0x7be18d6294e533bedd9a5d70a96ce8d9d4b87a7c74188ba65d3fe966bbed9d92` |

---

Questions, revisions or contract updates: **Strae on Discord**.
