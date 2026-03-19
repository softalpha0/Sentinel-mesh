Sentinel Mesh 
 A Multi-Agent DeFAI Security Orchestrator for Real-Time On-Chain Risk Mitigation.
## Project Overview
Sentinel Mesh is a decentralized finance (DeFAI) security layer built on the OpenServ x402 protocol. It bridges the gap between high-level AI reasoning and raw, on-chain execution. By utilizing a Multi-Agent Mesh, the system can ingest a token contract address, perform a deep liquidity and price audit on a local secure node, and coordinate with cloud-based LLMs to provide a human-readable risk assessment delivered directly to Telegram.
## The Architecture (The "Load-Bearing" Infra)
Sentinel Mesh doesn't just "chat" it executes. The system is composed of three distinct layers:
1. The Sentinel Coordinator (The Muscle): A custom External Agent running locally on a MacBook Pro, bridged to the OpenServ cloud via a secure ngrok tunnel. This agent utilizes a custom TypeScript SDK to fetch live data from DexScreener APIs and evaluate contract health.
2. The BRAID Auditor (The Brain): An OpenServ-native General Assistant that receives the technical data from the Sentinel. It applies the BRAID Reasoning Framework to evaluate if the liquidity-to-market-cap ratio suggests a "rug pull" or a safe entry.
3. The Notification Mesh (The Voice): A custom Telegram Bot Integration that provides real-time, asynchronous alerts, allowing traders to receive "Sentinel Reports" on their mobile devices the moment a risk is detected.
## Technical Stack
• Protocol: OpenServ x402 Agent Protocol.
• Language: TypeScript / Node.js.
• Infrastructure: External Agent via ngrok (Local-to-Cloud Bridge).
• Data Source: DexScreener On-Chain API.
• Alerting: Telegram Bot API.
• Security: Environment-variable-led (.env) credential management.
