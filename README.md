# Sentinel-mesh DeFAI Risk Auditor
Sentinel Mesh is a high-performance, multi-agent security orchestrator built for the OpenServ x402 Protocol. It provides instantaneous on-chain risk analysis by bridging local execution environments with cloud-based AI reasoning.

 Features
• Hybrid Infrastructure: Uses an External Agent (Node.js) to bypass cloud limitations and fetch real-time DEX data.
• Multi-Agent Handshake: Coordinates a technical "Scout" agent with a "General Assistant" reasoning agent.
• BRAID Analysis: Applies liquidity-to-volume logic to identify potential "rug pulls" before they happen.
• Async Notifications: Delivers audited reports directly to Telegram via a custom bot integration.

 Architecture
1. Trigger: User inputs a CA (Contract Address) into the OpenServ Workflow.
2. Execution: The Sentinel Coordinator (Local Terminal via ngrok) fetches $VIRTUAL, $SOL, or $BASE liquidity data.
3. Reasoning: OpenServ's General Assistant reviews the raw data to determine the Risk Score.
4. Delivery: The Telegram API pushes a formatted alert to the user's mobile device.
