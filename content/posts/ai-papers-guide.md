+++
title = "A Guide to Landmark AI Papers (2013-2023)"
date = 2026-03-03T01:45:00-08:00
draft = false
description = "A guided tour of landmark AI papers across deep learning, generative models, RL, multimodal systems, and safety."
tags = ["ai", "research-papers", "llm", "ml"]
+++

This post is a fast, high-signal tour through landmark AI papers that shaped modern machine learning.
It starts with the architectural shifts that redefined deep learning, then moves into generation, scaling, and reasoning.
You will see how breakthroughs in language, vision, reinforcement learning, and multimodal systems connect.
The goal is not to overwhelm with trivia, but to give you a durable mental map of what mattered and why.
Use the index to jump by topic, or read top-to-bottom as a compact research timeline.
At the end, there is a distilled concept list you can reuse as a study and interview checklist.

## Index of Papers

1. [Attention Is All You Need (2017)](#1-attention-is-all-you-need-2017)
2. [Deep Residual Learning for Image Recognition (2015)](#2-deep-residual-learning-for-image-recognition-2015)
3. [BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding (2018)](#3-bert-pre-training-of-deep-bidirectional-transformers-for-language-understanding-2018)
4. [Distilling the Knowledge in a Neural Network (2015)](#4-distilling-the-knowledge-in-a-neural-network-2015)
5. [Auto-Encoding Variational Bayes (2013)](#5-auto-encoding-variational-bayes-2013)
6. [Generative Adversarial Networks (2014)](#6-generative-adversarial-networks-2014)
7. [Denoising Diffusion Probabilistic Models (2020)](#7-denoising-diffusion-probabilistic-models-2020)
8. [Scaling Laws for Neural Language Models (2020)](#8-scaling-laws-for-neural-language-models-2020)
9. [Language Models are Few-Shot Learners / GPT-3 (2020)](#9-language-models-are-few-shot-learners--gpt-3-2020)
10. [Scaling Laws for Autoregressive Generative Modeling (2020)](#10-scaling-laws-for-autoregressive-generative-modeling-2020)
11. [Training Compute-Optimal Large Language Models / Chinchilla (2022)](#11-training-compute-optimal-large-language-models--chinchilla-2022)
12. [Sparks of Artificial General Intelligence: Early Experiments with GPT-4 (2023)](#12-sparks-of-artificial-general-intelligence-early-experiments-with-gpt-4-2023)
13. [Playing Atari with Deep Reinforcement Learning (2013)](#13-playing-atari-with-deep-reinforcement-learning-2013)
14. [Deep Reinforcement Learning with Double Q-learning (2015)](#14-deep-reinforcement-learning-with-double-q-learning-2015)
15. [Mastering the Game of Go with Deep Neural Networks and Tree Search / AlphaGo (2016)](#15-mastering-the-game-of-go-with-deep-neural-networks-and-tree-search--alphago-2016)
16. [Decision Transformer: Reinforcement Learning via Sequence Modeling (2021)](#16-decision-transformer-reinforcement-learning-via-sequence-modeling-2021)
17. [CLIP: Learning Transferable Visual Models From Natural Language Supervision (2021)](#17-clip-learning-transferable-visual-models-from-natural-language-supervision-2021)
18. [BLIP-2: Bootstrapping Language-Image Pre-training with Frozen Encoders and LLMs (2023)](#18-blip-2-bootstrapping-language-image-pre-training-with-frozen-encoders-and-llms-2023)
19. [Neural Ordinary Differential Equations (2018)](#19-neural-ordinary-differential-equations-2018)
20. [Highly Accurate Protein Structure Prediction with AlphaFold (2021)](#20-highly-accurate-protein-structure-prediction-with-alphafold-2021)
21. [AutoML-Zero: Evolving Machine Learning Algorithms From Scratch (2020)](#21-automl-zero-evolving-machine-learning-algorithms-from-scratch-2020)
22. [Concrete Problems in AI Safety (2016)](#22-concrete-problems-in-ai-safety-2016)
23. [Training Language Models to Follow Instructions with Human Feedback / InstructGPT (2022)](#23-training-language-models-to-follow-instructions-with-human-feedback--instructgpt-2022)
24. [Interpretability in the Wild (2022)](#24-interpretability-in-the-wild-2022)

## 1. Attention Is All You Need (2017)

The paper introduced the Transformer architecture and removed recurrence/convolutions from the core sequence model in favor of attention. It reported strong machine-translation results (for example, WMT14 En-De and En-Fr) with better parallelization and shorter training time than prior approaches.

Source: <https://arxiv.org/abs/1706.03762>

## 2. Deep Residual Learning for Image Recognition (2015)

ResNet introduced residual blocks (`F(x) + x`) to make very deep networks trainable. In the paper, a 152-layer residual net achieved top performance on ImageNet-era benchmarks and strongly influenced later architectures across vision and language.

Source: <https://arxiv.org/abs/1512.03385>

## 3. BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding (2018)

BERT introduced deep bidirectional pretraining for language understanding and showed large gains on multiple NLP tasks through fine-tuning. Its reported setup and results made pretrain-then-finetune the standard pattern in NLP for years.

Source: <https://arxiv.org/abs/1810.04805>

## 4. Distilling the Knowledge in a Neural Network (2015)

This paper formalized knowledge distillation in modern deep learning practice: transfer performance from larger teacher models or ensembles into smaller student models using soft targets. It is still a core model-compression technique.

Source: <https://arxiv.org/abs/1503.02531>

## 5. Auto-Encoding Variational Bayes (2013)

This paper introduced the VAE framework and the reparameterization trick for low-variance gradient estimation in latent-variable models. It enabled scalable variational learning with neural networks and became foundational in generative modeling.

Source: <https://arxiv.org/abs/1312.6114>

## 6. Generative Adversarial Networks (2014)

GANs framed generative modeling as a minimax game between generator and discriminator. The original paper showed the core adversarial training setup and demonstrated that neural networks could learn to generate realistic samples without explicit likelihood modeling.

Source: <https://arxiv.org/abs/1406.2661>

## 7. Denoising Diffusion Probabilistic Models (2020)

DDPM introduced a diffusion-based generative approach with iterative denoising and reported strong image-generation quality metrics (including then-state-of-the-art FID on CIFAR-10). This became the basis for much of modern diffusion generation work.

Source: <https://arxiv.org/abs/2006.11239>

## 8. Scaling Laws for Neural Language Models (2020)

Kaplan et al. showed power-law relationships for language-model cross-entropy loss vs. model size, data, and compute in their regime. The paper’s key contribution is not a new architecture, but a predictive framework for planning training runs.

Source: <https://arxiv.org/abs/2001.08361>

## 9. Language Models are Few-Shot Learners / GPT-3 (2020)

GPT-3 scaled dense autoregressive language models to 175B parameters and demonstrated broad zero-/one-/few-shot behavior without gradient updates at inference time. The paper also documents limitations, including benchmark contamination risk and uneven task performance.

Source: <https://arxiv.org/abs/2005.14165>

## 10. Scaling Laws for Autoregressive Generative Modeling (2020)

This work extends scaling-law analysis beyond language to additional domains (including image/video and multimodal settings), reporting smooth power-law trends for autoregressive Transformer performance under scaling.

Source: <https://arxiv.org/abs/2010.14701>

## 11. Training Compute-Optimal Large Language Models / Chinchilla (2022)

Chinchilla argues many large LLMs were undertrained on tokens and provides a revised compute-optimal scaling view: roughly scale model size and training tokens together. A 70B model trained on 1.4T tokens (same compute budget as Gopher 280B) outperformed larger models on many evaluations.

Source: <https://arxiv.org/abs/2203.15556>

## 12. Sparks of Artificial General Intelligence: Early Experiments with GPT-4 (2023)

This paper is an exploratory capability study of an early GPT-4 version across diverse tasks. It is an argument and qualitative/quantitative investigation, not a formal proof of AGI.

Source: <https://arxiv.org/abs/2303.12712>

## 13. Playing Atari with Deep Reinforcement Learning (2013)

The DQN work showed end-to-end RL from raw pixels using convolutional networks and Q-learning variants. It was a turning point that connected deep perception models with RL control in a practical benchmark setting.

Source: <https://arxiv.org/abs/1312.5602>

## 14. Deep Reinforcement Learning with Double Q-learning (2015)

Double DQN addressed overestimation bias in Q-learning and demonstrated improved Atari performance and stability relative to vanilla DQN in the tested games.

Source: <https://arxiv.org/abs/1509.06461>

## 15. Mastering the Game of Go with Deep Neural Networks and Tree Search / AlphaGo (2016)

AlphaGo combined policy/value neural networks with tree search and achieved a landmark result in Go, including a 5-0 match win over European champion Fan Hui. This was a major milestone for deep RL + search systems.

Source: <https://www.nature.com/articles/nature16961>

## 16. Decision Transformer: Reinforcement Learning via Sequence Modeling (2021)

Decision Transformer recasts offline RL as conditional sequence modeling, using return-conditioned autoregressive Transformers instead of explicit value-function optimization. The paper reports competitive or better results on multiple offline RL benchmarks.

Source: <https://arxiv.org/abs/2106.01345>

## 17. CLIP: Learning Transferable Visual Models From Natural Language Supervision (2021)

CLIP trained on large-scale image-text pairs and used natural language prompts for zero-shot transfer to many vision tasks. It helped establish contrastive vision-language pretraining as a central paradigm.

Source: <https://arxiv.org/abs/2103.00020>

## 18. BLIP-2: Bootstrapping Language-Image Pre-training with Frozen Encoders and LLMs (2023)

BLIP-2 proposed an efficient bridge (Q-Former) between frozen vision encoders and frozen LLMs, reducing trainable parameters while maintaining strong vision-language performance.

Source: <https://arxiv.org/abs/2301.12597>

## 19. Neural Ordinary Differential Equations (2018)

Neural ODEs model hidden-state evolution as a continuous-time ODE solved by a numerical solver. Key benefits in the paper include adaptive computation and memory-efficient training via adjoint-style backpropagation.

Source: <https://arxiv.org/abs/1806.07366>

## 20. Highly Accurate Protein Structure Prediction with AlphaFold (2021)

AlphaFold2 demonstrated major progress on protein structure prediction, with CASP14 performance that the paper describes as competitive with experimental structures in a majority of cases. This was a major AI-for-science breakthrough.

Source: <https://www.nature.com/articles/s41586-021-03819-2>

## 21. AutoML-Zero: Evolving Machine Learning Algorithms From Scratch (2020)

AutoML-Zero explored evolutionary discovery of ML algorithms from primitive operations rather than predefined deep-learning components. It demonstrated that search can rediscover useful algorithmic motifs (including backprop-like behavior) in constrained settings.

Source: <https://arxiv.org/abs/2003.03384>

## 22. Concrete Problems in AI Safety (2016)

This paper framed practical AI safety around concrete problem classes such as reward hacking, side effects, scalable supervision, safe exploration, and distributional shift. It strongly influenced applied safety/alignment research agendas.

Source: <https://arxiv.org/abs/1606.06565>

## 23. Training Language Models to Follow Instructions with Human Feedback / InstructGPT (2022)

Ouyang et al. described a pipeline of supervised fine-tuning, reward modeling from human preferences, and PPO optimization (RLHF). A headline result is that a 1.3B InstructGPT model was preferred by human raters over 175B base GPT-3 outputs on their prompt distribution.

Source: <https://arxiv.org/abs/2203.02155>

## 24. Interpretability in the Wild (2022)

This entry refers to the 2022 IOI-circuit work (`Interpretability in the Wild: a Circuit for Indirect Object Identification in GPT-2 small`). It presents a mechanistic circuit-level analysis of a natural language behavior in GPT-2 small.

Source: <https://arxiv.org/abs/2211.00593>

## Most Important Concepts

1. **Self-attention**: lets models relate each token to others directly, enabling parallel sequence processing.
2. **Residual connections**: stabilize deep optimization via shortcut paths (`x + F(x)`).
3. **Pretraining + fine-tuning**: train generic representations first, then adapt cheaply to specific tasks.
4. **Knowledge distillation**: compress a stronger model into a smaller deployable model.
5. **Latent-variable generative modeling (VAE)**: learn probabilistic latent spaces with tractable training.
6. **Adversarial generative modeling (GAN)**: generator/discriminator game for sample realism.
7. **Diffusion modeling**: generation via iterative denoising of noisy samples.
8. **Scaling laws**: performance follows predictable trends with model size, data, and compute.
9. **Compute-optimal training**: best allocation of fixed FLOPs across model size, tokens, and steps.
10. **In-context learning**: behavior changes from prompts/examples at inference time, without gradient updates.
11. **RL from raw observations**: deep perception + RL control (DQN lineage).
12. **Overestimation bias control**: Double Q-learning reduces optimistic value bias in Q-learning systems.
13. **Sequence modeling for decision-making**: Decision Transformer treats RL trajectories as token sequences.
14. **Vision-language alignment**: CLIP/BLIP-2 style training aligns text and image representations.
15. **Continuous-depth networks**: Neural ODEs treat layer transitions as differential equations.
16. **AI for science at scale**: AlphaFold shows deep learning can solve domain-defining scientific tasks.
17. **Automated algorithm discovery**: AutoML-Zero explores search over algorithm space, not only architectures.
18. **Alignment and safety engineering**: practical safety problems and RLHF pipelines both matter for real-world deployment.
