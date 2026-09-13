<h1 align="center">Awesome Brick Assembly 🧱 & Robot Creativity 🤖</h1>

<p align="center">
  <b>A curated collection of research on generative brick design, physical reasoning,<br>
  simulation, long-horizon planning, robotic construction, and embodied creativity.</b>
</p>

<p align="center">
  💭 Imagine &nbsp;→&nbsp; 🎨 Design &nbsp;→&nbsp; 🧪 Simulate &nbsp;→&nbsp;
  🧠 Reason &nbsp;→&nbsp; 🦾 Manipulate &nbsp;→&nbsp; 🧱 Build
</p>

<p align="center">
  <img alt="Status" src="https://img.shields.io/badge/status-actively_curated-2ea44f">
  <img alt="Brick Assembly" src="https://img.shields.io/badge/focus-brick_assembly-d62728">
  <img alt="Robot Creativity" src="https://img.shields.io/badge/focus-robot_creativity-7957d5">
  <img alt="Physical Intelligence" src="https://img.shields.io/badge/theme-physical_intelligence-007ec6">
</p>

<p align="center">
  <sub>Last updated: September 2026</sub>
</p>

---

<a id="contents"></a>

## 📚 Contents

- [🎯 Scope and Organization](#scope)
- [📖 Surveys and Overviews](#surveys)
- [🏷️ Research Tags](#tags)
- [🎨 1. Generative and Computational Brick Design](#generative-design)
- [⚖️ 2. Physics Modeling, Stability, and Simulation](#physics-simulation)
- [🧠 3. Long-Horizon Reasoning, Planning, and Assembly Understanding](#reasoning-planning)
- [🦾 4. Robotic Manipulation and Physical Construction](#robotic-construction)
- [✨ 5. Robot Creativity and Generative Physical Intelligence](#robot-creativity)
- [📦 6. Datasets, Benchmarks, and Challenges](#datasets-benchmarks)
- [🛠️ 7. Software and Tools](#software-tools)

---

<a id="scope"></a>

## 🎯 Scope and Organization

This repository studies a central Physical AI question:

> **How can AI and robots turn abstract human ideas into physically realizable objects?**

Interlocking bricks provide a challenging and accessible testbed for this goal. A complete system may need to:

- understand an abstract goal or reference;
- generate a novel object design;
- reason about geometry, connectivity, stability, and available parts;
- plan a long sequence of assembly operations;
- manipulate small components with high precision;
- monitor execution and recover from errors; and
- produce a real physical artifact.

The collection is organized into two layers:

- **Core brick intelligence:** Research that directly studies LEGO-style bricks, interlocking blocks, modular assembly, or brick-based construction.
- **Adjacent robot creativity:** Closely related research on robotic crafting, sculpting, generative fabrication, and automatic robot design.

Each paper appears once under its primary contribution. Cross-cutting contributions are represented through research tags.

[⬆️ Back to contents](#contents)

---

<a id="surveys"></a>

## 📖 Surveys and Overviews

| Year | Paper | Tags | Resources |
|---:|---|---|---|
| 2014 | **Survey on Automated LEGO Assembly Construction**<br><sub>Reviews representations, optimization objectives, stability criteria, and algorithms for converting 3D models into brick assemblies.</sub> | `🎨 Design` `⚖️ Physics` `🗺️ Planning` | [📄 Paper](https://dspace.zcu.cz/bitstream/11025/11949/1/Kim.pdf) |
| 2018 | **State of the Art on Stylized Fabrication**<br><sub>Reviews computational techniques for fabricating stylized physical objects, including brick-based representations.</sub> | `🎨 Design` `🧱 Construction` | [📄 Paper](https://doi.org/10.1111/cgf.13327) |

[⬆️ Back to contents](#contents)

---

<a id="tags"></a>

## 🏷️ Research Tags

### Research areas

| Tag | Meaning |
|---|---|
| `🎨 Design` | Generative, computational, or procedural design |
| `💬 Language` | Language-conditioned generation or interaction |
| `🖼️ Vision` | Image-conditioned generation or visual understanding |
| `📐 Geometry` | Shape representation, reconstruction, or optimization |
| `⚖️ Physics` | Stability, equilibrium, contact forces, or feasibility |
| `🧪 Simulation` | Physics engines, digital twins, or synthetic environments |
| `🧠 Reasoning` | Spatial, physical, symbolic, or multimodal reasoning |
| `🗺️ Planning` | Assembly sequencing, task planning, or motion planning |
| `👁️ Perception` | Detection, reconstruction, pose, or state estimation |
| `📖 Instructions` | Assembly-manual understanding or generation |
| `🦾 Manipulation` | Grasping, placement, insertion, or disassembly |
| `🧱 Construction` | Physical assembly or artifact construction |
| `🤲 Bimanual` | Coordinated dual-arm manipulation |
| `🤝 Multi-Robot` | Cooperative planning, allocation, or execution |
| `🎓 Demonstration` | Learning from human demonstrations |
| `🔄 Recovery` | Error detection, correction, or replanning |
| `✨ Creativity` | Open-ended generation or creative physical behavior |
| `🧑‍🤝‍🧑 Co-Creation` | Human–AI or human–robot creative collaboration |

### Resource and evaluation tags

| Tag | Meaning |
|---|---|
| `🤖 Real Robot` | Evaluated on physical robotic hardware |
| `📦 Dataset` | Introduces or releases a dataset |
| `🏆 Benchmark` | Evaluation suite, competition, or challenge |
| `💻 Open Source` | Public implementation or software release |
| ⭐ | Particularly representative work |

### Resource links

| Icon | Resource |
|---|---|
| 📄 | Paper |
| 🌐 | Project page |
| 💻 | Code |
| 📦 | Dataset |
| 🤗 | Model |
| 🎥 | Video |
| 📊 | Benchmark or leaderboard |

[⬆️ Back to contents](#contents)

---

<a id="generative-design"></a>

## 🎨 1. Generative and Computational Brick Design

> Creating physically meaningful brick structures from language, images, 3D geometry, sketches, examples, or learned distributions.

### 🧠 Foundation Models and Learned Generation

| Year | Paper | Tags | Resources |
|---:|---|---|---|
| 2026 | **BrickAnything: Geometry-Conditioned Buildable Brick Generation with Structure-Aware Tokenization**<br><sub>Generates buildable brick structures from point-cloud geometry using attachment-aware tree tokenization, constrained decoding, and adaptive rollback.</sub> | `🎨 Design` `📐 Geometry` `⚖️ Physics` | [📄 Paper](https://arxiv.org/abs/2605.26182) |
| 2026 | **BrickNet: Graph-Backed Generative Brick Assembly** — CVPR 2026<br><sub>Uses a graph-based program representation to generate assemblies containing diverse brick types and connection semantics.</sub> | `🎨 Design` `📐 Geometry` `📦 Dataset` | [📄 Paper](https://arxiv.org/abs/2604.22984) · [🌐 Project](https://kulits.github.io/BrickNet/) |
| 2025 | ⭐ **Generating Physically Stable and Buildable Brick Structures from Text (BrickGPT / LegoGPT)** — ICCV 2025, Marr Prize<br><sub>Generates physically stable brick structures from natural-language prompts using autoregressive next-brick prediction and physics-aware rollback.</sub> | `🎨 Design` `💬 Language` `⚖️ Physics` `💻 Open Source` | [📄 Paper](https://arxiv.org/abs/2505.05469) · [🌐 Project](https://avalovelace1.github.io/BrickGPT/) · [💻 Code](https://github.com/AvaLovelace1/BrickGPT) · [📦 Data](https://huggingface.co/datasets/AvaLovelace/StableText2Brick) |
| 2025 | **LegoACE: Autoregressive Construction Engine for Expressive LEGO Assemblies** — SIGGRAPH Asia 2025<br><sub>Generates expressive brick assemblies conditioned on text or multi-view normal images.</sub> | `🎨 Design` `💬 Language` `🖼️ Vision` `💻 Open Source` | [📄 Paper](https://doi.org/10.1145/3757377.3763881) · [🌐 Project](https://xh38.github.io/LegoACE/) · [💻 Code](https://github.com/VAST-AI-Research/LegoACE) · [🤗 Models](https://huggingface.co/VAST-AI/LegoACE) |
| 2025 | **LEGO-Maker: A Semantic-Driven Algorithm for Text-to-3D Generation** — ICCV 2025<br><sub>Decomposes language-conditioned generation into target-image generation, semantic decomposition, and brick-based realization.</sub> | `🎨 Design` `💬 Language` `📐 Geometry` | [📄 Paper](https://openaccess.thecvf.com/content/ICCV2025/html/Zhang_LEGO-Maker_A_Semantic-Driven_Algorithm_for_Text-to-3D_Generation_ICCV_2025_paper.html) |
| 2025 | **LEGO-Maker: Autoregressive Image-Conditioned LEGO Model Creation** — SIGGRAPH Asia 2025<br><sub>Uses compact brick tokenization, multi-token prediction, and rollback to generate detailed assemblies from images.</sub> | `🎨 Design` `🖼️ Vision` `📐 Geometry` | [📄 Paper](https://doi.org/10.1145/3763285) |
| 2024 | **Learn to Create Simple LEGO Micro Buildings** — SIGGRAPH Asia 2024<br><sub>Learns a generative representation for producing coherent LEGO micro-building designs.</sub> | `🎨 Design` `📐 Geometry` `📦 Dataset` `💻 Open Source` | [📄 Paper](https://doi.org/10.1145/3687755) · [💻 Code](https://github.com/Occulte/LEGO_Buildings_Generation) |
| 2024 | **Creating LEGO Figurines from Single Images** — SIGGRAPH 2024<br><sub>Creates personalized, physically assemblable figurines with printable decals from portrait images.</sub> | `🎨 Design` `🖼️ Vision` `🧱 Construction` | [📄 Paper](https://doi.org/10.1145/3658167) |
| 2021 | ⭐ **Brick-by-Brick: Combinatorial Construction with Deep Reinforcement Learning** — NeurIPS 2021<br><sub>Learns to assemble unseen brick objects sequentially from one or more target images while masking invalid actions.</sub> | `🎨 Design` `🖼️ Vision` `🧠 Reasoning` `🗺️ Planning` `💻 Open Source` | [📄 Paper](https://proceedings.neurips.cc/paper/2021/hash/2d4027d6df9c0256b8d4474ce88f8c88-Abstract.html) · [💻 Code](https://github.com/POSTECH-CVLab/Brick-by-Brick) |
| 2021 | **Image2Lego: Customized LEGO Set Generation from Images**<br><sub>Maps single images into voxelized 3D representations and converts them into brick models and building instructions.</sub> | `🎨 Design` `🖼️ Vision` `📐 Geometry` | [📄 Paper](https://arxiv.org/abs/2108.08477) · [🌐 Project](https://krlennon.github.io/Image2LEGO/) |
| 2020 | **Building LEGO Using Deep Generative Models of Graphs** — NeurIPS ML4Eng Workshop<br><sub>Represents assemblies as graphs and learns a sequential graph generative model from human-designed structures.</sub> | `🎨 Design` `📐 Geometry` `💻 Open Source` | [📄 Paper](https://arxiv.org/abs/2012.11543) · [💻 Code](https://github.com/uoguelph-mlrg/GenerativeLEGO) |
| 2020 | **Combinatorial 3D Shape Generation via Sequential Assembly**<br><sub>Uses Bayesian optimization to assemble volumetric primitives while considering global geometry and stability.</sub> | `🎨 Design` `📐 Geometry` `⚖️ Physics` `💻 Open Source` | [📄 Paper](https://arxiv.org/abs/2004.07414) · [💻 Code](https://github.com/POSTECH-CVLab/Combinatorial-3D-Shape-Generation) |

### 🖼️ Image-, Portrait-, and Sketch-Based Design

| Year | Paper | Tags | Resources |
|---:|---|---|---|
| 2023 | **Computational Design of LEGO Sketch Art** — SIGGRAPH Asia 2023<br><sub>Transforms input images into expressive brick-and-tile sketch models with smooth curves and salient features.</sub> | `🎨 Design` `🖼️ Vision` `📐 Geometry` | [📄 Paper](https://doi.org/10.1145/3618306) |
| 2022 | **Brick Yourself within 3 Minutes** — ICRA 2022<br><sub>Converts a portrait into a customized physical brick model and assembly instructions using an automated vending-machine-style system.</sub> | `🎨 Design` `🖼️ Vision` `🧱 Construction` `🤖 Real Robot` | [🌐 Project](https://www.unicus.cn/research/31-20.html) |
| 2019 | **Computational LEGO Technic Design** — SIGGRAPH Asia 2019<br><sub>Produces connected, structurally meaningful LEGO Technic models from sketches and optional motion annotations.</sub> | `🎨 Design` `📐 Geometry` `⚖️ Physics` | [📄 Paper](https://arxiv.org/abs/2007.02245) · [🌐 Project](https://xuhaocuhk.github.io/projects/compute_technic/) |
| 2019 | **Automatic Generation of Vivid LEGO Architectural Sculptures** — Computer Graphics Forum<br><sub>Preserves repeating elements, planar regions, and architectural details when converting buildings into brick sculptures.</sub> | `🎨 Design` `📐 Geometry` | [📄 Paper](https://doi.org/10.1111/cgf.13603) |

### 📐 Search, Optimization, and Classical Computational Design

| Year | Paper | Tags | Resources |
|---:|---|---|---|
| 2024 | **Streamlining LEGO Model Design: An Automated Optimisation Approach**<br><sub>Optimizes brick layouts to reduce design errors and improve automated model generation.</sub> | `🎨 Design` `📐 Geometry` | [📄 Paper](https://www.sciencedirect.com/science/article/pii/S2212827124009314) |
| 2018 | **Split-and-Merge-Based Genetic Algorithm for LEGO Brick Sculpture Optimization** — IEEE Access<br><sub>Uses specialized genetic operators to minimize brick count while preserving feasibility, stability, and connectivity.</sub> | `🎨 Design` `⚖️ Physics` | [📄 Paper](https://doi.org/10.1109/ACCESS.2018.2859039) |
| 2016 | **A Multi-Phase Search Approach to the LEGO Construction Problem** — SoCS<br><sub>Combines layer-level candidate generation with local search to produce connected and structurally sound layouts.</sub> | `🎨 Design` `🗺️ Planning` | [📄 Paper](https://doi.org/10.1609/socs.v7i1.18385) |
| 2015 | ⭐ **Legolization: Optimizing LEGO Designs** — SIGGRAPH Asia 2015<br><sub>Converts arbitrary 3D models into brick sculptures while jointly considering shape, color, workload, and force-based stability.</sub> | `🎨 Design` `📐 Geometry` `⚖️ Physics` | [📄 Paper](https://www.cs.columbia.edu/~yonghao/siga15/abstsiga15.html) |
| 2015 | **Finding an Optimal LEGO Brick Layout of a Voxelized 3D Object**<br><sub>Formulates brick layout generation as an optimization problem over voxelized target geometry.</sub> | `🎨 Design` `📐 Geometry` | [📄 Paper](https://doi.org/10.1145/2739480.2754667) |
| 2013 | **LEGO Builder: Automatic Generation of LEGO Assembly Manuals from 3D Polygon Models**<br><sub>Converts polygonal models into connected brick structures and automatically generates assembly instructions.</sub> | `🎨 Design` `📖 Instructions` | [📄 Paper](https://doi.org/10.3169/mta.1.354) |
| 2013 | **Automatic Generation of Constructable Brick Sculptures** — Eurographics<br><sub>Transforms voxelized meshes into stable brick sculptures and repairs weak or disconnected structures.</sub> | `🎨 Design` `⚖️ Physics` `📖 Instructions` | [📄 Paper](https://infoscience.epfl.ch/entities/publication/719977db-2ebd-44ee-8f58-1b22c7f0bdce) |
| 2003 | **Using Assembly Representations to Enable Evolutionary Design of LEGO Structures** — AIEDAM<br><sub>Introduces graph-grammar representations and evolutionary operators for automated LEGO structure design.</sub> | `🎨 Design` `📐 Geometry` | [📄 Paper](https://doi.org/10.1017/S0890060403172046) |

[⬆️ Back to contents](#contents)

---

<a id="physics-simulation"></a>

## ⚖️ 2. Physics Modeling, Stability, and Simulation

> Determining whether brick structures can exist, remain stable, sustain forces, and behave correctly during assembly or disassembly.

| Year | Paper | Tags | Resources |
|---:|---|---|---|
| 2026 | ⭐ **BrickSim: A Physics-Based Simulator for Manipulating Interlocking Brick Assemblies**<br><sub>Models snap-fit formation, connection breakage, internal forces, structural collapse, and robot interaction in real time.</sub> | `⚖️ Physics` `🧪 Simulation` `🦾 Manipulation` `💻 Open Source` | [📄 Paper](https://arxiv.org/abs/2603.16853) · [🌐 Project](https://intelligent-control-lab.github.io/BrickSim/) · [💻 Code](https://github.com/intelligent-control-lab/BrickSim) |
| 2026 | **Fourfold Is Enough: Connected LEGO Models from One Brick Type**<br><sub>Studies the theoretical scale required to reproduce connected brick models using only a single rectangular brick type.</sub> | `📐 Geometry` `⚖️ Physics` | [📄 Paper](https://arxiv.org/abs/2609.09205) |
| 2024 | ⭐ **StableLego: Stability Analysis of Block Stacking Assembly** — IEEE RA-L<br><sub>Uses rigid-block equilibrium and force-balancing optimization to classify stability and identify structurally weak regions.</sub> | `⚖️ Physics` `🧠 Reasoning` `📦 Dataset` `💻 Open Source` | [📄 Paper](https://arxiv.org/abs/2402.10711) · [💻 Code and Data](https://github.com/intelligent-control-lab/StableLego) |
| 2023 | **BrickFEM: An Automated Finite Element Model for Static and Dynamic Simulations of Simple LEGO Sets**<br><sub>Automatically constructs finite-element models for stress, strain, clamping, loading, and disassembly analysis.</sub> | `⚖️ Physics` `🧪 Simulation` | [📄 Paper](https://engrxiv.org/preprint/view/2898) |

### Central physical constraints

- stud–tube and snap-fit connectivity;
- gravity and static equilibrium;
- friction and contact-force distribution;
- insertion and extraction forces;
- structural strength and weak-point localization;
- collision-free intermediate configurations;
- inventory and resource constraints;
- robot reachability and manipulation feasibility; and
- dynamic collapse and connection breakage.

[⬆️ Back to contents](#contents)

---

<a id="reasoning-planning"></a>

## 🧠 3. Long-Horizon Reasoning, Planning, and Assembly Understanding

> Understanding assembly state, interpreting instructions, reasoning about spatial and physical relationships, and planning extended construction sequences.

### 🧠 Spatial and Physical Reasoning

| Year | Paper | Tags | Resources |
|---:|---|---|---|
| 2026 | **Brick-Composer: Using MLLMs for Assembly with Diverse Bricks**<br><sub>Introduces BC-Bench and trains multimodal language models for fine-grained brick selection and pose estimation.</sub> | `🧠 Reasoning` `🖼️ Vision` `🗺️ Planning` `🏆 Benchmark` | [📄 Paper](https://arxiv.org/abs/2606.05445) |
| 2026 | **Sample-Efficient Post-Training for LEGO Spatial-Physics Reasoning**<br><sub>Studies failures where physically valid generations remain semantically or geometrically incorrect and introduces data selection and preference optimization.</sub> | `🧠 Reasoning` `⚖️ Physics` `💬 Language` | [📄 Paper](https://arxiv.org/abs/2606.07602) |
| 2026 | **WorkBenchMark: A LEGO-Based Assembly Benchmark with an Assembly-by-Disassembly Baseline for the Smart Manufacturing League**<br><sub>Provides 400 Duplo assembly tasks across four complexity levels with perception, symbolic reasoning, simulation, and baseline methods.</sub> | `🧠 Reasoning` `🗺️ Planning` `👁️ Perception` `🏆 Benchmark` | [📄 Paper](https://arxiv.org/abs/2606.19358) |
| 2025 | **LEGO-Puzzles: How Good Are MLLMs at Multi-Step Spatial Reasoning?**<br><sub>Evaluates multimodal models on 1,100 visual questions covering spatial understanding and multi-step reasoning.</sub> | `🧠 Reasoning` `🖼️ Vision` `🏆 Benchmark` | [📄 Paper](https://arxiv.org/abs/2503.19990) |
| 2025 | **LEGO Co-builder: Exploring Fine-Grained Vision-Language Modeling for Multimodal LEGO Assembly Assistants** — ICMI 2026<br><sub>Evaluates instruction following, object recognition, and assembly-state detection in multimodal assembly scenes.</sub> | `🧠 Reasoning` `👁️ Perception` `📖 Instructions` `🏆 Benchmark` | [📄 Paper](https://arxiv.org/abs/2507.05515) |

### 🗺️ Assembly Sequence and Task Planning

| Year | Paper | Tags | Resources |
|---:|---|---|---|
| 2025 | **AssemblyComplete: 3D Combinatorial Construction with Deep Reinforcement Learning** — ACC 2025<br><sub>Infers the intended object from a partial assembly and plans physically valid actions to complete missing regions.</sub> | `🧠 Reasoning` `🗺️ Planning` `⚖️ Physics` | [📄 Paper](https://arxiv.org/abs/2410.15469) |
| 2024 | ⭐ **Physics-Aware Combinatorial Assembly Sequence Planning Using Data-Free Action Masking**<br><sub>Uses reinforcement learning and online physics-aware action masking to produce physically executable assembly sequences.</sub> | `🗺️ Planning` `⚖️ Physics` `🧠 Reasoning` `💻 Open Source` | [📄 Paper](https://arxiv.org/abs/2408.10162) |
| 2024 | **TreeSBA: Tree-Transformer for Self-Supervised Sequential Brick Assembly** — ECCV 2024<br><sub>Predicts assembly actions from multi-view images using a LEGO-tree representation and synthetic-to-real self-supervision.</sub> | `🗺️ Planning` `🖼️ Vision` `📐 Geometry` `💻 Open Source` | [📄 Paper](https://arxiv.org/abs/2407.15648) · [🌐 Project](https://dreamguo.github.io/projects/TreeSBA/) · [💻 Code](https://github.com/dreamguo/TreeSBA) |
| 2022 | **Planning Assembly Sequence with Graph Transformer**<br><sub>Represents assemblies using heterogeneous graphs and predicts construction sequences with graph attention.</sub> | `🗺️ Planning` `🧠 Reasoning` | [📄 Paper](https://arxiv.org/abs/2210.05236) |
| 2022 | **Blocks Assemble! Learning to Assemble with Large-Scale Structured Reinforcement Learning** — ICML 2022<br><sub>Studies structured reinforcement learning for sequential construction using block-based assembly environments.</sub> | `🗺️ Planning` `🧪 Simulation` | [📄 Paper](https://proceedings.mlr.press/v162/ghasemipour22a.html) |

### 📖 Manual Understanding and Instruction Generation

| Year | Paper | Tags | Resources |
|---:|---|---|---|
| 2024 | **Learning to Build by Building Your Own Instructions**<br><sub>Lets an agent disassemble an unseen model, save visual intermediate states, and use the resulting instruction book to rebuild it.</sub> | `🧠 Reasoning` `📖 Instructions` `🎓 Demonstration` | [📄 Paper](https://arxiv.org/abs/2410.01111) |
| 2022 | ⭐ **Translating a Visual LEGO Manual to a Machine-Executable Plan** — ECCV 2022<br><sub>Introduces MEPNet for converting illustrated assembly manuals into structured, machine-executable 3D plans.</sub> | `📖 Instructions` `👁️ Perception` `🗺️ Planning` `💻 Open Source` | [📄 Paper](https://arxiv.org/abs/2207.12572) · [🌐 Project](https://cs.stanford.edu/~rcwang/projects/lego_manual/) · [💻 Code](https://github.com/Relento/lego_release) |

### 👁️ State Estimation, Error Detection, and Reconstruction

| Year | Paper | Tags | Resources |
|---:|---|---|---|
| 2024 | **SCANet: Correcting LEGO Assembly Errors with Self-Correct Assembly Network** — IROS 2024<br><sub>Detects incorrectly assembled components and predicts corrective actions using manual images and partial assemblies.</sub> | `👁️ Perception` `🧠 Reasoning` `🔄 Recovery` `📦 Dataset` | [📄 Paper](https://arxiv.org/abs/2403.18195) · [🌐 Project](https://scanet-iros2024.github.io/) |
| 2023 | **MobileBrick: Building LEGO for 3D Reconstruction on Mobile Devices** — CVPR 2023<br><sub>Introduces a multi-view mobile RGB-D dataset with precise geometry for detailed object reconstruction.</sub> | `👁️ Perception` `📐 Geometry` `📦 Dataset` `💻 Open Source` | [📄 Paper](https://arxiv.org/abs/2303.01932) · [🌐 Project](https://code.active.vision/MobileBrick/) · [💻 Code](https://github.com/ActiveVisionLab/MobileBrick) |
| 2022 | ⭐ **Break and Make: Interactive Structural Understanding Using LEGO Bricks** — ECCV 2022<br><sub>Introduces an interactive task in which an agent inspects and disassembles a model before reconstructing it from scratch.</sub> | `🧠 Reasoning` `👁️ Perception` `🧪 Simulation` `💻 Open Source` | [📄 Paper](https://arxiv.org/abs/2207.13738) · [💻 Simulator](https://github.com/aaronwalsman/ltron) · [💻 Training Code](https://github.com/aaronwalsman/ltron-torch-eccv22) |

[⬆️ Back to contents](#contents)

---

<a id="robotic-construction"></a>

## 🦾 4. Robotic Manipulation and Physical Construction

> Executing precise, contact-rich, long-horizon assembly and disassembly using physical robots.

### 🤲 Long-Horizon, Bimanual, and Multi-Robot Assembly

| Year | Paper | Tags | Resources |
|---:|---|---|---|
| 2026 | ⭐ **BrickCraft: Visuomotor Skill Composition with Situated Manual Guidance for Long-Horizon Interlocking Brick Assembly**<br><sub>Composes reusable visuomotor skills using situated manuals that project assembly intent into current robot observations.</sub> | `🦾 Manipulation` `📖 Instructions` `🗺️ Planning` `🤖 Real Robot` | [📄 Paper](https://arxiv.org/abs/2605.07605) · [🌐 Project](https://intelligent-control-lab.github.io/BrickCraft/) |
| 2025 | ⭐ **APEX-MR: Multi-Robot Asynchronous Planning and Execution for Cooperative Assembly** — RSS 2025<br><sub>Coordinates task, motion, and asynchronous execution for safe and efficient cooperative brick assembly.</sub> | `🤝 Multi-Robot` `🤲 Bimanual` `🗺️ Planning` `🤖 Real Robot` `💻 Open Source` | [📄 Paper](https://arxiv.org/abs/2503.15836) · [💻 Code](https://github.com/intelligent-control-lab/APEX-MR) |

### 🦾 Precision Manipulation and End Effectors

| Year | Paper | Tags | Resources |
|---:|---|---|---|
| 2025 | **Eye-in-Finger: Smart Fingers for Delicate Assembly and Disassembly of LEGO** — IROS 2025<br><sub>Embeds high-resolution cameras at the tool tip for submillimeter alignment and closed-loop error correction.</sub> | `🦾 Manipulation` `👁️ Perception` `🔄 Recovery` `🤖 Real Robot` | [📄 Paper](https://arxiv.org/abs/2503.06848) |
| 2024 | **A Lightweight and Transferable Design for Robust LEGO Manipulation** — ISFA 2024<br><sub>Combines a transferable end-of-arm tool with safe motion optimization for repeatable assembly and disassembly.</sub> | `🦾 Manipulation` `🤖 Real Robot` | [📄 Paper](https://arxiv.org/abs/2309.02354) |

### 🎓 Learning from Human Demonstration

| Year | Paper | Tags | Resources |
|---:|---|---|---|
| 2023 | **Simulation-Aided Learning from Demonstration for Robotic LEGO Construction**<br><sub>Extracts construction plans from human demonstrations and validates them in simulation before physical deployment.</sub> | `🎓 Demonstration` `🧪 Simulation` `🗺️ Planning` `🤖 Real Robot` | [📄 Paper](https://arxiv.org/abs/2309.11010) |
| 2023 | **Robotic LEGO Assembly and Disassembly from Human Demonstration**<br><sub>Learns assembly and disassembly sequences from human demonstrations, verifies them using a digital twin, and executes them with an industrial robot.</sub> | `🎓 Demonstration` `🦾 Manipulation` `🧪 Simulation` `🤖 Real Robot` `💻 Open Source` | [📄 Paper](https://arxiv.org/abs/2305.15667) · [💻 Code](https://github.com/intelligent-control-lab/Robotic_LEGO_Assembly_and_Disassembly_from_Human_Demonstration) |

### Key manipulation challenges

- submillimeter alignment;
- tight geometric tolerances;
- press-fit insertion and extraction;
- force- and vision-guided correction;
- grasping from clutter;
- occlusion near the contact point;
- collision-free access to partial structures;
- bimanual coordination and robot handoffs;
- accumulated error over long task horizons; and
- failure detection and recovery.

[⬆️ Back to contents](#contents)

---

<a id="robot-creativity"></a>

## ✨ 5. Robot Creativity and Generative Physical Intelligence

> Systems that interpret open-ended intent, generate new designs or goals, reason about physical feasibility, and realize creative outcomes through embodied action.

### ✨ Generative Physical Realization

| Year | Paper | Tags | Resources |
|---:|---|---|---|
| 2026 | ⭐ **Prompt-to-Product: Generative Assembly via Bimanual Manipulation** — IEEE Robotics & Automation Magazine<br><sub>Transforms a natural-language idea into a stable brick design, plans hundreds of operations, and constructs the resulting product with a bimanual robot.</sub> | `✨ Creativity` `💬 Language` `🎨 Design` `🤲 Bimanual` `🧱 Construction` `🤖 Real Robot` | [📄 Paper](https://arxiv.org/abs/2508.21063) · [🌐 Project](https://prompt2product.github.io/) |
| 2024 | **Text2Robot: Evolutionary Robot Design from Text Descriptions**<br><sub>Transforms language specifications into manufacturable quadrupedal robot designs using generative 3D models and body-control co-optimization.</sub> | `✨ Creativity` `💬 Language` `🎨 Design` `⚖️ Physics` | [📄 Paper](https://arxiv.org/abs/2406.19963) · [🌐 Project](https://generalroboticslab.com/Text2Robot/) |
| 2023 | **DiffuseBot: Breeding Soft Robots with Physics-Augmented Generative Diffusion Models** — NeurIPS 2023<br><sub>Generates soft-robot morphologies while incorporating differentiable physical simulation and control performance.</sub> | `✨ Creativity` `🎨 Design` `⚖️ Physics` `🧪 Simulation` | [📄 Paper](https://arxiv.org/abs/2311.17053) · [🌐 Project](https://diffusebot.github.io/) |
| 2020 | **RoboGrammar: Graph Grammar for Terrain-Optimized Robot Design** — SIGGRAPH Asia 2020<br><sub>Uses a graph grammar and learned search strategy to automatically generate robot morphologies for target terrains.</sub> | `✨ Creativity` `🎨 Design` `🧪 Simulation` | [🌐 Project](https://people.csail.mit.edu/jiex/papers/robogrammar/) |

### 🏺 Robotic Crafting, Sculpting, and Making

| Year | Paper | Tags | Resources |
|---:|---|---|---|
| 2024 | **LLM-Craft: Robotic Crafting of Elasto-Plastic Objects with Large Language Models**<br><sub>Uses multimodal language-model reasoning to iteratively shape clay toward geometric and semantic goals.</sub> | `✨ Creativity` `💬 Language` `🧠 Reasoning` `🤖 Real Robot` | [📄 Paper](https://arxiv.org/abs/2406.08648) · [🌐 Project](https://sites.google.com/andrew.cmu.edu/llmcraft) |
| 2024 | **SculptDiff: Learning Robotic Clay Sculpting from Humans with Goal-Conditioned Diffusion Policy**<br><sub>Learns goal-conditioned sculpting policies from demonstrations using point-cloud observations and diffusion models.</sub> | `✨ Creativity` `🎓 Demonstration` `🦾 Manipulation` `🤖 Real Robot` | [📄 Paper](https://arxiv.org/abs/2403.10401) · [🌐 Project](https://sites.google.com/andrew.cmu.edu/imitation-sculpting/home) |
| 2024 | **RoPotter: Toward Robotic Pottery and Deformable Object Manipulation with Structural Priors**<br><sub>Investigates robotic pottery through perception, manipulation, and structural priors for deformable material shaping.</sub> | `✨ Creativity` `⚖️ Physics` `🦾 Manipulation` `🤖 Real Robot` | [📄 Paper](https://arxiv.org/abs/2408.02184) |
| 2023 | **RoboCook: Long-Horizon Elasto-Plastic Object Manipulation with Diverse Tools** — CoRL 2023<br><sub>Combines learned dynamics, tool selection, and long-horizon planning to create food products such as dumplings and cookies.</sub> | `✨ Creativity` `🧠 Reasoning` `🗺️ Planning` `🤖 Real Robot` | [📄 Paper](https://arxiv.org/abs/2306.14447) |
| 2023 | **SculptBot: Pre-Trained Models for 3D Deformable Object Manipulation** — ICRA 2024<br><sub>Uses pre-trained point-cloud representations and model-based planning to sculpt clay into target shapes.</sub> | `✨ Creativity` `📐 Geometry` `🦾 Manipulation` `🤖 Real Robot` | [📄 Paper](https://arxiv.org/abs/2309.08728) · [🌐 Project](https://sites.google.com/andrew.cmu.edu/sculptbot) |
| 2022 | **RoboCraft: Learning to See, Simulate, and Shape Elasto-Plastic Objects with Graph Networks** — RSS 2022<br><sub>Learns particle-based dynamics from RGB-D observations and plans actions that shape deformable materials into unseen target geometries.</sub> | `✨ Creativity` `👁️ Perception` `⚖️ Physics` `🤖 Real Robot` | [📄 Paper](https://arxiv.org/abs/2205.02909) |
| 2022 | **DALL-E-Bot: Introducing Web-Scale Diffusion Models to Robotics**<br><sub>Uses a generative image model to imagine natural object arrangements and then physically realizes the generated scenes.</sub> | `✨ Creativity` `💬 Language` `🖼️ Vision` `🤖 Real Robot` | [📄 Paper](https://arxiv.org/abs/2210.02438) |

### What counts as robot creativity?

A system is especially relevant when it supports one or more of:

- **Open-ended intent:** the desired output is not fully specified in advance.
- **Generative design:** the system creates a new object, structure, or morphology.
- **Physical grounding:** generated ideas are evaluated against geometry and physics.
- **Embodied realization:** the system turns a virtual concept into a physical result.
- **Adaptation:** the robot responds to uncertainty, failure, or changing goals.
- **Co-creation:** humans and robots iteratively develop and construct an idea together.

[⬆️ Back to contents](#contents)

---

<a id="datasets-benchmarks"></a>

## 📦 6. Datasets, Benchmarks, and Challenges

All brick-related datasets, evaluation suites, and competitions are consolidated here.

### 🎨 Generative Design and Structural Data

| Resource | Year | Description | Tags | Access |
|---|---:|---|---|---|
| **BrickNet Dataset** | 2026 | More than 100,000 human-designed LDraw objects and scenes with diverse parts and connection types. | `🎨 Design` `📐 Geometry` `📦 Dataset` | [🌐 Project](https://kulits.github.io/BrickNet/) |
| **StableText2Brick** | 2025 | More than 47,000 stable brick structures representing over 28,000 unique objects with text descriptions. | `💬 Language` `⚖️ Physics` `📦 Dataset` | [📦 Data](https://huggingface.co/datasets/AvaLovelace/StableText2Brick) |
| **StableLego** | 2024 | More than 50,000 objects with brick layouts and corresponding structural-stability inference. | `⚖️ Physics` `📦 Dataset` | [📦 Data](https://github.com/intelligent-control-lab/StableLego) |
| **LEGO Micro-Buildings** | 2024 | Structured micro-building models for learned LEGO generation. | `🎨 Design` `📐 Geometry` `📦 Dataset` | [💻 Repository](https://github.com/Occulte/LEGO_Buildings_Generation) |
| **Combinatorial 3D Shape Generation Dataset** | 2020 | Primitive-based 3D objects for sequential combinatorial construction. | `🎨 Design` `🗺️ Planning` `📦 Dataset` | [💻 Repository](https://github.com/POSTECH-CVLab/Combinatorial-3D-Shape-Generation) |
| **LDraw Official Model Repository** | Ongoing | Community-maintained digital models of official brick sets represented using LDraw. | `📐 Geometry` `📦 Dataset` | [📦 Repository](https://omr.ldraw.org/) |

### 🧠 Reasoning, Planning, and Assembly Understanding

| Resource | Year | Description | Tags | Access |
|---|---:|---|---|---|
| **BC-Bench** | 2026 | Evaluates multimodal models on diverse-brick selection and fine-grained placement-pose estimation. | `🧠 Reasoning` `🖼️ Vision` `🏆 Benchmark` | [📄 Paper](https://arxiv.org/abs/2606.05445) |
| **WorkBenchMark** | 2026 | Four hundred Duplo-based robotic assembly tasks across four levels of complexity. | `🗺️ Planning` `👁️ Perception` `🏆 Benchmark` | [📄 Paper](https://arxiv.org/abs/2606.19358) |
| **LEGO Co-builder** | 2025 | Stepwise visual scenes and procedural instructions for evaluating multimodal assembly assistants. | `🧠 Reasoning` `📖 Instructions` `🏆 Benchmark` | [📄 Paper](https://arxiv.org/abs/2507.05515) |
| **LEGO-Puzzles** | 2025 | 1,100 visual question-answering examples covering 11 spatial and sequential reasoning tasks. | `🧠 Reasoning` `🖼️ Vision` `🏆 Benchmark` | [📄 Paper](https://arxiv.org/abs/2503.19990) |
| **LEGO-ECA** | 2024 | Assembly manuals, partial builds, failure examples, and corrective labels for error detection. | `👁️ Perception` `🔄 Recovery` `📦 Dataset` | [🌐 Project](https://scanet-iros2024.github.io/) |
| **LTRON / Break and Make** | 2022 | Interactive simulator and collection of fan-designed assemblies for disassembly and reconstruction. | `🧠 Reasoning` `🧪 Simulation` `🏆 Benchmark` | [💻 Simulator](https://github.com/aaronwalsman/ltron) |
| **MEPNet LEGO Manuals** | 2022 | Three visual-manual datasets for translating illustrated instructions into executable assembly plans. | `📖 Instructions` `🗺️ Planning` `📦 Dataset` | [💻 Repository](https://github.com/Relento/lego_release) |

### 👁️ Perception and Reconstruction

| Resource | Year | Description | Tags | Access |
|---|---:|---|---|---|
| **MobileBrick** | 2023 | Multi-view mobile RGB-D captures of 153 brick sets with precise 3D annotations. | `👁️ Perception` `📐 Geometry` `📦 Dataset` | [🌐 Project](https://code.active.vision/MobileBrick/) · [💻 Code](https://github.com/ActiveVisionLab/MobileBrick) |
| **Photos and Rendered Images of LEGO Bricks** | 2023 | Large-scale collection containing real photographs and synthetic renders of individual brick types. | `👁️ Perception` `📦 Dataset` | [📄 Dataset Paper](https://doi.org/10.1038/s41597-023-02682-2) |
| **B200 LEGO Detection Dataset** | 2024 | Synthetic detection dataset covering 200 brick classes. | `👁️ Perception` `📦 Dataset` | [📦 Data](https://www.kaggle.com/datasets/ronanpickell/b100-lego-detection-dataset) |
| **B200C LEGO Classification Dataset** | 2021 | Approximately 800,000 synthetic images covering 200 commonly used brick classes. | `👁️ Perception` `📦 Dataset` | [📦 Data](https://www.kaggle.com/datasets/ronanpickell/b200c-lego-classification-dataset) · [💻 Generator](https://github.com/korra-pickell/LEGO-Classification-Dataset) |

### 🏆 Challenges

| Challenge | Focus | Tags | Access |
|---|---|---|---|
| **RoCo: Robotic Collaborative Assembly Challenge** | Long-horizon reasoning, physics understanding, dexterous manipulation, generalization, and multi-robot assembly. | `🏆 Benchmark` `🗺️ Planning` `🤲 Bimanual` `🤖 Real Robot` | [🌐 Website](https://rocochallenge.github.io/RoCo-IROS2026/) |

### Suggested evaluation dimensions

- geometric and semantic fidelity;
- structural stability and connectivity;
- collision-free buildability;
- inventory and resource compliance;
- assembly-sequence validity;
- success on unseen structures;
- step-level and full-assembly success;
- manipulation precision;
- long-horizon completion;
- error detection and recovery;
- sim-to-real transfer;
- bimanual or multi-robot efficiency; and
- human-rated creativity and intent alignment.

[⬆️ Back to contents](#contents)

---

<a id="software-tools"></a>

## 🛠️ 7. Software and Tools

### 🧪 Simulation and Physical Reasoning

| Tool | Purpose | Access |
|---|---|---|
| **BrickSim** | Real-time simulation of snap-fit connections, assembly, disassembly, collapse, and robot interaction. | [💻 GitHub](https://github.com/intelligent-control-lab/BrickSim) |
| **StableLego** | Optimization-based structural-stability analysis and weak-region localization. | [💻 GitHub](https://github.com/intelligent-control-lab/StableLego) |
| **LTRON** | Interactive environment for brick assembly, disassembly, and structural-understanding tasks. | [💻 GitHub](https://github.com/aaronwalsman/ltron) |

### 🎨 Generative Design

| Tool | Purpose | Access |
|---|---|---|
| **BrickGPT** | Language-conditioned generation of stable brick structures. | [💻 GitHub](https://github.com/AvaLovelace1/BrickGPT) |
| **LegoACE** | Text- and image-conditioned autoregressive assembly generation. | [💻 GitHub](https://github.com/VAST-AI-Research/LegoACE) |
| **BrickNet** | Graph-backed generative modeling with diverse parts and connection types. | [🌐 Project](https://kulits.github.io/BrickNet/) |
| **GenerativeLEGO** | Graph-neural-network models for sequential assembly generation. | [💻 GitHub](https://github.com/uoguelph-mlrg/GenerativeLEGO) |
| **Brick-by-Brick** | Reinforcement-learning framework for image-conditioned combinatorial construction. | [💻 GitHub](https://github.com/POSTECH-CVLab/Brick-by-Brick) |
| **Combinatorial 3D Shape Generation** | Bayesian-optimization framework for sequential primitive assembly. | [💻 GitHub](https://github.com/POSTECH-CVLab/Combinatorial-3D-Shape-Generation) |

### 🧠 Planning and Assembly Understanding

| Tool | Purpose | Access |
|---|---|---|
| **APEX-MR** | Multi-robot planning and asynchronous execution for cooperative assembly. | [💻 GitHub](https://github.com/intelligent-control-lab/APEX-MR) |
| **BrickCraft** | Situated manual guidance and visuomotor skill composition for long-horizon assembly. | [🌐 Project](https://intelligent-control-lab.github.io/BrickCraft/) |
| **MEPNet** | Translation of visual assembly manuals into machine-executable plans. | [💻 GitHub](https://github.com/Relento/lego_release) |
| **SCANet** | Detection and correction of brick assembly errors. | [🌐 Project](https://scanet-iros2024.github.io/) |
| **TreeSBA** | Self-supervised prediction of sequential assembly actions from multi-view images. | [💻 GitHub](https://github.com/dreamguo/TreeSBA) |

### 📐 Brick Representation and CAD

| Tool | Purpose | Access |
|---|---|---|
| **LDraw** | Open file format and parts library for representing brick models. | [🌐 Website](https://www.ldraw.org/) |
| **LDraw Official Model Repository** | Collection of community-recreated official set models. | [📦 Repository](https://omr.ldraw.org/) |
| **LeoCAD** | Open-source CAD editor built around the LDraw ecosystem. | [🌐 Website](https://www.leocad.org/) |
| **BrickLink Studio** | Brick CAD, rendering, instruction generation, and part-inventory tools. | [🌐 Website](https://www.bricklink.com/v3/studio/download.page) |
| **BrickHub** | Repository for sharing original digital brick models. | [🌐 Website](https://brickhub.org/) |

---

<p align="center">
  <b>From imagination to physical creation—one brick at a time.</b>
</p>