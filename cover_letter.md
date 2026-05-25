Date: [Submission Date]

To: Editor-in-Chief
IEEE Transactions on Intelligent Transportation Systems

Dear Editor-in-Chief,

We submit our manuscript entitled "PA-TSMixer: Multi-Scale Temporal Mixing for
Aircraft Trajectory Prediction" for consideration for publication in the IEEE
Transactions on Intelligent Transportation Systems.

NOVELTY AND CONTRIBUTION:
This paper presents PA-TSMixer, a novel multi-scale temporal mixing architecture
for aircraft trajectory prediction. The key innovation is a parameter-efficient
three-branch design that captures trajectory patterns at fine (full resolution),
medium (2x pooled), and coarse (4x pooled) temporal scales, with proportional
capacity reduction (full, half, quarter hidden dimensions) that reduces multi-scale
overhead by 56% compared to uniform-capacity designs. To our knowledge, this is
the first work to systematically investigate multi-scale temporal mixing within
the TSMixer framework for the aircraft trajectory prediction domain.

The main contributions are:
1. A novel multi-scale architecture achieving 19.6% ADE reduction over TSMixer on
   synthetic aircraft data (p<0.001, 3 seeds)
2. Demonstrated noise robustness: relative improvement grows from 15.2% to 26.9%
   as GPS noise triples, due to implicit low-pass filtering in pooled branches
3. 59% prediction variance reduction on real-world ADS-B data (TartanAviation)
4. Per-maneuver analysis showing 36.9% ADE reduction on constant-turn trajectories
5. Comprehensive comparison against Transformer, TimesNet, TimeMixer, and LSTM
   baselines, with physics baselines (CV/CA/LR) establishing the necessity of
   data-driven methods

FIT WITH T-ITS:
Aircraft trajectory prediction is a core topic in intelligent transportation
systems, directly supporting conflict detection, flow management, and separation
assurance in air traffic management. Our work bridges the gap between general
time series forecasting architectures and the specific requirements of aviation
safety-critical applications. The demonstrated noise robustness and computational
efficiency (16x fewer parameters than Transformer) are of practical value for
real-time ATM deployment.

DATA AND CODE:
All datasets, model implementations, experiment scripts, and trained checkpoints
are publicly available at https://github.com/chunhaoliu/aircraft-main. The
manuscript source code is available at https://github.com/chunhaoliu/PA-TSMixer-T-ITS.

We confirm that:
- This manuscript has not been published or submitted elsewhere
- All authors have approved the manuscript and agree with its submission to T-ITS
- There are no conflicts of interest to declare
- The work complies with IEEE ethical standards

We suggest the following potential reviewers (optional):
[Optional: 3-5 reviewer suggestions with affiliations and emails]

Thank you for your consideration. We look forward to your response.

Sincerely,
Chunhao Liu (on behalf of all authors)
School of Automation
Nanjing University of Science and Technology
Nanjing 210094, China
Email: chunhao.liu@njust.edu.cn
