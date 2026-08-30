# Hi, I'm Romeo! 👋

**🎓 MS CS (AI) @ USC · Graduating May 2027 | 🤖 Robotics Research @ USC ISI | ⚡ Failure Analysis @ Bloom Energy**

I build the machine learning layer for physical systems where being wrong is expensive: robots, energy servers, reactors. Different hardware, one question: how much behavior can a model learn without abandoning the physics that governs it?

---

## 🔬 Current Research & Work

**@ USC Information Sciences Institute — Polymorphic Robotics Lab** *(Sep 2025 – present)*
- Developing a **distributed inverse kinematics algorithm** for modular self-reconfigurable robots: each module runs its own local solver and coordinates by message passing over the physical connection graph, applying damped least squares to its local Jacobian column. No single controller needs the full kinematic chain
- Moved constraint enforcement out of a global controller into individual modules, making the solver **morphology-agnostic**: the same algorithm runs on arbitrary assembled topologies without re-deriving kinematics
- Engineered closed-loop IK solvers using real-time physics readback to counteract gravity-induced joint sag in multi-link modular systems
- Tuned high-fidelity physics constraints in Unreal Engine 5, correcting unit-scale inertia calculations to achieve critical damping for reconfigurable modules
- Built the simulation environments (Unreal Engine, MuJoCo) and sim-to-real pipelines validating the work on physical SuperBot hardware
- Paper in preparation, targeting ICRA/IROS

**@ Bloom Energy — Failure Analysis, Quality & Reliability** *(Summer 2026)*
- Proposed and built a **locally-hosted conversational agent** (Ollama) with a **tool-use architecture**, providing natural-language access to the fleet-intelligence platform: pulling telemetry, running component-health algorithms, computing reliability analytics. Self-hosted by design so proprietary data never leaves company infrastructure
- Wired detection algorithms into a **config-file-driven CLI** so analyses run without code changes, then deployed the repo and trained the team's specialists to run and tune it themselves
- Scaled a telemetry-based failure detector for DC-DC power converters to the full confirmed-failure population: **recall 82.2% → 92.5%, zero new false positives, ~27-day median detection lead**
- Owned a solo failure-analysis investigation end to end (reliability modeling through physical flow-bench testing) and presented it at the company-wide review
- Researched **single-event effects (SEE)** device physics and neutron detection instrumentation to support a radiation-effects test campaign

**@ LineSlip Solutions** *(2024 – 2026)*
- Production **RAG** pipeline on Llama 3.1-8B with Elasticsearch retrieval and custom reranking, serving **10K+ queries/day**
- 35% accuracy improvement over baseline; 40% latency reduction via INT8 quantization

---

## 💡 Research Interests

Applying AI and optimization to hard tech problems where physics constrains the solution:

- ⚛️ **Nuclear Energy** — reactor modeling & simulation, digital twins, surrogate models, fault diagnosis
- 🔋 **Energy Systems** — fuel cell degradation, predictive maintenance, fleet reliability
- 🤖 **Robotics & Autonomy** — distributed control, modular self-reconfigurable systems, sim-to-real
- 🧪 **Physics-Informed ML** — learning dynamics without discarding the governing physics

---

## 📌 Featured Projects

### ⚛️ [Nuclear Power Plant Fault Diagnosis & Root Cause Analysis](https://github.com/Romeo-5/Nuclear-Power-Plant-Accident-Diagnosis-and-Root-Cause-Analysis)
Deep learning on time-series reactor sensor data for accident detection and diagnosis

- Semi-supervised anomaly detection across **96 operational parameters** and **18 accident scenarios**
- Autoencoder, LSTM, and Transformer architectures
- Multi-class accident classification with **SHAP-based root cause attribution**, validated against known accident physics
- **Data:** NPPAD dataset (*Nature Scientific Data*) from the PCTRAN PWR simulator
- **Tech:** PyTorch, pandas, scikit-learn

### 🎬 [TemporalStyleNet](https://github.com/Romeo-5/Temporal-Style-Net) — Real-Time Video Style Transfer
Video processing achieving 6.45 FPS on 1080p

- RAFT optical flow for temporal consistency and ego-motion estimation
- Trained on **118K MS-COCO images** using **distributed PyTorch DDP** across 4 GPUs
- **Tech:** PyTorch, RAFT, computer vision

### 🤖 Modular Robot Coordination (USC ISI)
Distributed inverse kinematics for modular self-reconfigurable robots

- Per-module local solvers with neighbor message passing; damped least squares on local Jacobian columns
- Null-space redundancy resolution for joint-limit avoidance; potential-field obstacle avoidance
- Simulation-to-hardware deployment on physical SuperBot modules
- **Tech:** Python, NumPy, SciPy, Unreal Engine, MuJoCo

### 🌍 [Cross-Cultural Inspiration Coach](https://github.com/Romeo-5/Inspirational_Coach)
AI coaching with a fine-tuned Llama 3.2 — **Session Winner, 55th Annual Senior Design Conference**

- QLoRA PEFT for culturally-aware content generation
- Full-stack web application with goal tracking
- **Tech:** Python, TypeScript, Llama, QLoRA, Firebase

---

## 🛠️ Technical Expertise

**Core:** Physics-Informed ML · Distributed Optimization · Time-Series Analysis · Anomaly Detection · Digital Twins & Surrogate Modeling

**Languages:** Python · SQL · C/C++ · Java · R · Shell

**ML/AI:** PyTorch · scikit-learn · Transformers · sentence-transformers · Distributed Training (DDP) · LLM fine-tuning (QLoRA/PEFT) · Quantization

**Agents & LLM Systems:** Tool-use architectures · Local model deployment (Ollama) · Production RAG · Retrieval + reranking · Semantic clustering

**Reliability & Physics:** Kaplan–Meier · Weibull hazard modeling · Probability calibration · Single-event effects (SEE/SEB) · JESD89A · Neutron flux modeling

**Simulation & Robotics:** Unreal Engine · MuJoCo · Inverse kinematics · Sim-to-real · Multi-agent coordination

**Production:** FastAPI · Elasticsearch · Postgres · Docker · CI/CD · Git · Linux

---

## 🏆 Highlights

- 📝 First-author publication at **AHFE Hawaii 2024** — AI-facilitated creative interfaces
- ⚛️ ML fault diagnosis for nuclear reactor transients (NPPAD / PCTRAN)
- 🤖 Distributed IK for modular self-reconfigurable robots; paper targeting ICRA/IROS
- 🔧 Built and deployed an agentic system on locally-hosted models for an industrial reliability team
- ⚡ Production ML serving 10K+ queries/day
- 🥇 Session Winner, 55th Annual Senior Design Conference — Santa Clara University

---

## 📚 Publications

**Creative Collaborator: AI-facilitated UI for Creating Engaging and Insightful Memes**
*First Author* | AHFE Hawaii 2024 | [DOI: 10.54941/ahfe1005579](https://doi.org/10.54941/ahfe1005579)

**Distributed Inverse Kinematics for Modular Self-Reconfigurable Robots**
*with W.-M. Shen* | In preparation, ICRA/IROS

---

## 📫 Connect

- 💼 [LinkedIn](https://linkedin.com/in/romeo-nickel)
- 📧 rjnickel@usc.edu
- 📍 Los Angeles, CA
