# Awesome Brick Assembly <img src="assets/brick-assembly.svg" alt="LEGO-style brick assembly" width="40" height="40" align="middle"> & Robot Creativity 🤖

Research, datasets, and tools for turning ideas into physical objects through brick design, simulation, planning, and robotic assembly.

<a id="contents"></a>

## Contents

- [Surveys](#surveys)
- [1. Generative Design](#generative-design)
- [2. Physics and Simulation](#physics-simulation)
- [3. Reasoning and Planning](#reasoning-planning)
- [4. Robotic Assembly](#robotic-construction)
- [5. Robot Creativity](#robot-creativity)
- [Datasets and Benchmarks](#datasets-benchmarks)
- [Software and CAD](#software-tools)
- [Contributing](#contributing)

**Start here:** Read the surveys, then follow the **★** paper in each research area.

<a id="surveys"></a>

## Surveys

| Year | Paper | Links |
|---:|---|---|
| 2018 | **State of the Art on Stylized Fabrication** | [Paper](https://doi.org/10.1111/cgf.13327) |
| 2014 | **Survey on Automated LEGO Assembly Construction** | [Paper](https://dspace.zcu.cz/bitstream/11025/11949/1/Kim.pdf) |

[Back to contents](#contents)

<a id="generative-design"></a>

## 1. Generative Design

Generate brick structures from text, images, geometry, or examples.

### Learned Generation

| Year | Paper | Links |
|---:|---|---|
| 2026 | **BrickAnything: Geometry-Conditioned Buildable Brick Generation with Structure-Aware Tokenization** | [Paper](https://arxiv.org/abs/2605.26182) · [Code](https://github.com/xjtunzy/BrickAnything) |
| 2026 | **BrickNet: Graph-Backed Generative Brick Assembly** — CVPR 2026 | [Paper](https://arxiv.org/abs/2604.22984) · [Project](https://kulits.github.io/BrickNet/) |
| 2025 | ★ **Generating Physically Stable and Buildable Brick Structures from Text (BrickGPT / LegoGPT)** — ICCV 2025, [Best Paper (Marr Prize)](https://www.thecvf.com/?page_id=413) | [Paper](https://arxiv.org/abs/2505.05469) · [Project](https://avalovelace1.github.io/BrickGPT/) · [Code](https://github.com/AvaLovelace1/BrickGPT) · [Data](https://huggingface.co/datasets/AvaLovelace/StableText2Brick) |
| 2025 | **LegoACE: Autoregressive Construction Engine for Expressive LEGO Assemblies** — SIGGRAPH Asia 2025 | [Paper](https://doi.org/10.1145/3757377.3763881) · [Project](https://xh38.github.io/LegoACE/) · [Code](https://github.com/VAST-AI-Research/LegoACE) · [Models](https://huggingface.co/VAST-AI/LegoACE) |
| 2025 | **LEGO-Maker: A Semantic-Driven Algorithm for Text-to-3D Generation** — ICCV 2025 | [Paper](https://openaccess.thecvf.com/content/ICCV2025/html/Zhang_LEGO-Maker_A_Semantic-Driven_Algorithm_for_Text-to-3D_Generation_ICCV_2025_paper.html) |
| 2025 | **LEGO-Maker: Autoregressive Image-Conditioned LEGO Model Creation** — SIGGRAPH Asia 2025 | [Paper](https://doi.org/10.1145/3763285) |
| 2024 | **Learn to Create Simple LEGO Micro Buildings** — SIGGRAPH Asia 2024 | [Paper](https://doi.org/10.1145/3687755) · [Code](https://github.com/Occulte/LEGO_Buildings_Generation) |
| 2021 | **Brick-by-Brick: Combinatorial Construction with Deep Reinforcement Learning** — NeurIPS 2021 | [Paper](https://proceedings.neurips.cc/paper/2021/hash/2d4027d6df9c0256b8d4474ce88f8c88-Abstract.html) · [Code](https://github.com/POSTECH-CVLab/Brick-by-Brick) |
| 2021 | **Image2Lego: Customized LEGO Set Generation from Images** | [Paper](https://arxiv.org/abs/2108.08477) · [Project](https://krlennon.github.io/Image2LEGO/) |
| 2020 | **Building LEGO Using Deep Generative Models of Graphs** — NeurIPS ML4Eng Workshop | [Paper](https://arxiv.org/abs/2012.11543) · [Code](https://github.com/uoguelph-mlrg/GenerativeLEGO) |

### Images, Portraits, and Sketches

| Year | Paper | Links |
|---:|---|---|
| 2024 | **Creating LEGO Figurines from Single Images** — SIGGRAPH 2024 | [Paper](https://doi.org/10.1145/3658167) |
| 2023 | **Computational Design of LEGO Sketch Art** — SIGGRAPH Asia 2023 | [Paper](https://doi.org/10.1145/3618306) |
| 2022 | **Brick Yourself within 3 Minutes** — ICRA 2022 | [Paper](https://air.tsinghua.edu.cn/en/Brick-Yourself-within-3-Minutes.pdf) · [Project](https://www.unicus.cn/research/31-20.html) |
| 2019 | **Computational LEGO Technic Design** — SIGGRAPH Asia 2019 | [Paper](https://arxiv.org/abs/2007.02245) · [Project](https://xuhaocuhk.github.io/projects/compute_technic/) |
| 2019 | **Automatic Generation of Vivid LEGO Architectural Sculptures** — Computer Graphics Forum | [Paper](https://doi.org/10.1111/cgf.13603) |

### Optimization and Geometric Foundations

| Year | Paper | Links |
|---:|---|---|
| 2026 | **Fourfold Is Enough: Connected LEGO Models from One Brick Type** | [Paper](https://arxiv.org/abs/2609.09205) |
| 2024 | **Streamlining LEGO Model Design: An Automated Optimisation Approach** | [Paper](https://www.sciencedirect.com/science/article/pii/S2212827124009314) |
| 2020 | **Combinatorial 3D Shape Generation via Sequential Assembly** | [Paper](https://arxiv.org/abs/2004.07414) · [Code](https://github.com/POSTECH-CVLab/Combinatorial-3D-Shape-Generation) |
| 2018 | **Split-and-Merge-Based Genetic Algorithm for LEGO Brick Sculpture Optimization** — IEEE Access | [Paper](https://doi.org/10.1109/ACCESS.2018.2859039) |
| 2016 | **A Multi-Phase Search Approach to the LEGO Construction Problem** — SoCS | [Paper](https://doi.org/10.1609/socs.v7i1.18385) |
| 2015 | **Legolization: Optimizing LEGO Designs** — SIGGRAPH Asia 2015 | [Paper](https://www.cs.columbia.edu/~yonghao/siga15/abstsiga15.html) |
| 2015 | **Finding an Optimal LEGO Brick Layout of a Voxelized 3D Object** | [Paper](https://doi.org/10.1145/2739480.2754667) |
| 2013 | **LEGO Builder: Automatic Generation of LEGO Assembly Manuals from 3D Polygon Models** | [Paper](https://doi.org/10.3169/mta.1.354) |
| 2013 | **Automatic Generation of Constructable Brick Sculptures** — Eurographics | [Paper](https://infoscience.epfl.ch/entities/publication/719977db-2ebd-44ee-8f58-1b22c7f0bdce) |
| 2003 | **Using Assembly Representations to Enable Evolutionary Design of LEGO Structures** — AIEDAM | [Paper](https://doi.org/10.1017/S0890060403172046) |

[Back to contents](#contents)

<a id="physics-simulation"></a>

## 2. Physics and Simulation

Model connectivity, stability, contact forces, and assembly dynamics.

| Year | Paper | Links |
|---:|---|---|
| 2026 | ★ **BrickSim: A Physics-Based Simulator for Manipulating Interlocking Brick Assemblies** | [Paper](https://arxiv.org/abs/2603.16853) · [Project](https://intelligent-control-lab.github.io/BrickSim/) · [Code](https://github.com/intelligent-control-lab/BrickSim) |
| 2024 | **StableLego: Stability Analysis of Block Stacking Assembly** — IEEE RA-L | [Paper](https://arxiv.org/abs/2402.10711) · [Code and Data](https://github.com/intelligent-control-lab/StableLego) |
| 2023 | **BrickFEM: An Automated Finite Element Model for Static and Dynamic Simulations of Simple LEGO Sets** | [Paper](https://engrxiv.org/preprint/view/2898) |

[Back to contents](#contents)

<a id="reasoning-planning"></a>

## 3. Reasoning and Planning

Understand instructions and assembly states; plan sequences and correct errors.

### Spatial and Physical Reasoning

| Year | Paper | Links |
|---:|---|---|
| 2026 | **Brick-Composer: Using MLLMs for Assembly with Diverse Bricks** | [Paper](https://arxiv.org/abs/2606.05445) |
| 2026 | **Sample-Efficient Post-Training for LEGO Spatial-Physics Reasoning** | [Paper](https://arxiv.org/abs/2606.07602) |
| 2026 | **WorkBenchMark: A LEGO-Based Assembly Benchmark with an Assembly-by-Disassembly Baseline for the Smart Manufacturing League** — RoboCup 2026 | [Paper](https://arxiv.org/abs/2606.19358) |
| 2026 | **LEGO Co-builder: Exploring Fine-Grained Vision-Language Modeling for Multimodal LEGO Assembly Assistants** — ICMI 2026 (accepted) | [Paper](https://arxiv.org/abs/2507.05515) |
| 2025 | **LEGO-Puzzles: How Good Are MLLMs at Multi-Step Spatial Reasoning?** | [Paper](https://arxiv.org/abs/2503.19990) |

### Assembly Planning

| Year | Paper | Links |
|---:|---|---|
| 2025 | **AssemblyComplete: 3D Combinatorial Construction with Deep Reinforcement Learning** — ACC 2025 | [Paper](https://arxiv.org/abs/2410.15469) |
| 2024 | **Physics-Aware Combinatorial Assembly Sequence Planning Using Data-Free Action Masking** | [Paper](https://arxiv.org/abs/2408.10162) · [Code](https://github.com/intelligent-control-lab/PhysicsAwareCombinatorialASP) |
| 2024 | **TreeSBA: Tree-Transformer for Self-Supervised Sequential Brick Assembly** — ECCV 2024 | [Paper](https://arxiv.org/abs/2407.15648) · [Project](https://dreamguo.github.io/projects/TreeSBA/) · [Code](https://github.com/dreamguo/TreeSBA) |
| 2022 | **Planning Assembly Sequence with Graph Transformer** | [Paper](https://arxiv.org/abs/2210.05236) |
| 2022 | **Blocks Assemble! Learning to Assemble with Large-Scale Structured Reinforcement Learning** — ICML 2022 | [Paper](https://proceedings.mlr.press/v162/ghasemipour22a.html) |

### Assembly Instructions

| Year | Paper | Links |
|---:|---|---|
| 2024 | **Learning to Build by Building Your Own Instructions** | [Paper](https://arxiv.org/abs/2410.01111) |
| 2022 | ★ **Translating a Visual LEGO Manual to a Machine-Executable Plan** — ECCV 2022 | [Paper](https://arxiv.org/abs/2207.12572) · [Project](https://cs.stanford.edu/~rcwang/projects/lego_manual/) · [Code](https://github.com/Relento/lego_release) |

### Perception and Error Correction

| Year | Paper | Links |
|---:|---|---|
| 2024 | **SCANet: Correcting LEGO Assembly Errors with Self-Correct Assembly Network** — IROS 2024 | [Paper](https://arxiv.org/abs/2403.18195) · [Project](https://scanet-iros2024.github.io/) |
| 2023 | **MobileBrick: Building LEGO for 3D Reconstruction on Mobile Devices** — CVPR 2023 | [Paper](https://arxiv.org/abs/2303.01932) · [Project](https://code.active.vision/MobileBrick/) · [Code](https://github.com/ActiveVisionLab/MobileBrick) |
| 2022 | **Break and Make: Interactive Structural Understanding Using LEGO Bricks** — ECCV 2022 | [Paper](https://arxiv.org/abs/2207.13738) · [Simulator](https://github.com/aaronwalsman/ltron) · [Training Code](https://github.com/aaronwalsman/ltron-torch-eccv22) |

[Back to contents](#contents)

<a id="robotic-construction"></a>

## 4. Robotic Assembly

Execute assembly and disassembly with physical robots.

### Long-Horizon and Multi-Robot Assembly

| Year | Paper | Links |
|---:|---|---|
| 2026 | **BrickCraft: Visuomotor Skill Composition with Situated Manual Guidance for Long-Horizon Interlocking Brick Assembly** | [Paper](https://arxiv.org/abs/2605.07605) · [Project](https://intelligent-control-lab.github.io/BrickCraft/) |
| 2025 | ★ **APEX-MR: Multi-Robot Asynchronous Planning and Execution for Cooperative Assembly** — RSS 2025 | [Paper](https://arxiv.org/abs/2503.15836) · [Code](https://github.com/intelligent-control-lab/APEX-MR) |

### Precision Manipulation

| Year | Paper | Links |
|---:|---|---|
| 2025 | **Eye-in-Finger: Smart Fingers for Delicate Assembly and Disassembly of LEGO** — IROS 2025 | [Paper](https://arxiv.org/abs/2503.06848) |
| 2024 | **A Lightweight and Transferable Design for Robust LEGO Manipulation** — ISFA 2024 | [Paper](https://arxiv.org/abs/2309.02354) |

### Learning from Demonstration

| Year | Paper | Links |
|---:|---|---|
| 2023 | **Simulation-Aided Learning from Demonstration for Robotic LEGO Construction** | [Paper](https://arxiv.org/abs/2309.11010) |
| 2023 | **Robotic LEGO Assembly and Disassembly from Human Demonstration** | [Paper](https://arxiv.org/abs/2305.15667) · [Code](https://github.com/intelligent-control-lab/Robotic_LEGO_Assembly_and_Disassembly_from_Human_Demonstration) |

[Back to contents](#contents)

<a id="robot-creativity"></a>

## 5. Robot Creativity

Connect generative design with physical making, including work beyond bricks.

### From Prompt to Product

| Year | Paper | Links |
|---:|---|---|
| 2026 | ★ **Prompt-to-Product: Generative Assembly via Bimanual Manipulation** — IEEE Robotics & Automation Magazine | [Paper](https://arxiv.org/abs/2508.21063) · [Project](https://prompt2product.github.io/) |

### Robot Design

| Year | Paper | Links |
|---:|---|---|
| 2024 | **Text2Robot: Evolutionary Robot Design from Text Descriptions** | [Paper](https://arxiv.org/abs/2406.19963) · [Project](https://generalroboticslab.com/Text2Robot/) |
| 2023 | **DiffuseBot: Breeding Soft Robots with Physics-Augmented Generative Diffusion Models** — NeurIPS 2023 | [Paper](https://arxiv.org/abs/2311.17053) · [Project](https://diffusebot.github.io/) |
| 2020 | **RoboGrammar: Graph Grammar for Terrain-Optimized Robot Design** — SIGGRAPH Asia 2020 | [Project](https://people.csail.mit.edu/jiex/papers/robogrammar/) |

### Crafting and Sculpting

| Year | Paper | Links |
|---:|---|---|
| 2024 | **LLM-Craft: Robotic Crafting of Elasto-Plastic Objects with Large Language Models** | [Paper](https://arxiv.org/abs/2406.08648) · [Project](https://sites.google.com/andrew.cmu.edu/llmcraft) |
| 2024 | **SculptDiff: Learning Robotic Clay Sculpting from Humans with Goal-Conditioned Diffusion Policy** | [Paper](https://arxiv.org/abs/2403.10401) · [Project](https://sites.google.com/andrew.cmu.edu/imitation-sculpting/home) |
| 2024 | **RoPotter: Toward Robotic Pottery and Deformable Object Manipulation with Structural Priors** | [Paper](https://arxiv.org/abs/2408.02184) |
| 2024 | **SculptBot: Pre-Trained Models for 3D Deformable Object Manipulation** — ICRA 2024 | [Paper](https://arxiv.org/abs/2309.08728) · [Project](https://sites.google.com/andrew.cmu.edu/sculptbot) |
| 2023 | **RoboCook: Long-Horizon Elasto-Plastic Object Manipulation with Diverse Tools** — CoRL 2023 | [Paper](https://arxiv.org/abs/2306.14447) |
| 2023 | **DALL-E-Bot: Introducing Web-Scale Diffusion Models to Robotics** — IEEE RA-L 2023 | [Paper](https://arxiv.org/abs/2210.02438) |
| 2022 | **RoboCraft: Learning to See, Simulate, and Shape Elasto-Plastic Objects with Graph Networks** — RSS 2022 | [Paper](https://arxiv.org/abs/2205.02909) |

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

<a id="software-tools"></a>

## Software and CAD

Research code is linked beside each paper. For model creation and exchange:

| Tool | Purpose |
|---|---|
| [LDraw](https://www.ldraw.org/) | Open brick-model format and parts library |
| [LeoCAD](https://www.leocad.org/) | Open-source editor for LDraw models |
| [BrickLink Studio](https://www.bricklink.com/v3/studio/download.page) | Brick design, rendering, instructions, and inventories |
| [BrickHub](https://brickhub.org/) | Share and browse digital brick models |

<a id="contributing"></a>

## Contributing

Suggest additions or corrections through an issue or pull request. Include the title, year, venue, and official links; place new entries in the relevant section, newest first.

*Paper years follow the listed venue or the linked paper’s first publication/preprint. Resource availability and usage terms are documented at the linked sources.*

<a id="license"></a>

**License:** [MIT](LICENSE). Linked works retain their own licenses; please cite the original research.
