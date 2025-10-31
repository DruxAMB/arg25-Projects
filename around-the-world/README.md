# Around the World – A Web3 Match-3 Adventure

## Team
- Team/Individual Name: Muhammad Amoo
- GitHub Handles: @druxamb
- Devfolio Handles: @druxamb

## Project Description
Match your way across five vibrant regions while weaving cultural storytelling into a casual puzzle experience. Around the World uses Base to bring onchain utility to a familiar match-3 loop, rewarding meaningful progress and ownership for players.

## Tech Stack
- Base (L2) smart contract platform
- Next.js 15 + React App Router
- TypeScript with strict ESLint configuration
- Tailwind CSS for styling
- Framer Motion for animations
- Globe.gl for 3D globe navigation
- MiniKit + OnchainKit for wallet onboarding
- Viem + Wagmi for blockchain interactions
- CDP SDK with spend permissions automation
- Upstash Redis for realtime leaderboards
- Gemini 2.0 Flash for reward calculations

## Objectives
- Deliver a playable match-3 prototype spanning five themed regions with both 3D globe and 2D map navigation.
- Integrate PlayerRegistry and NFT reward contracts so progression and collectibles are recorded on Base.
- Ship automated reward distribution leveraging Gemini AI + CDP spend permissions.
- Document setup, gameplay, and contribution flows so new collaborators can extend the experience without hand-holding.

## Weekly Progress

### Week 1 (ends Oct 31)
**Goals:**
- Lock down feature scope, success metrics, and milestone plan.
- Stand up Next.js + Tailwind foundation with MiniKit wallet onboarding.
- Scaffold data layer (Upstash Redis) and contract wrappers for PlayerRegistry + NFT minting.

**Progress Summary:**  <!-- Document outcomes, blockers, contract deployment status -->

### Week 2 (ends Nov 7)
**Goals:**
- Implement core match-3 mechanics, region theming, and dual navigation modes.
- Wire leaderboard data persistence + Gemini-driven reward calculations.
- Begin Farcaster social sharing and campaign challenge UX.

**Progress Summary:**  <!-- Capture gameplay progress, testing notes, and smart contract verification -->

### 🗓️ Week 3 (ends Nov 14)
**Goals:**
- Polish animations, audio, and responsive layout across devices.
- Run end-to-end reward distribution rehearsal on Base mainnet.
- Prepare final presentation assets, demo, and documentation updates.

**Progress Summary:**  <!-- Summarize QA results, launch readiness, and outstanding risks -->

## Final Wrap-Up
- **Main Repository Link:** `https://github.com/DruxAMB/AroundTheWorld`
- **Contract Deployment Link:** `https://basescan.org/address/0x2b2c5fb40096c0ab465c07b3a67ea77addb57d36`
- **Demo:** `https://youtu.be/OvT3Oa-bJcI`

## 🧾 Learnings
<!-- Summarize key takeaways after Week 3 -->

## Next Steps
<!-- Document post-program roadmap -->

## 🔗 Key Docs
- Around the World GitBook summary: `https://github.com/DruxAMB/AroundTheWorld/SUMMARY.md`
- Documentation hub index: `https://github.com/DruxAMB/AroundTheWorld/SUMMARY.md`

## ⚠️ Risks & Mitigations
- **AI reward automation maturity**: Gemini + CDP pipeline still undergoing integration tests. → Mitigation: maintain manual fallback playbook for Week 3 demo.
- **Base mainnet gas costs**: Live minting during demo could fluctuate. → Mitigation: preload demo wallets and rehearse transactions off-peak.
- **3D globe performance on low-end devices**: Globe.gl + animations may stutter. → Mitigation: ship quality toggle and ensure 2D map parity.

## 🔐 Smart Contract References
- AroundTheWorld: `0x2b2c5fb40096c0ab465c07b3a67ea77addb57d36`

## 📚 Additional Documentation
- GitBook: https://proofprep.gitbook.io/aroundtheworld/developer-documentation/project-overview
