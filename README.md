# Awesome Brick Assembly <img src="assets/brick-assembly.svg" alt="LEGO-style brick assembly" width="40" height="40" align="absmiddle"> & Robot Creativity 🤖

Brick assembly has drawn increasing research attention in recent years because it combines several challenges central to Physical AI:

- **Semantic interpretation:** translating abstract design goals into concrete assembly requirements.
- **Physical reasoning:** accounting for geometry, contact, and structural stability.
- **Generalization:** adapting to diverse brick configurations and previously unseen tasks.
- **Planning over long horizons:** sequencing many interdependent assembly actions.
- **Precise manipulation:** handling miniature components within tight tolerances while preserving fragile connections.

Each challenge is a research problem in its own right. Their combination makes brick assembly a unified, accessible, and reproducible testbed for Physical AI.

This repository curates research papers on generative brick assembly design, physics modeling and simulation, reasoning and planning, robotic manipulation, and robot creativity. It also links to publicly available datasets, benchmarks, software tools, and demos.

<a id="contents"></a>

## Contents

- [Surveys and Reviews](#surveys)
- [1. Generative Design](#brick-design)
- [2. Physics Modeling and Simulation](#physics-modeling-simulation)
- [3. Reasoning and Planning](#reasoning-planning)
- [4. Robotic Manipulation](#robotic-manipulation)
- [5. Robot Creativity](#robot-creativity)
- [Datasets and Benchmarks](#datasets-benchmarks)
- [Tools and Demos](#tools-demos)

<a id="surveys"></a>

## Surveys and Reviews

Each review below discusses LEGO construction directly; the focus column distinguishes dedicated coverage from broader surveys.

| Year | Paper | Focus | Links |
|---:|---|---|---|
| 2021 | **State of the Art on Computational Design of Assemblies with Rigid Parts** | Surveys computational methods for designing rigid-part assemblies, including LEGO construction and structural stability. | [Paper](https://doi.org/10.1111/cgf.142660) |
| 2018 | **State of the Art on Stylized Fabrication** | Reviews computational methods for fabricating stylized objects, including LEGO model design and stability. | [Paper](https://doi.org/10.1111/cgf.13327) |
| 2014 | **Survey on Automated LEGO Assembly Construction** | Surveys algorithms for converting target shapes into connected, buildable LEGO brick layouts. | [Paper](https://dspace.zcu.cz/bitstream/11025/11949/1/Kim.pdf) |

[Back to contents](#contents)

<a id="brick-design"></a>
<a id="generative-design"></a>

## 1. Generative Design

Generate and optimize brick assembly structures from text, images, geometry, or other starting points.

### From Text

| Year | Paper | Focus | Links |
|---:|---|---|---|
| 2026 | **BrickNet: Graph-Backed Generative Brick Assembly** (also supports unconditional generation) — CVPR 2026 | Introduces a connectivity-based graph representation for generating valid build sequences with thousands of brick types. | [Paper](https://arxiv.org/abs/2604.22984) · [Project](https://kulits.github.io/BrickNet/) |
| 2025 | ★ **Generating Physically Stable and Buildable Brick Structures from Text (BrickGPT / LegoGPT)** — ICCV 2025, [Best Paper (Marr Prize)](https://www.thecvf.com/?page_id=413) | Generates text-conditioned brick structures with an autoregressive model and physics-aware checks that reject unstable placements. | [Paper](https://arxiv.org/abs/2505.05469) · [Project](https://avalovelace1.github.io/BrickGPT/) · [Code](https://github.com/AvaLovelace1/BrickGPT) · [Data](https://huggingface.co/datasets/AvaLovelace/StableText2Brick) |
| 2025 | **LEGO-Maker: A Semantic-Driven Algorithm for Text-to-3D Generation** — ICCV 2025 | Decomposes text-driven 3D models into functional components and adds motion to the resulting modular assets. | [Paper](https://openaccess.thecvf.com/content/ICCV2025/html/Zhang_LEGO-Maker_A_Semantic-Driven_Algorithm_for_Text-to-3D_Generation_ICCV_2025_paper.html) |

### From Images and Sketches

| Year | Paper | Focus | Links |
|---:|---|---|---|
| 2025 | **LegoACE: Autoregressive Construction Engine for Expressive LEGO Assemblies** (also supports text) — SIGGRAPH Asia 2025 | Generates connected LEGO models from text or multiview normal maps using compact brick tokens and autoregressive prediction. | [Paper](https://doi.org/10.1145/3757377.3763881) · [Project](https://xh38.github.io/LegoACE/) · [Code](https://github.com/VAST-AI-Research/LegoACE) · [Models](https://huggingface.co/VAST-AI/LegoACE) |
| 2025 | **LEGO-Maker: Autoregressive Image-Conditioned LEGO Model Creation** — SIGGRAPH Asia 2025 | Generates multi-type brick models from images with autoregressive tokens and rollback to avoid collisions. | [Paper](https://doi.org/10.1145/3763285) |
| 2024 | **Creating LEGO Figurines from Single Images** — SIGGRAPH 2024 | Turns portrait photos into buildable LEGO figurines with personalized, printable surface decals. | [Paper](https://doi.org/10.1145/3658167) |
| 2023 | **Computational Design of LEGO Sketch Art** — SIGGRAPH Asia 2023 | Converts images into LEGO sketch art by optimizing expressive contours and filling them with bricks. | [Paper](https://doi.org/10.1145/3618306) |
| 2022 | **Brick Yourself within 3 Minutes** — ICRA 2022 | Converts a captured portrait into a personalized brick model and assembly instructions through an automated kiosk. | [Paper](https://air.tsinghua.edu.cn/en/Brick-Yourself-within-3-Minutes.pdf) · [Project](https://www.unicus.cn/research/31-20.html) |
| 2021 | **Brick-by-Brick: Combinatorial Construction with Deep Reinforcement Learning** — NeurIPS 2021 | Learns to assemble unseen target shapes from images while filtering out invalid brick placements. | [Paper](https://proceedings.neurips.cc/paper/2021/hash/2d4027d6df9c0256b8d4474ce88f8c88-Abstract.html) · [Code](https://github.com/POSTECH-CVLab/Brick-by-Brick) |
| 2021 | **Image2Lego: Customized LEGO Set Generation from Images** | Reconstructs 3D shapes from photographs, converts them to bricks, and generates building instructions. | [Paper](https://arxiv.org/abs/2108.08477) · [Project](https://krlennon.github.io/Image2LEGO/) |
| 2019 | **Computational LEGO Technic Design** — SIGGRAPH Asia 2019 | Optimizes LEGO Technic structures from sketches while accounting for visual fidelity, connectivity, and structural integrity. | [Paper](https://arxiv.org/abs/2007.02245) · [Project](https://xuhaocuhk.github.io/projects/compute_technic/) |

### From Geometry and 3D Models

| Year | Paper | Focus | Links |
|---:|---|---|---|
| 2026 | **Fourfold Is Enough: Connected LEGO Models from One Brick Type** | Proves that fourfold scaling suffices to rebuild any finite face-connected voxel shape with connected 2-by-4 bricks. | [Paper](https://arxiv.org/abs/2609.09205) |
| 2026 | **BrickAnything: Geometry-Conditioned Buildable Brick Generation with Structure-Aware Tokenization** | Generates buildable brick sequences from 3D geometry using attachment-aware tokens and validity-constrained decoding. | [Paper](https://arxiv.org/abs/2605.26182) · [Code](https://github.com/xjtunzy/BrickAnything) |
| 2024 | **Streamlining LEGO Model Design: An Automated Optimisation Approach** | Converts 3D models into layered LEGO layouts while reducing brick count and improving interlayer connections. | [Paper](https://www.sciencedirect.com/science/article/pii/S2212827124009314) |
| 2020 | **Combinatorial 3D Shape Generation via Sequential Assembly** | Uses Bayesian optimization to assemble target 3D shapes from primitives under geometric and stability constraints. | [Paper](https://arxiv.org/abs/2004.07414) · [Code](https://github.com/POSTECH-CVLab/Combinatorial-3D-Shape-Generation) |
| 2019 | **Automatic Generation of Vivid LEGO Architectural Sculptures** — Computer Graphics Forum | Converts architectural models into brick sculptures that preserve repeating elements and other distinctive visual features. | [Paper](https://doi.org/10.1111/cgf.13603) |
| 2018 | **Split-and-Merge-Based Genetic Algorithm for LEGO Brick Sculpture Optimization** — IEEE Access | Uses split-and-merge genetic search to minimize brick count while preserving shape, connectivity, and stability. | [Paper](https://doi.org/10.1109/ACCESS.2018.2859039) |
| 2016 | **A Multi-Phase Search Approach to the LEGO Construction Problem** — SoCS | Combines layered and local search to find connected, structurally sound brick layouts for target volumes. | [Paper](https://doi.org/10.1609/socs.v7i1.18385) |
| 2015 | **Legolization: Optimizing LEGO Designs** — SIGGRAPH Asia 2015 | Refines brick layouts from 3D models using force-based stability analysis, color fidelity, and brick count. | [Paper](https://www.cs.columbia.edu/~yonghao/siga15/abstsiga15.html) |
| 2015 | **Finding an Optimal LEGO Brick Layout of a Voxelized 3D Object** | Uses genetic search to maximize connectivity and reduce brick count in voxel-derived LEGO layouts. | [Paper](https://doi.org/10.1145/2739480.2754667) |
| 2013 | **LEGO Builder: Automatic Generation of LEGO Assembly Manuals from 3D Polygon Models** | Converts polygon models into connected LEGO designs and step-by-step instructions using a brick-connection graph. | [Paper](https://doi.org/10.3169/mta.1.354) |
| 2013 | **Automatic Generation of Constructable Brick Sculptures** — Eurographics | Voxelizes 3D meshes, merges bricks, repairs structural weaknesses, and produces building instructions. | [Paper](https://infoscience.epfl.ch/entities/publication/719977db-2ebd-44ee-8f58-1b22c7f0bdce) |

### Other Inputs and Unconditional Generation

| Year | Paper | Focus | Links |
|---:|---|---|---|
| 2024 | **Learn to Create Simple LEGO Micro Buildings** — SIGGRAPH Asia 2024 | Learns to generate diverse micro-building volumes and reconstructs them as connected, buildable brick models. | [Paper](https://doi.org/10.1145/3687755) · [Code](https://github.com/Occulte/LEGO_Buildings_Generation) |
| 2020 | **Building LEGO Using Deep Generative Models of Graphs** — NeurIPS ML4Eng Workshop | Learns graph-based assembly patterns from human-built LEGO models to generate new brick structures. | [Paper](https://arxiv.org/abs/2012.11543) · [Code](https://github.com/uoguelph-mlrg/GenerativeLEGO) |
| 2003 | **Using Assembly Representations to Enable Evolutionary Design of LEGO Structures** — AIEDAM | Evolves electromechanical LEGO assemblies represented as graphs using genetic operators and structural evaluations. | [Paper](https://doi.org/10.1017/S0890060403172046) |

[Back to contents](#contents)

<a id="physics-modeling-simulation"></a>
<a id="physics-simulation"></a>

## 2. Physics Modeling and Simulation

Model connectivity, stability, contact forces, and assembly dynamics.

| Year | Paper | Focus | Links |
|---:|---|---|---|
| 2026 | ★ **BrickSim: A Physics-Based Simulator for Manipulating Interlocking Brick Assemblies** | Simulates assembly, disassembly, and collapse in real time with a force-based model of snap-fit connections. | [Paper](https://arxiv.org/abs/2603.16853) · [Project](https://intelligent-control-lab.github.io/BrickSim/) · [Code](https://github.com/intelligent-control-lab/BrickSim) |
| 2024 | **StableLego: Stability Analysis of Block Stacking Assembly** — IEEE RA-L | Estimates assembly stability and weak regions by optimizing contact-force balance, with a large LEGO layout dataset. | [Paper](https://arxiv.org/abs/2402.10711) · [Code and Data](https://github.com/intelligent-control-lab/StableLego) |
| 2023 | **BrickFEM: An Automated Finite Element Model for Static and Dynamic Simulations of Simple LEGO Sets** | Automates finite-element model generation and analysis for the static and dynamic behavior of simple LEGO assemblies. | [Paper](https://engrxiv.org/preprint/view/2898) |

[Back to contents](#contents)

<a id="reasoning-planning"></a>

## 3. Reasoning and Planning

Understand instructions and assembly states; plan sequences and correct errors.

### Spatial and Physical Reasoning

| Year | Paper | Focus | Links |
|---:|---|---|---|
| 2026 | **Brick-Composer: Using MLLMs for Assembly with Diverse Bricks** | Introduces a diverse-brick assembly benchmark and trains multimodal models for brick selection and placement. | [Paper](https://arxiv.org/abs/2606.05445) |
| 2026 | **Sample-Efficient Post-Training for LEGO Spatial-Physics Reasoning** | Combines targeted data selection with geometry- and physics-based rewards to improve LEGO synthesis reasoning. | [Paper](https://arxiv.org/abs/2606.07602) |
| 2026 | **WorkBenchMark: A LEGO-Based Assembly Benchmark with an Assembly-by-Disassembly Baseline for the Smart Manufacturing League** — RoboCup 2026 | Introduces 400 Duplo assembly tasks and an open-vocabulary planning baseline based on disassembly. | [Paper](https://arxiv.org/abs/2606.19358) |
| 2026 | **LEGO Co-builder: Exploring Fine-Grained Vision-Language Modeling for Multimodal LEGO Assembly Assistants** — ICMI 2026 (accepted) | Benchmarks vision-language models on stepwise LEGO instruction following, object detection, and assembly-state recognition. | [Paper](https://arxiv.org/abs/2507.05515) |
| 2025 | **LEGO-Puzzles: How Good Are MLLMs at Multi-Step Spatial Reasoning?** | Tests multimodal models on elementary LEGO spatial questions and increasingly long assembly plans. | [Paper](https://arxiv.org/abs/2503.19990) |

### Assembly Planning

| Year | Paper | Focus | Links |
|---:|---|---|---|
| 2025 | **AssemblyComplete: 3D Combinatorial Construction with Deep Reinforcement Learning** — ACC 2025 | Uses reinforcement learning and an action mask to infer and complete stable, partially built LEGO structures. | [Paper](https://arxiv.org/abs/2410.15469) |
| 2024 | **Physics-Aware Combinatorial Assembly Sequence Planning Using Data-Free Action Masking** | Learns brick placement sequences while filtering actions that violate physical assembly constraints. | [Paper](https://arxiv.org/abs/2408.10162) · [Code](https://github.com/intelligent-control-lab/PhysicsAwareCombinatorialASP) |
| 2024 | **TreeSBA: Tree-Transformer for Self-Supervised Sequential Brick Assembly** — ECCV 2024 | Predicts brick assembly actions from multiview images using a LEGO tree and self-supervised real-image training. | [Paper](https://arxiv.org/abs/2407.15648) · [Project](https://dreamguo.github.io/projects/TreeSBA/) · [Code](https://github.com/dreamguo/TreeSBA) |
| 2022 | **Planning Assembly Sequence with Graph Transformer** | Represents LEGO models as heterogeneous graphs and learns feasible assembly orders with a graph transformer. | [Paper](https://arxiv.org/abs/2210.05236) |
| 2022 | **Blocks Assemble! Learning to Assemble with Large-Scale Structured Reinforcement Learning** — ICML 2022 | Trains graph-based reinforcement learning policies to assemble magnetic blocks into unseen target blueprints. | [Paper](https://proceedings.mlr.press/v162/ghasemipour22a.html) |

### Assembly Instructions

| Year | Paper | Focus | Links |
|---:|---|---|---|
| 2024 | **Learning to Build by Building Your Own Instructions** | Lets an agent create visual instructions while disassembling a model, then use them to rebuild it. | [Paper](https://arxiv.org/abs/2410.01111) |
| 2022 | ★ **Translating a Visual LEGO Manual to a Machine-Executable Plan** — ECCV 2022 | Reconstructs executable 3D assembly steps from manual images using keypoint detection and 2D-to-3D projection. | [Paper](https://arxiv.org/abs/2207.12572) · [Project](https://cs.stanford.edu/~rcwang/projects/lego_manual/) · [Code](https://github.com/Relento/lego_release) |

### Perception and Error Correction

| Year | Paper | Focus | Links |
|---:|---|---|---|
| 2024 | **SCANet: Correcting LEGO Assembly Errors with Self-Correct Assembly Network** — IROS 2024 | Detects misplaced bricks against manual images and predicts corrections for single-step assembly errors. | [Paper](https://arxiv.org/abs/2403.18195) · [Project](https://scanet-iros2024.github.io/) |
| 2023 | **MobileBrick: Building LEGO for 3D Reconstruction on Mobile Devices** — CVPR 2023 | Provides mobile RGB-D captures of LEGO sets with accurate 3D geometry for reconstruction benchmarks. | [Paper](https://arxiv.org/abs/2303.01932) · [Project](https://code.active.vision/MobileBrick/) · [Code](https://github.com/ActiveVisionLab/MobileBrick) |
| 2022 | **Break and Make: Interactive Structural Understanding Using LEGO Bricks** — ECCV 2022 | Introduces an interactive simulator where agents learn a LEGO model by disassembling and rebuilding it. | [Paper](https://arxiv.org/abs/2207.13738) · [Simulator](https://github.com/aaronwalsman/ltron) · [Training Code](https://github.com/aaronwalsman/ltron-torch-eccv22) |

[Back to contents](#contents)

<a id="robotic-manipulation"></a>
<a id="robotic-construction"></a>

## 4. Robotic Manipulation

Study robotic perception, manipulation, and execution for brick assembly and disassembly.

### Long-Horizon and Multi-Robot Assembly

| Year | Paper | Focus | Links |
|---:|---|---|---|
| 2026 | **BrickCraft: Visuomotor Skill Composition with Situated Manual Guidance for Long-Horizon Interlocking Brick Assembly** | Combines reusable visuomotor skills with spatially grounded manuals to assemble unseen brick structures over long horizons. | [Paper](https://arxiv.org/abs/2605.07605) · [Project](https://intelligent-control-lab.github.io/BrickCraft/) |
| 2025 | ★ **APEX-MR: Multi-Robot Asynchronous Planning and Execution for Cooperative Assembly** — RSS 2025 | Coordinates multiple robots asynchronously to execute long LEGO assembly plans safely and efficiently. | [Paper](https://arxiv.org/abs/2503.15836) · [Code](https://github.com/intelligent-control-lab/APEX-MR) |

### Precision Manipulation

| Year | Paper | Focus | Links |
|---:|---|---|---|
| 2025 | **Eye-in-Finger: Smart Fingers for Delicate Assembly and Disassembly of LEGO** — IROS 2025 | Embeds high-resolution sensing in robot fingertips to correct alignment during precise LEGO assembly and disassembly. | [Paper](https://arxiv.org/abs/2503.06848) |
| 2024 | **A Lightweight and Transferable Design for Robust LEGO Manipulation** — ISFA 2024 | Combines a purpose-built end effector with learned motion optimization for reliable LEGO manipulation across robots. | [Paper](https://arxiv.org/abs/2309.02354) |

### Learning from Demonstration

| Year | Paper | Focus | Links |
|---:|---|---|---|
| 2023 | **Simulation-Aided Learning from Demonstration for Robotic LEGO Construction** | Extracts construction plans from human demonstrations and checks them in simulation before robotic execution. | [Paper](https://arxiv.org/abs/2309.11010) |
| 2023 | **Robotic LEGO Assembly and Disassembly from Human Demonstration** | Enables an industrial robot to learn LEGO assembly and disassembly tasks by observing human demonstrations. | [Paper](https://arxiv.org/abs/2305.15667) · [Code](https://github.com/intelligent-control-lab/Robotic_LEGO_Assembly_and_Disassembly_from_Human_Demonstration) |

[Back to contents](#contents)

<a id="robot-creativity"></a>

## 5. Robot Creativity

Connect generative design with physical making, including work beyond bricks.

### From Prompt to Product

| Year | Paper | Focus | Links |
|---:|---|---|---|
| 2026 | ★ **Prompt-to-Product: Generative Assembly via Bimanual Manipulation** — IEEE Robotics & Automation Magazine | Turns text prompts into buildable brick designs and physically assembles them with a two-arm robot. | [Paper](https://arxiv.org/abs/2508.21063) · [Project](https://prompt2product.github.io/) |

### Robot Design

| Year | Paper | Focus | Links |
|---:|---|---|---|
| 2024 | **Text2Robot: Evolutionary Robot Design from Text Descriptions** | Generates manufacturable walking robot bodies from text through evolutionary search and body-control optimization. | [Paper](https://arxiv.org/abs/2406.19963) · [Project](https://generalroboticslab.com/Text2Robot/) |
| 2023 | **DiffuseBot: Breeding Soft Robots with Physics-Augmented Generative Diffusion Models** — NeurIPS 2023 | Generates soft-robot bodies with a physics-guided diffusion model and jointly optimizes morphology and control. | [Paper](https://arxiv.org/abs/2311.17053) · [Project](https://diffusebot.github.io/) |
| 2020 | **RoboGrammar: Graph Grammar for Terrain-Optimized Robot Design** — SIGGRAPH Asia 2020 | Searches a grammar of fabricable robot bodies and controllers to find designs suited to specific terrains. | [Project](https://people.csail.mit.edu/jiex/papers/robogrammar/) |

### Crafting and Sculpting

| Year | Paper | Focus | Links |
|---:|---|---|---|
| 2024 | **LLM-Craft: Robotic Crafting of Elasto-Plastic Objects with Large Language Models** | Uses language-model planning with shape-aware state and action representations to craft deformable objects. | [Paper](https://arxiv.org/abs/2406.08648) · [Project](https://sites.google.com/andrew.cmu.edu/llmcraft) |
| 2024 | **SculptDiff: Learning Robotic Clay Sculpting from Humans with Goal-Conditioned Diffusion Policy** | Learns goal-conditioned clay sculpting policies from demonstrations using point-cloud observations and diffusion. | [Paper](https://arxiv.org/abs/2403.10401) · [Project](https://sites.google.com/andrew.cmu.edu/imitation-sculpting/home) |
| 2024 | **RoPotter: Toward Robotic Pottery and Deformable Object Manipulation with Structural Priors** | Uses clay cross-section priors and state recovery to learn long-horizon pottery-wheel shaping. | [Paper](https://arxiv.org/abs/2408.02184) |
| 2024 | **SculptBot: Pre-Trained Models for 3D Deformable Object Manipulation** — ICRA 2024 | Learns clay deformation dynamics from point clouds and plans grasps to sculpt target shapes. | [Paper](https://arxiv.org/abs/2309.08728) · [Project](https://sites.google.com/andrew.cmu.edu/sculptbot) |
| 2023 | **RoboCook: Long-Horizon Elasto-Plastic Object Manipulation with Diverse Tools** — CoRL 2023 | Learns tool-object dynamics and policies for multi-step shaping of deformable materials with varied tools. | [Paper](https://arxiv.org/abs/2306.14447) |
| 2023 | **DALL-E-Bot: Introducing Web-Scale Diffusion Models to Robotics** — IEEE RA-L 2023 | Uses a diffusion-generated goal image to rearrange real objects into a plausible scene without task-specific training. | [Paper](https://arxiv.org/abs/2210.02438) |
| 2022 | **RoboCraft: Learning to See, Simulate, and Shape Elasto-Plastic Objects with Graph Networks** — RSS 2022 | Learns particle-based deformable-object dynamics from RGB-D observations and plans actions to reach target shapes. | [Paper](https://arxiv.org/abs/2205.02909) |

[Back to contents](#contents)

<a id="datasets-benchmarks"></a>

## Datasets and Benchmarks

### Design and Structure

| Dataset / Benchmark | Contents | Links |
|---|---|---|
| **BrickNet Dataset** | 100,000+ human-designed LDraw objects and scenes. | [Project](https://kulits.github.io/BrickNet/) |
| **LegoVerse** | 55,000+ models spanning 9,314 brick types. | [Project](https://xh38.github.io/LegoACE/) |
| **StableText2Brick** | 47,000+ stable brick structures with text descriptions. | [Data](https://huggingface.co/datasets/AvaLovelace/StableText2Brick) |
| **StableLego** | 50,000+ objects with brick layouts and stability estimates. | [Data](https://github.com/intelligent-control-lab/StableLego) |
| **LEGO Micro-Buildings** | Micro-building models for learned generation. | [Repository](https://github.com/Occulte/LEGO_Buildings_Generation) |
| **Combinatorial 3D Shape Generation Dataset** | Primitive-based objects for sequential construction. | [Repository](https://github.com/POSTECH-CVLab/Combinatorial-3D-Shape-Generation) |
| **LDraw Official Model Repository** | Community-maintained LDraw models of official sets. | [Repository](https://omr.ldraw.org/) |

### Reasoning and Planning

| Dataset / Benchmark | Contents | Links |
|---|---|---|
| **BC-Bench** | Diverse-brick selection and placement-pose estimation. | [Paper](https://arxiv.org/abs/2606.05445) |
| **WorkBenchMark** | 400 Duplo assembly tasks across four complexity levels. | [Paper](https://arxiv.org/abs/2606.19358) |
| **LEGO Co-builder** | Visual states and instructions for multimodal assembly assistants. | [Paper](https://arxiv.org/abs/2507.05515) |
| **LEGO-Puzzles** | 1,100 elementary visual questions plus multi-step assembly planning. | [Paper](https://arxiv.org/abs/2503.19990) |
| **LTRON Procedural Vehicles** | Procedural vehicles for learning visual assembly instructions. | [Paper](https://arxiv.org/abs/2410.01111) |
| **LEGO-ECA** | Partial builds, assembly errors, and corrective labels. | [Project](https://scanet-iros2024.github.io/) |
| **LTRON / Break and Make** | Simulated disassembly and reconstruction of brick models. | [Simulator](https://github.com/aaronwalsman/ltron) |
| **MEPNet LEGO Manuals** | Three visual-manual datasets for assembly planning. | [Repository](https://github.com/Relento/lego_release) |

### Perception

| Dataset / Benchmark | Contents | Links |
|---|---|---|
| **MobileBrick** | Mobile RGB-D captures of 153 brick sets with 3D annotations. | [Project](https://code.active.vision/MobileBrick/) · [Code](https://github.com/ActiveVisionLab/MobileBrick) |
| **Photos and Rendered Images of LEGO Bricks** | Real photographs and synthetic renders of individual bricks. | [Dataset Paper](https://doi.org/10.1038/s41597-023-02682-2) |
| **B200C LEGO Classification Dataset** | Approximately 800,000 synthetic images across 200 brick classes. | [Data](https://www.kaggle.com/datasets/ronanpickell/b200c-lego-classification-dataset) · [Generator](https://github.com/korra-pickell/LEGO-Classification-Dataset) |
| **B200 LEGO Detection Dataset** | Synthetic object detection across 200 brick classes. | [Data](https://www.kaggle.com/datasets/ronanpickell/b100-lego-detection-dataset) |

### Challenges

**[RoCo — IROS 2026](https://rocochallenge.github.io/RoCo-IROS2026/):** Robotic collaborative assembly challenge with brick-assembly and industrial board-assembly tracks.

[Back to contents](#contents)

<a id="tools-demos"></a>
<a id="software-tools"></a>

## Tools and Demos

Research code and project pages are linked beside the relevant papers.

### Company Demos and Posts

| Company | Demonstration | What it shows | Links |
|---|---|---|---|
| Generalist AI | One-shot LEGO assembly | A robot copies a three-brick structure after observing a human-built example. | [Blog](https://generalistai.com/blog/the-robots-build-now-too) · [Video](https://www.youtube.com/watch?v=eF9PqpPB0MM) |
| Generalist AI | LEGO disassembly and sorting | A robot separates assembled bricks and sorts them into color-matched bins. | [Blog](https://generalistai.com/blog/research-preview) · [Video](https://www.youtube.com/watch?v=3YV5dzvTvco) |
| Dexmal | Great Wall brick assembly | Multiple robots collaborate on a Great Wall model built from small interlocking bricks. | [Event page](https://www.worldrobotconference.com/expo/event/244.html) · [Video post](https://x.com/Dexmal_AI/status/2095403201378033719) |
| 1X | NEO hand dexterity | NEO assembles a small LEGO structure in a demonstration of its dexterous hands. | [Blog](https://www.1x.tech/discover/neos-hands) · [Video](https://www.youtube.com/watch?v=QRyXV3csReA) |
| Universal Robots | Collaborative LEGO rocket | A robot and a person jointly assemble a LEGO rocket. | [Video](https://video.universal-robots.com/a-robot-learns-to-jointly-assemble-a-lego-rocket) |

### Brick Design Tools

For brick model creation and exchange:

| Tool | Purpose |
|---|---|
| [LDraw](https://www.ldraw.org/) | Open brick-model format and parts library |
| [LeoCAD](https://www.leocad.org/) | Open-source editor for LDraw models |
| [BrickLink Studio](https://www.bricklink.com/v3/studio/download.page) | Brick design, rendering, instructions, and inventories |
| [BrickHub](https://brickhub.org/) | Share and browse digital brick models |

<a id="license"></a>

**License:** [MIT](LICENSE). Linked works retain their own licenses; please cite the original research.
