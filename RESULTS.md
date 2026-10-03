# CMPE 260 – Project 1 (DQN Pong) — Results Log

Running record of every training run's key numbers, extracted from TensorBoard / training.log at the time each run finished. Use this as the single source of truth when writing the report — no need to dig back through Colab.

## Baseline (vanilla DQN: replay buffer + target network + epsilon-greedy)

| Metric | Value |
|---|---|
| Run name | `Oct02_22-06-02_5eeed8b9b8a3-PongNoFrameskip-v4` |
| GPU | Tesla T4 |
| Stop condition | Auto-stopped (`MEAN_REWARD_BOUND = 19.0`) |
| Frames to converge | 1,507,440 |
| Games played | 670 |
| Time to converge | 3.958 hours (~3 hr 57 min) |
| Final mean reward (100-game rolling avg) | **19.03** |
| Log confirmation | `Solved in 1507440 frames!` |

**Notes:** This run completed cleanly and exited on its own (unlike the first baseline attempt, which had to be manually killed and showed a text-log/TensorBoard mismatch due to stdout buffering). All four TensorBoard panels (reward, reward_100, epsilon, speed) agree exactly on the same endpoint — step 1,507,440, 3.958 hr — so this is a fully consistent, reliable baseline number. Use **19.03 / 1,507,440 frames / 3.958 hr / Tesla T4** as the official baseline for all Step 2 comparisons.

Screenshots: `screenshots/baseline/` (training_log_solved.png, epsilon.png, reward.png, reward_100.png, speed.png)

Earlier (superseded) run: 19.32 mean reward / 1,247,055 frames / 3.199 hr — kept for reference in `screenshots/baseline_19.32_old/`, not used for reporting.

## Step 2 — Algorithm 1: [TBD]

| Metric | Value |
|---|---|
| GPU | |
| Frames to converge | |
| Time to converge | |
| Final mean reward | |
| Target (≥10% faster than baseline) | ≤ 3.56 hours |
| Target (score closer to 21) | > 19.03 |

## Step 2 — Algorithm 2: [TBD]

| Metric | Value |
|---|---|
| GPU | |
| Frames to converge | |
| Time to converge | |
| Final mean reward | |
| Target (≥10% faster than baseline) | ≤ 3.56 hours |
| Target (score closer to 21) | > 19.03 |

## Step 3 — PER (on best of the two above)

| Metric | Value |
|---|---|
| GPU | |
| Frames to converge | |
| Time to converge | |
| Final mean reward | |
