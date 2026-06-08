# Mini Hack Cohort 2 — Gaming and Gamified Solutions on Avalanche
> Team1 Kenya | 2026 | Technical Lead: Joseph Njoroge (Scotch)

[![Status](https://img.shields.io/badge/Cohort%202-Upcoming-555?style=flat-square)](https://team1-kenya-mini-hack.vercel.app)
[![Network](https://img.shields.io/badge/Network-Avalanche%20Fuji-e84142?style=flat-square)](https://testnet.snowtrace.io)
[![Stack](https://img.shields.io/badge/Stack-Solidity%20%7C%20ERC--721%20%7C%20IPFS%20%7C%20WebSockets-333?style=flat-square)](#tools)

Fork this repo to your personal GitHub account. Build a game or gamified system with on-chain assets and token economies on Avalanche. Deploy to Fuji testnet. Present at Builders Connect.

---

## Prerequisite

Cohort 2 requires Cohort 1 completion or equivalent knowledge. Equivalent means you can demonstrate:

- Writing and deploying a Solidity contract to Fuji testnet using Hardhat
- Writing passing unit tests with Hardhat and Chai
- Connecting a wallet to a frontend using ethers.js or the Core Wallet SDK
- Reading and writing contract state from a frontend

If you completed Cohort 1, you are ready. If you did not, complete the freeCodeCamp JavaScript Algorithms and Data Structures certification and work through the Avalanche Academy Smart Contracts Fundamentals module before applying.

---

## What you will build

A playable game or gamified system with digital ownership at its core. By Week 4 you will have minted NFT in-game assets, built a reward token economy, implemented on-chain game logic with a leaderboard, and deployed a working frontend with multiplayer state.

---

## Session schedule

| Day | Time | Platform | What happens |
|-----|------|----------|-------------|
| Tuesday | 8:00 PM EAT | Google Meet | New concepts, live coding, hands-on exercises |
| Thursday | 8:00 PM EAT | Google Meet | Second teaching block — select Thursdays include a guest practitioner in the second half |
| Thursday | 6:00 PM EAT | Discord voice | Office hours — bring your blockers before the main session |

Google Meet link is pinned in Discord `#announcements`.

---

## Getting started

### 1. Fork this repository

Click **Use this template** or **Fork**. Fork to your personal GitHub account.

### 2. Clone and set up

```bash
git clone git@github.com:YOUR-HANDLE/minihack-cohort2-template.git
cd minihack-cohort2-template
npm install
cp .env.example .env
npx hardhat compile
```

### 3. Get Fuji testnet AVAX

Visit [core.app/tools/testnet-faucet](https://core.app/tools/testnet-faucet) and request AVAX to your Core Wallet Fuji address.

---

## Accounts to create before Week 1

| Account | Link | Notes |
|---------|------|-------|
| GitHub | github.com | Use your real name |
| Avalanche Builders Hub | core.app/builders-hub | Quest 1 — primary KPI, create this first |
| Core Wallet on Fuji | core.app | Required wallet |
| Alchemy or Infura | alchemy.com | Free tier — RPC access |
| Pinata | pinata.cloud | Free tier — IPFS storage for NFT metadata |

Fuji testnet RPC:
```
RPC URL:   https://api.avax-test.network/ext/bc/C/rpc
Chain ID:  43113
Explorer:  https://testnet.snowtrace.io
```

---

## Weekly workflow

```bash
git checkout main
git pull origin main
git checkout -b week-{N}-{your-github-handle}
```

PR title format:
```
[Cohort 2 Week N] Your Name - Deliverable title
```

Submit PR link in Discord `#submissions` and complete quests on Plug and Play — both due Sunday midnight EAT.

---

## Weekly deliverables and quests

### Week 1 — NFTs and in-game asset ownership

**Sessions:**
- Tuesday: Blockchain gaming — play-to-earn vs play-and-own. ERC-721 and ERC-1155 token standards — differences, when to use each, gas implications.
- Thursday: Minting an NFT on Fuji. Storing metadata on IPFS with Pinata. Displaying NFT assets in a game UI. OpenSea metadata standards.

**Deliverable:** Mint an in-game asset NFT (sword, character skin, or item of your design) on Fuji testnet. Display it in a basic HTML or React UI. Submit: contract, mint script, IPFS metadata link, and a screenshot of the NFT in your UI.

**Quests (Plug and Play — due Sunday midnight EAT):**

| Quest | Task |
|-------|------|
| Q1 | Create or verify your Builders Hub account — submit a screenshot of your active profile |
| Q2 | Complete the "NFTs on Avalanche" module on Avalanche Academy and upload your certificate |
| Q3 | Deploy your ERC-721 contract to Fuji and submit the Snowtrace link |
| Q4 | Upload your NFT metadata to IPFS via Pinata and submit the IPFS CID |
| Q5 | Post a screenshot of your NFT displayed in your UI in Discord `#week-1-cohort2` |

---

### Week 2 — On-chain game logic and token economies

**Sessions:**
- Tuesday: What belongs on-chain vs off-chain in a game — trade-offs of gas, speed, and verifiability. Writing a game contract that records scores, ownership, and outcomes. On-chain randomness. Gas optimisation patterns.
- Thursday: Designing a game token economy — minting, earning, spending, anti-inflation mechanics. ERC-20 reward token tied to gameplay. In-game shop contract. Treasury design and emission schedules. Lessons from real blockchain game economies.

**Deliverable:** A game contract that records player scores and picks a winner. A reward token players earn by playing. An in-game shop where tokens can be spent. Submit: contracts, tests, deployment scripts, and a written explanation of your token emission design.

**Quests (Plug and Play — due Sunday midnight EAT):**

| Quest | Task |
|-------|------|
| Q1 | Complete the "Token Design" or "DeFi Fundamentals" module on Avalanche Academy and upload your certificate |
| Q2 | Deploy your game contract to Fuji and submit the Snowtrace link |
| Q3 | Write a 1-page token economy design doc — supply, earn rate, sink mechanisms — submit as a GitHub gist link |
| Q4 | Run a local test simulating 3 players earning and spending tokens — submit a screenshot of the passing test |
| Q5 | Post in Discord `#week-2-cohort2`: what is one thing that could break your token economy, and how would you fix it? |

---

### Week 3 — Multiplayer systems and Avalanche subnets

**Sessions:**
- Tuesday: Multiplayer on-chain mechanics — leaderboards, PvP outcomes, session-based state. Off-chain state with on-chain settlement. Real-time updates using WebSockets alongside on-chain events.
- Thursday: Avalanche subnets — what they are, why gaming studios use them, custom gas tokens, high throughput, low fees. Deploying to a test subnet. Bridging assets back to C-Chain. Gamified systems beyond games — loyalty programmes, community engagement, reward systems for Kenyan brands.

**Deliverable:** A multiplayer mini-game with an on-chain leaderboard. Players compete, scores are recorded on-chain, and a winner is determined by the contract. Submit: all contracts, a WebSocket backend, and a frontend that shows the live leaderboard.

**Quests (Plug and Play — due Sunday midnight EAT):**

| Quest | Task |
|-------|------|
| Q1 | Complete the "Avalanche Subnets" module on Avalanche Academy and upload your certificate |
| Q2 | Deploy your leaderboard contract to Fuji and submit the Snowtrace link |
| Q3 | Submit a 3-sentence explanation of why a gaming studio would choose a subnet over C-Chain |
| Q4 | Design a gamified loyalty programme for a real Kenyan business — submit a 1-page concept doc |
| Q5 | Deploy at least one contract component to a test subnet and submit the deployment details |

---

### Week 4 — Build sprint and Demo Day

**Sessions:**
- Tuesday: No new content. Full build sprint. Technical lead and module leads run 15-minute check-in slots on Discord voice throughout the day.
- Thursday: Final testing and bug fixes. Demo rehearsal — each builder does a practice 3-minute run-through. Community feedback. Preparation for Builders Connect.

**Deliverable (Final project):** A playable game or gamified system deployed on Fuji testnet. Must include NFT assets, a reward token, at least one on-chain interaction per play session, and a working frontend. Submit: GitHub repo, deployed frontend URL, Snowtrace links for all contracts, and a 5-minute demo video.

**Demo Day:** Builders Connect — last Saturday of the month. Each builder gets 3 minutes live demo + 2 minutes Q&A. Mandatory for graduation.

**Quests (Plug and Play — due Sunday midnight EAT):**

| Quest | Task |
|-------|------|
| Q1 | Deploy your final game or gamified system to Fuji and submit all Snowtrace contract links |
| Q2 | Submit your GitHub repo with README covering: what you built, how to play it, how the economy works |
| Q3 | Upload your 5-minute demo video link |
| Q4 | Complete the cohort exit survey on Plug and Play |
| Q5 | Nominate one fellow builder for community recognition in Discord `#shoutouts` |

---

## Assessment rubric

| Criterion | Weight | Excellent | Good | Needs work |
|-----------|--------|-----------|------|------------|
| Functionality | 35% | All features work on testnet | Core features work | Partial or broken |
| Integration depth | 25% | NFT + token + on-chain game logic + frontend | Two layers integrated | Single component only |
| Code quality | 20% | Clean, commented, tested | Readable, some tests | Hard to follow, no tests |
| Documentation | 10% | Full README + demo video | README present | Minimal docs |
| Demo presentation | 10% | Clear, confident, live demo | Demo works with notes | Slides only, no demo |

**Grade bands:** Distinction 90-100% / Merit 75-89% / Pass 60-74% / Incomplete below 60%

Week 4 final project = 40% of cohort grade. Weeks 1-3 = 60% combined.

---

## Submission policy

- **Deadline:** Sunday midnight EAT for PR link and quests
- **Late — up to 48 hours:** Accepted with 20% penalty
- **Late — beyond 48 hours:** Zero for that week
- **Three consecutive zeros:** Removal from cohort without certificate
- **Week 4 pairs:** Allowed — both builders listed in PR, both present at Builders Connect

---

## Resources

**Avalanche**
- Docs: [docs.avax.network](https://docs.avax.network)
- Builders Hub: [core.app/builders-hub](https://core.app/builders-hub)
- Core Wallet: [core.app](https://core.app)
- Fuji faucet: [core.app/tools/testnet-faucet](https://core.app/tools/testnet-faucet)
- Snowtrace Fuji: [testnet.snowtrace.io](https://testnet.snowtrace.io)

**NFTs and gaming**
- OpenZeppelin ERC-721: [docs.openzeppelin.com/contracts](https://docs.openzeppelin.com/contracts)
- Pinata IPFS: [docs.pinata.cloud](https://docs.pinata.cloud)
- Hardhat: [hardhat.org/docs](https://hardhat.org/docs)
- ethers.js: [docs.ethers.org](https://docs.ethers.org)

**Programme**
- Handbook: [team1-kenya-mini-hack.vercel.app](https://team1-kenya-mini-hack.vercel.app)
- Discord: linked from the landing page

---

## Help

Post in Discord `#help` with: what you are trying to do, what you tried, and the exact error message.

Office hours: Thursdays 6:00 PM to 7:00 PM EAT on Discord voice.

Tag `@scotch` only after posting in `#help` and not getting a response within a reasonable time.
