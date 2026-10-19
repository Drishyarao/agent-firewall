# AgentGuard: A Firewall for AI Agents

DevHack 2026 | PS 2.1: AI Agent Safety & Control | Team Sentinel

AgentGuard sits between an AI agent and the tools it uses. Every action the agent wants to take is checked first, then **allowed**, **blocked**, or **held for human approval**.

## Features
- Rule-based policy engine (no deletions, external emails held, payment limits)
- Prompt-injection detection on content the agent reads
- Human approval queue (Approve / Deny)
- Live dashboard with full audit log
- Kill switch that freezes the agent instantly
- Red Team mode: simulated attacks to demonstrate the defence

## Tech stack
Node.js, Express, HTML/JavaScript

## How to run
1. Install Node.js (v18 or higher)
2. In the project folder, run: `npm install`
3. Start the server: `node server.js`
4. Open http://localhost:3000 for the dashboard
5. In a second terminal, run `node test.js` to simulate an AI agent
6. Click **RED TEAM ATTACK** on the dashboard to simulate attacks

## Files
- `server.js`: the firewall (rules, approvals, kill switch)
- `test.js`: a fake AI agent that sends sample actions
- `public/index.html`: the live dashboard

## Note
All agent tools in this demo are simulated. No real emails, payments or deletions happen.