##Project Research Update #3

We have successfully implemented a complete end-to-end Reinforcement Learning (RL) pipeline for adaptive LLM task offloading. By leveraging the BurstGPT dataset, we developed a custom  simulation environment that evaluates offloading decisions across a three-tier architecture: Local, Edge, and Cloud.

Key Technical Achievements:

- Built a numpy-backend environment that accounts for dynamic queue pressure and token length dependent latency.

- Trained a Proximal Policy Optimization (PPO) agent that successfully learned to navigate the trade-off between energy consumption and P99 latency SLOs.

- Established baselines (Always Local, Threshold-based, and Random policies) to quantify the performance gain of an intelligent controller.

- Result: The agent demonstrated a proactive shift in strategy, successfully identifying when local resource congestion necessitates offloading to cloud tiers to prevent latency violations.


Overall, with the core training loop, environment, and baseline comparison framework now fully operational, we have a foundation for a research paper.
