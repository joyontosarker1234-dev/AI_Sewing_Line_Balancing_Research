# Primary Research Question

How can AI-driven line balancing combined with discrete-event simulation improve sewing-line efficiency in Bangladeshi garment factories?

## Hypotheses

1. **Hypothesis 1:** An RL-based assignment policy can produce higher throughput and lower balance delay than classical heuristics (like LPT or greedy).

2. **Hypothesis 2:** AI policies are more robust under real-world issues like worker absences (5-10%) and demand spikes.

3. **Hypothesis 3:** A simulation-trained AI policy can work on slightly different line setups (generalization).

## Evaluation Metrics

We will measure success using these numbers (calculated from simulation runs):

- **Throughput**: Items completed per hour (higher = better).
- **Average Cycle Time**: Time from start to finish per garment (seconds; lower = better).
- **Workstation Utilization**: % of time workers are busy (higher = better).
- **Balance Delay**: % of wasted time due to uneven tasks  
  → Formula: `(M × C - Σ p_i) / (M × C) × 100`  
  → (M = number of workers, C = cycle time, p_i = task times; lower = better).
- **Average Worker Idle Time**: Seconds workers wait per shift (lower = better).
- **Robustness**: How much performance drops under absences or demand spikes (% change).

## Why Bangladesh?

- RMG sector: 4,000+ factories, 4 million workers, $40B+ exports.
- Problems: High absenteeism (5-15%), demand fluctuations, unbalanced lines → 20-30% downtime.
- Opportunity: AI + simulation can reduce waste → more jobs, higher wages.
