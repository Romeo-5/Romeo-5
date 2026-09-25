# Hi, I'm Romeo! 👋

**🎓 MS CS (AI) @ USC · Graduating May 2027 | 🤖 Robotics Research @ USC ISI | ⚛️ Nuclear M&S**

I build the machine learning layer for physical systems where being wrong is expensive: robots, energy servers, reactors. Different hardware, one question: how much behavior can a model learn without abandoning the physics that governs it?

---

## 🔬 Research & Work

**@ USC Information Sciences Institute — Polymorphic Robotics Lab** *(Sep 2025 – present)*
- Developing a **distributed inverse kinematics algorithm** for modular self-reconfigurable robots: each module runs its own local solver and coordinates by message passing over the physical connection graph, applying damped least squares to its local Jacobian column. No single controller needs the full kinematic chain
- Moved constraint enforcement into individual modules, making the solver **morphology-agnostic**. The same algorithm runs on arbitrary assembled topologies without re-deriving kinematics
- Write the physics simulation stack in **C**; tuned constraints in Unreal Engine and MuJoCo (including unit-scale inertia corrections for critical damping) and built the sim-to-real pipelines validating on physical SuperBot hardware

**@ Bloom Energy — Failure Analysis, Quality & Reliability** *(Summer 2026)*
- Scaled a telemetry-based failure detector for DC-DC power converters to the full confirmed-failure population: **recall 82.2% → 92.5%, zero new false positives, ~27-day median detection lead**
- Owned a failure investigation end to end, reliability modeling through physical flow-bench testing, and presented it at the company-wide review
- Proposed and built a **locally-hosted conversational agent** (Ollama, tool-use architecture) over the fleet analytics, plus a config-driven CLI, so the team's PhD specialists could run analyses without me
- Researched **single-event effects** device physics and neutron detection instrumentation for a radiation-effects test campaign

**@ LineSlip Solutions** *(2024 – 2026)*
- Production **RAG** pipeline on Llama 3.1-8B with Elasticsearch retrieval and custom reranking, serving **10K+ queries/day**; 35% accuracy improvement, 40% latency reduction via INT8 quantization

---

## 💡 Research Interests

Applying AI and optimization where physics constrains the solution:

⚛️ **Nuclear** — reactor modeling & simulation, surrogate models, digital twins, fault diagnosis · 🔋 **Energy Systems** — degradation, predictive maintenance, fleet reliability · 🤖 **Robotics** — distributed control, modular systems, sim-to-real · 🧪 **Physics-Informed ML** — learning dynamics without discarding the governing physics

---

## 📌 Featured Projects

### ⚛️ [Surrogate Modeling of Lattice Reactivity with Uncertainty Quantification](https://github.com/Romeo-5/Surrogate-Modeling-of-Lattice-Reactivity-with-Uncertainty-Quantification)
Monte Carlo neutron transport in OpenMC, with a surrogate measured against the stochastic uncertainty of the calculation it replaces

- **488-run transport campaign** over a PWR pin-cell lattice, sweeping enrichment, fuel temperature, moderator density, and pitch
- Verified by Shannon-entropy source convergence, 1/√N scaling of σ, and spectrum shape — not by a single eigenvalue; quoted uncertainty confirmed against seed-replicate scatter
- **Gaussian-process surrogate for k-infinity:** 25 pcm error against the true response surface (noise deconvolved in quadrature) vs 90 pcm transport σ, at ~10⁷× lower marginal cost
- **Reactivity coefficients validated against transport runs the surrogate never saw** — Doppler 0.3σ, enrichment 0.2σ. The moderation optimum found by sweeping density and by sweeping pitch agrees to 0.06%
- **Tech:** OpenMC, scikit-learn, ENDF/B-VII.1, Docker

### ⚛️ [Reactor Transient Diagnosis](https://github.com/Romeo-5/Nuclear-Power-Plant-Accident-Diagnosis-and-Root-Cause-Analysis)
Deep learning on time-series reactor sensor data for accident detection and diagnosis

- Semi-supervised anomaly detection across **96 operational parameters** and **18 accident scenarios**
- Multi-class classification with **SHAP-based root-cause attribution**, validated against known accident physics
- **Data:** NPPAD dataset (*Nature Scientific Data*), PCTRAN PWR simulator · **Tech:** PyTorch, scikit-learn

### 🎬 [TemporalStyleNet](https://github.com/Romeo-5/Temporal-Style-Net)
Real-time video style transfer at 6.45 FPS on 1080p

- RAFT optical flow for frame-to-frame temporal consistency; trained on **118K images** with **distributed data-parallel training across 4 GPUs**
- **Tech:** PyTorch, DDP, RAFT

### 🌍 [Cross-Cultural Inspiration Coach](https://github.com/Romeo-5/Inspirational_Coach)
Fine-tuned Llama 3.2 coaching app — **Session Winner, 55th Annual Senior Design Conference**

- QLoRA PEFT for culturally-aware generation; full-stack web application
- **Tech:** Python, TypeScript, Llama, QLoRA, Firebase

---

## 🛠️ Technical Expertise

**Nuclear & Reactor Physics:** OpenMC · Monte Carlo neutron transport · k-infinity eigenvalue calculations · cross-section libraries (ENDF/B) · reactivity coefficients & Doppler feedback · single-event effects (SEE/SEB) · JESD89A

**Modeling, Simulation & UQ:** Surrogate models (Gaussian processes) · digital twins · uncertainty quantification · Latin hypercube & Sobol sampling · design of experiments · Kaplan–Meier · Weibull hazard modeling · probability calibration · numerical solvers (damped least squares, null-space methods) · Unreal Engine · MuJoCo · sim-to-real

**ML & Agents:** PyTorch · scikit-learn · Transformers · distributed training (DDP) · anomaly detection · SHAP · LLM fine-tuning (QLoRA) · tool-use architectures · local model deployment (Ollama) · production RAG

**Languages & Systems:** Python · C · SQL · C++ · Java · Shell · Linux · Docker · Git · CI/CD · FastAPI · Postgres · Elasticsearch 

---

## 📚 Publications

**Creative Collaborator: AI-facilitated UI for Creating Engaging and Insightful Memes** — *first author* | AHFE International, 2024 | [DOI: 10.54941/ahfe1005579](https://doi.org/10.54941/ahfe1005579)

**Distributed Inverse Kinematics for Modular Self-Reconfigurable Robots** — with W.-M. Shen | *in preparation, IROS 2027*

---

## 📫 Connect

[LinkedIn](https://linkedin.com/in/romeo-nickel) · rjnickel@usc.edu · Los Angeles, CA
