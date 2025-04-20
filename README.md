# cordena-tax-handler

Solana on-chain logic to auto-handle Cordena’s 5% transaction tax.

## What It Does

This Solana program handles $CORD token transfer logic with built-in fee automation:
- **Burn 2%** of each transfer amount.
- **Redirect 3%** to a designated liquidity wallet.
- **Log all actions** transparently for verifiability.

## How It Works

1. User initiates a token transfer
2. The program intercepts it
3. It:
   - Splits the fee (2% burn, 3% LP)
   - Sends 95% to the recipient
   - Emits log messages

## To Do

- Write full logic for fee split
- Add Solana token authority checks
- Finalize LP & Burn addresses

## Program ID

TBD (to be added after deployment)

---

Built for Cordena: https://twitter.com/TheCordena