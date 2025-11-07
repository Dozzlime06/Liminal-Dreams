# AI Agent Creation Flow

## Steps
1. User mints NFT on OpenSea (optional for airdrop)
2. User **pays $LD tokens** to create AI agent
3. **x402Scan detects payment and deploys AI agent**
4. Agent executes predefined on-chain tasks
5. All activity and payments are logged by x402Scan

## Example API Request (Optional Frontend)
```json
{
  "userAddress": "0x1234...abcd",
  "agentType": "trading-bot",
  "paymentLD": 100
}

Example Response

{
  "status": "success",
  "agentId": "AGENT_001",
  "message": "AI agent deployed successfully.",
  "paymentLD": 100
}

Notes:
	•	API is optional; x402Scan handles agent creation automatically upon $LD payment
	•	NFT is optional; only $LD payment is required
	•	x402Scan logs agent creation, payment, and activity

---

# **architecture.md**  

```markdown
# Liminal Dreams Architecture

## Components
1. **NFT Mint Pass**
   - ERC-721 on OpenSea
   - Optional, for $LD airdrop eligibility
2. **$LD Token**
   - ERC-20 on HyperEVM
   - Used as **payment** for AI agent creation
3. **AI Agent**
   - Created automatically by x402Scan upon $LD payment
   - Performs predefined on-chain tasks
4. **x402 Explorer**
   - Detects $LD payments
   - Deploys AI agents
   - Tracks agent activity and payments
   - Provides transparency and analytics dashboards
