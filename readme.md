# Verified Airdrop

**Verified Airdrop** is a Web3 platform that lets projects distribute tokens only to **real humans** using **Civic verification** on **Solana**.

## What It Does

This app allows users to:
- Connect their Solana wallet (e.g. Phantom)
- Verify their identity via Civic Auth
- View available airdrops
- Claim tokens *only if verified* and *not previously claimed*

Projects can:
- Prevent bots and sybil attacks
- Track who claimed what and when

## Tech Stack

- **Frontend:** Next.js (React) + Tailwind CSS
- **Auth:** Civic Auth (`@civic/auth-react`)
- **Wallet:** Solana Wallet Adapter
- **Backend:** Node.js + TypeScript
- **Blockchain:** Solana Web3 + SPL Token transfers
- **Database:** Supabase or PostgreSQL (for claim tracking)

## MVP Scope

1. Connect wallet + Civic verification
2. Show list of airdrops
3. Protect “Claim” button until verified
4. Backend API to:
   - Verify Civic status
   - Check if already claimed
   - Send SPL tokens
   - Log claim

## Getting Started

### 1. Clone the repo
 
```bash
git clone https://github.com/your-username/verified-airdrop.git
cd verified-airdrop
```
### 2. Install Dependencies

```bash
npm install
```
### 3. Set up environment variables

```bash
Create a .env.local file with:
NEXT_PUBLIC_CIVIC_GATEKEEPER_NETWORK=...
NEXT_PUBLIC_SOLANA_NETWORK=...
```
### 4. Start the dev server

```bash
npm run dev
```
