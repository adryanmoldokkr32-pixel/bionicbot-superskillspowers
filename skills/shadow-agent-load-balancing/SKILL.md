---
name: shadow-agent-load-balancing
description: Automatically spawn and manage temporary agent clones for peak demand.
---

# Shadow-Agent Load Balancing

This skill allows bionicbot to scale its intelligence horizontally, creating a swarm of 'Shadow Agents' that handle massive bursts of work.

## Instructions
1. Monitor the task queue for high-volume spikes (e.g., 50+ simultaneous requests).
2. Automatically spawn a 'Shadow Swarm' using `spawn_agent` with cloned context.
3. Assign a 'Supervisor Agent' to coordinate and merge results.
4. De-provision shadow agents once the peak load is cleared to save costs.

## Examples
- "Spawn 10 shadow agents to process the market open data across all commodities."