# Breakthrough in 6G Open-RAN Security! This Simulator Unveils the Core Capabilities of Trusted Perception ISAC [with Python code]

6G Open-RAN security breakthrough! This simulator reveals the core capabilities of Trust-Aware ISAC (Integrated Sensing and Communications) in the research field of 6G Open-RAN (Open Wireless Access Network). In the realm of security and adaptability, trust has always been a central theme. Recently, the Trust-Aware ISAC (Integrated Sensing and Communications) simulator, which is open sourced for submission to IEEE JSAC 2026, not only fully reproduces the core logic of the trust-aware quantum assisted digital twin control framework but also verifies its breakthrough performance in the 6G ISAC security scenario with bit-level reproducible experimental results.

Key highlights: Redefining the boundaries of security and performance for 6G ISAC
This simulator is more than just a simple theoretical verification tool; it is a full-link replication of the physical layer to the control layer for 6G ISAC, covering six key dimensions:
Physical layer: Reproduces 8×8 UPA scenarios at 28 GHz, 256 antenna JT-RZF cooperative transmission, and Rayleigh AR(1) fading, as well as lognormal shadow effects
Perception capability: Achieves Swerling-I detection, 512 pulse coherent accumulation, paired with a dedicated 400 MHz waveform, achieving perception accuracy at CRLB (Cramer-Rao Lower Bound) level
Digital twin: Implements a configurable synchronous delay twin model based on Kalman-like filters, supporting fidelity quantification assessment
Trust mechanism: Integrates the Bayes-EWMA (Exponential Weighted Moving Average) algorithm, ensuring the reliability of trust evaluation through bounded log likelihood and hard security threshold
Quantum assistance: Implements VQC (Variational Quantum Circuit) scoring using classical deterministic agents, reducing candidate actions from 50 to 12, significantly lowering computational overhead
Security protection: Supports Poisson trigger/geometric duration interference, deception, and hybrid attack simulations, accurately replicating abnormal attack patterns in 6G scenarios
Notably, when compared to the current strongest baseline (digital twin + quantum assistance):
Utility improvement **+2.3%** under nominal conditions
Utility improvement **+21%** under 6% abnormal attack scenarios
After sustained attacks, the trust value recovers 10% to 90% within 21 time slots without breaching the security baseline.

The core architecture of this simulation is a 10ms closed-loop trust perception control logic. The essence of this model lies in its replication of the closed-loop control stack of 6G ISAC—each 10ms a time slot, fully reproducing the entire process from physical measurements to base station deployment:
Physical measurement → Digital twin → Injection of anomalies → Trust evaluation → Quantum-assisted filtering → Trust perception gate → Base station deployment

Among these, the Trust perception gate is the core safety mechanism:
T(t) ≥ T_safe → Optimal action and safe action weighted output T(t) < T_safe → Force switching to static ISAC safe action
This ensures that the control strategy is monotonically secure from a mechanism perspective.

Quick Start Guide: Verification in 30 seconds, full experiment replication in 30 minutes with a minimal deployment process for researchers to quickly verify the framework's capabilities:
1. Clone the repository
2. Environment configuration (Python 3.10+)
   pip install -r requirements.txt
3. 30-second smoke test
   python src/controller.py
4. Full-scale experiment replication (approximately 30 minutes)
   python src/run_all.py
After the experiment, you can generate paper-level charts with one click:
Generate PNG/PDF: python tools/make_figures.py
Generate zero-dependency SVG: python tools/build_figures.py
All results are traceable to the JSON file in results/ directory, corresponding to the paper charts.

Experiment Results: Data confirms the dual advantages of 6G ISAC's security and performance
From the simulated data output, it is evident that this framework has significant advantages:
Baseline comparison: Static ISAC utility 0.459, complete framework utility 0.622, rate 96.8 Mbps, detection probability 0.721
Robustness to anomalies: under a 6% anomaly rate, the gap with the strongest baseline utility is 0.106, highlighting strong resilience against attacks.
Latency Tolerance: Twin latency within 1-10 slots, utility fluctuations are only approximately 1%, trust gate absorbs the cost of outdated telemetry.
Scalability: Scalable for both user/target scales, with a deployment inference latency of only 1.8ms, meeting near real-time control requirements.
V. Open Source Value: Promoting Reproducibility and Innovation in 6G ISAC Research This open-source simulation tool brings three major benefits to the field of 6G ISAC research:
1  
Bit-level reproducibility: A single master_seed ensures consistent results across all experiments.
2  
Low-threshold expansion: Supports the addition of pre-encoders, exception types, baseline methods, and deployment scale.
3  
Open Source Friendly: Follow the MIT license, with no barriers to collaboration between academia, industry, and research.
The core results in Table 3, Fig.2, Fig.6, etc. in the paper have been fully reproduced. The experimental summary report can be generated by one-click with src/synthesize.py to quickly verify the new algorithm and strategy.
6G Open-RAN security is moving from "adaptive" to trustworthy adaptive. This trust-aware ISAC simulator enables the integration framework of quantum assistance + digital twins + trust perception to move from theory to engineering validation, providing a unified benchmark platform for global 6G researchers.

## Images

![6G Open-RAN security breakthrough! This simulator reveals the core capabilities of trust-aware ISAC. [Python code attached]](01.jpg)
![6G Open-RAN security breakthrough! This simulator reveals the core capabilities of trust-aware ISAC. [Python code attached]](02.jpg)
![6G Open-RAN security breakthrough! This simulator reveals the core capabilities of trust-aware ISAC. [Python code attached]](03.jpg)
![6G Open-RAN security breakthrough! This simulator reveals the core capabilities of trust-aware ISAC. [Python code attached]](04.jpg)
![6G Open-RAN security breakthrough! This simulator reveals the core capabilities of trust-aware ISAC. [Python code attached]](05.jpg)
![6G Open-RAN security breakthrough! This simulator reveals the core capabilities of trust-aware ISAC. [Python code attached]](06.jpg)

<!-- PAYMENT_BLOCK -->

## Get this dataset

- Payment link (Stripe): [Buy now](https://buy.stripe.com/3cs8yP7sY87d0vu9AB)
- Payment QR code: ![Payment QR code](pay.png)

<!-- /PAYMENT_BLOCK -->
