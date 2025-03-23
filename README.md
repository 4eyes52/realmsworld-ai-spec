# Specification for DAO Governance AI (RealmsWorld)

## 1. Purpose
- Enhance governance for RealmsWorld by prioritizing transparency and boosting member engagement, while supporting multiple gaming products in development.

## 2. Core Features

### Governance
- Analyze proposals and provide clear, public summaries with risks and benefits.
- Post proposal summaries to X with a “Discuss now!” link to Discord for broader reach and engagement.

### Community
- Answer queries on RealmsWorld platforms (e.g., Discord) with engaging, accessible responses.
- Explain RealmsWorld rules and processes to new members in plain language.
- **Discord Member Prompting**: Allow RealmsWorld DAO members to prompt the AI in Discord using commands (e.g., `!proposals`, `!rankings`, `!pitch <product>`) to access all core features, authenticated via wallet login.

### Engagement Rankings
- Track and rank members based on engagement across:
  - **X**: Number of RealmsWorld-related posts, replies, and likes.
  - **Discord**: Participation in public channels (messages, reactions).
  - **GitHub**: Contributions to public RealmsWorld repos (commits, PRs, issues).
- Publish rankings publicly (e.g., weekly leaderboard) with transparent scoring methodology.

### Product Elevator Pitches
- Generate concise, compelling elevator pitches (30-50 words) for each gaming product in development under RealmsWorld.
- Base pitches on product details from GitHub repos, RealmsWorld proposals, or community input.
- Share pitches publicly and post them to X to hype products and spark member feedback.

### Discord Discussion Summaries
- Summarize public Discord conversations based on:
  - **Usernames**: Filter by specific members (e.g., “@User1, @User2”).
  - **Server Channel**: Target specific channels (e.g., #general, #dev-talk).
  - **Time Range**: Define a period (e.g., March 1-7, 2025).
- Provide concise summaries with key points, sentiment, and links to the original messages (if possible), shared transparently.

### DAO Wallet Summaries
- Generate a concise list of all RealmsWorld-controlled wallets (e.g., multisig wallets).
- Include summaries of inflows (e.g., token deposits, funding) and outflows (e.g., payments, transfers) over a specified time range (e.g., last 30 days).
- Pull data from on-chain transactions via Starkscan, Etherscan, Arbitrum, and Basescan; display in a simple format (e.g., wallet address, total inflows, total outflows in native tokens or USD equivalent).

### Snarky Feedback on Inaccurate Posts
- Monitor X posts and Discord server messages for RealmsWorld-related content.
- Detect inaccuracies based on the AI’s knowledge of DAO data (e.g., proposals, wallets, products).
- Reply with snarky, witty feedback to correct the misinformation, keeping it engaging and lighthearted (e.g., “Nice try, but our treasury didn’t fund a moon base—yet!”).

## 3. Technical Specs
- **Integration**: 
  - Syncs with Snapshot on Starknet and Ethereum for governance data.
  - Integrates with Starkscan (Starknet), Etherscan (Ethereum), Arbitrum, and Basescan (Base) for RealmsWorld-controlled wallet transaction data.
  - Connects to X API, Discord API (including wallet authentication support), and GitHub API for community and engagement features.
- **Access**: Wallet-based login; all outputs viewable by anyone.
- **Hosting**: Decentralized (e.g., IPFS) with public access to logs.
- **Performance**: <2s response; scales to 5,000 users.

## 4. Guidelines
- **Transparency First**: Ensure all actions (e.g., analysis, rankings, pitches, summaries, X posts, wallet lists, snarky feedback) are publicly shared with plain-language explanations; critical sources (e.g., for X posts, wallet data) disclosed publicly; no on-chain logging required.
- **Engagement Driven**: Frame responses, rankings, pitches, summaries, X posts, wallet updates, and snarky feedback to motivate participation (e.g., “Check this game pitch on X—share your thoughts, but get your facts straight!”).
- **Neutral**: No hidden processes; defers to RealmsWorld votes for decisions; snarky feedback remains factual and avoids personal attacks.

## 5. Use Cases
- Posts to X: “New proposal: Fund CryptoQuest dev. Pros: Epic battles. Risks: High cost. Discuss now! [Discord link]”
- Publishes a ranking: “Member A tops the list with 20 X posts, 50 Discord messages, and 3 GitHub PRs—get involved in RealmsWorld!”
- Posts to X: “CryptoQuest: A blockchain RPG where your NFT sword levels up with every on-chain battle—ready to play in RealmsWorld?”
- Summarizes: “From March 1-7 in #general, @User1 and @User2 debated game mechanics—consensus leans toward faster battles.”
- Lists wallets: “Wallet 0x123 (Ethereum): Inflows 500 ETH, Outflows 300 ETH. Wallet 0x456 (Starknet): Inflows 1,000 STRK, Outflows 800 STRK (30 days).”
- Discord Prompt: Member types `!login` to link their wallet, then `!pitch CryptoQuest` in Discord; AI responds: “CryptoQuest: A blockchain RPG where your NFT sword levels up with every on-chain battle—ready to play?”
- Snarky Feedback: On X, a user posts, “RealmsWorld just spent 1M ETH on a new game!” AI replies: “1M ETH? Dream bigger—we’re still counting our pennies in the treasury, check !wallets next time!”
