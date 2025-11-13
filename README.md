# AI-for-Brain-Disease-Diagnostics-Strategic-Adoption-and-Market-Entry-of-QP-Brain-in-UK-Healthcare
📘 Project Overview

This repository presents part of the group project “AI for Brain Disease Diagnostics: Strategic Adoption and Market Entry of QP-Brain in UK Healthcare”, conducted at Queen Mary University of London (MSc Business Analytics, 2024/25).

The project explores how Quibim’s QP-Brain, an AI-powered MRI analysis tool for neurological conditions, can be strategically deployed across the NHS England system. It combines market research, data analytics, and strategy design to propose a phased adoption plan for real-world AI implementation in healthcare.

This repository focuses on Section 3: Trust-Level Prioritisation Framework, which forms the analytical foundation of the entire project.

🎯 Section 3 – Trust-Level Prioritisation Framework

The objective of this section is to identify NHS Trusts with the highest potential need for QP-Brain deployment, based on operational capacity, diagnostic burden, and digital readiness.

Analytical Goals

Quantify diagnostic pressure across NHS Trusts.

Integrate multi-source NHS datasets into comparable indicators.

Normalise and score each Trust to measure diagnostic demand.

Apply K-means clustering to segment Trusts into priority groups for phased rollout.

⚙️ Methodology
1. Data Normalisation

Variables scaled using Min–Max normalisation (Go et al., 2020).

Ensures comparability among indicators with different units or directions (↑ good / ↓ good).

𝑥
′
=
𝑥
−
min
⁡
(
𝑥
)
max
⁡
(
𝑥
)
−
min
⁡
(
𝑥
)
x
′
=
max(x)−min(x)
x−min(x)
	​

2. Composite Scoring

Combines multiple indicators (MRI volume, waiting time, radiology staffing, and GDE flag).

Equal weighting applied in the baseline model.

Score
𝑖
=
1
𝑛
∑
𝑗
=
1
𝑛
𝑥
𝑖
𝑗
′
Score
i
	​

=
n
1
	​

j=1
∑
n
	​

x
ij
′
	​


Higher scores = greater diagnostic burden and stronger AI adoption potential.

3. Trust Segmentation via K-means Clustering

Following Momahhed et al. (2023), K-means clustering was used to group Trusts by operational similarity.
The analysis produced three deployment phases:

Phase	Characteristics	Strategic Implication
Phase 1	High MRI volume + long waiting time	Early deployment & pilot validation
Phase 2	Long waiting + lower volumes	Secondary rollout
Phase 3	Efficient but high workload	Demonstration & scalability sites
📊 Key Insights

Diagnostic workload and workforce gaps are unevenly distributed across NHS Trusts.

A small cluster of large, high-burden Trusts (e.g. UHB, NCA, Imperial College Healthcare) represent optimal pilot sites for early QP-Brain adoption.

The framework enables data-driven, scalable rollout aligned with NHS operational priorities.

🧾 References

Go, Y.-S., Lee, S., & Kim, C. (2020). Development of the Korean Community Health Determinants Index (K-CHDI). PLOS ONE, 15(10), e0240304.

Momahhed, M., et al. (2023). K-means Clustering of Outpatient Prescription Claims for Health Insureds in Iran. BMC Public Health, 23, 1065.

NHS England (2024). Diagnostic Imaging Dataset Statistical Release.

NHS England (2024). Diagnostics Waiting Times and Activity Statistics.

NHS England (2025). HCHS Workforce Census.

NHS England (2024). Acute Global Digital Exemplars Programme Report.

📄 License

This repository is provided for academic and non-commercial use only as part of a postgraduate coursework project.
Please cite the original report if using this work in any publication or research output.
