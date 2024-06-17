# Simple-PPO

This repo is simple implementation of PPO algorithm. PPO is model-free, on-policy reinforcement learning algorithm which constrain the KL-divergence of behavior policy and current policy.

In paper, there is two version of algorithm - Clipped Surrogate Objective and Adaptive KL Penalty Coefficient. We're implementing only clipped version of algorithm.

You can see the paper in [here](https://arxiv.org/pdf/1707.06347).

# Benchmark

We tested our implementation on 4 mujoco environment :
- [Half Cheetah](https://gymnasium.farama.org/environments/mujoco/half_cheetah/)
- [Hopper](https://gymnasium.farama.org/environments/mujoco/hopper/)
- [Inverted Double Pendulum](https://gymnasium.farama.org/environments/mujoco/inverted_double_pendulum/)
- [Walker2d](https://gymnasium.farama.org/environments/mujoco/walker2d/)

| HalfCheetah-v4 video | HalfCheetah-v4 training curve |
| --- | --- |
| ![HalfCheetah-v4](assets\HalfCheetah.gif) | ![HalfCheetah-v4](assets\HalfCheetah.png) |

| Hopper-v4 video | Hopper-v4 training curve |
| --- | --- |
| ![Hopper-v4](assets\Hopper.gif) | ![Hopper-v4](assets\Hopper.png) |

| InvertedDoublePendulum-v4 video | InvertedDoublePendulum-v4 training curve |
| --- | --- |
| ![InvertedDoublePendulum-v4](assets\InvertedDoublePendulum.gif) | ![InvertedDoublePendulum-v4](assets\InvertedDoublePendulum.png) |

| Walker2d-v4 video | Walker2d-v4 training curve |
| --- | --- |
| ![Walker2d-v4](assets\Walker2d.gif) | ![Walker2d-v4](assets\Walker2d.png) |

# Dependencies
This repo require following :
```
numpy
pytorch
matplotlib
gymnasium[mujoco]
```