---
layout: homepage
---

## About Me

Welcome! I am currently a Ph.D. student in Computer Science at the Academy of Interdisciplinary Studies (AIS), Hong Kong University of Science and Technology (HKUST). Prior to my doctoral study, I received my M.Sc. degree from the Department of Computer Science and Technology, Tsinghua University, supervised by [Prof. Huaping Liu](https://sites.google.com/site/thuliuhuaping/home), and my B.Eng. degree from [Tsien's Excellence Education Program](https://www.hy.tsinghua.edu.cn/hyen/Academics/Lectures.htm), Tsinghua University.

My research interest mainly focuses on **Multi-modal Large Models Pretraining**, **VLA Pre-training** and **Data Auto-labeling & Mixture Optimization** for embodied intelligence. My previous work involves the navigation and mobile manipulation in embodied scenarios (AI2-THOR, Habitat et al.). My ultimate goal is to discover generalizable representations for a wide range of robot skills.

I am currently seeking industry or postdoctoral positions in model pretraining and data optimization for embodied intelligence. If you have positions in related areas, please feel free to contact me.

## News

- **\[05/2026\]** Co-organizing the AgiBot World Challenge 2026 at ICRA 2026!
- **\[05/2026\]** Attended the ICRA 2026 with 1 presented poster in Vienna!
- **\[01/2026\]** Granted a US Patent on robot control (US 12,521,890).
- **\[11/2025\]** Joined AgiBot as an Embodied AI Algorithm Engineer, working on VLA pre-training.
- **\[10/2023\]** Attended the IROS 2023 with 2 presented posters in Detroit!
- **\[08/2023\]** Working as a research engineer in Lenovo Research.
- **\[07/2023\]** Graduated from Tsinghua University with M.Sc. degree in Computer Science.
- **\[06/2023\]** Two papers are accepted by IROS 2023.
- **\[05/2023\]** Attended the ICRA 2023 with 1 presented poster in London!

## Education

- Sep 2024 - Present Ph.D. Student in Computer Science, Academy of Interdisciplinary Studies (AIS), Hong Kong University of Science and Technology (HKUST). Research focus: Multi-modal Large Models Pretraining, VLA Pre-training, Data Auto-labeling & Mixture Optimization.
- Sep 2020 - Jun 2023 M.Sc. in Computer Science, Department of Computer Science and Technology, Tsinghua University. Advisor: [Prof. Huaping Liu](https://sites.google.com/site/thuliuhuaping/home). Research focus: Robotic Manipulation, Visual Navigation, Imitation Learning.
- Sep 2016 - Jun 2020 B.Eng. in Engineering Mechanics (Tsien's Excellence Education Program), Tsinghua University.

## Experience

- **Embodied AI Algorithm Engineer (VLA Pre-training), AgiBot** — Nov 2025 - Present, Shanghai / Beijing
  - Architected a CoT-VLA pre-training framework based on Qwen3-VL-4B with Chain-of-Thought injection; achieved 97.5% baseline success rate on LIBERO and 95%+ with CoT reasoning.
  - Built an automated multi-source data engine (LLM APIs + local models) curating 100k+ industrial and general trajectories with filtering, phase segmentation and multi-modal tagging.
  - Validated data mixtures on physical wheeled humanoid platforms for long-horizon industrial/indoor tasks.

- **Algorithm Engineer Intern, AgileX Robotics** — Jun 2025 - Oct 2025, Shenzhen
  - Developed an OpenVLA and Qwen3-VL based dataset evaluation pipeline (tri-view feature fusion, entropy-weighted scoring, SAM 2 segmentation).
  - Fine-tuned and deployed pi0.5 base models for tabletop tasks (grasping, folding clothes, sorting) on dual-arm setups.
  - Led VLA post-training quantization studies (INT8/INT4, GPTQ, AWQ) benchmarking edge robot deployment.

- **Research Engineer (Mobile Intelligence), Lenovo Research** — Aug 2023 - Aug 2024, Beijing
  - Trained and benchmarked multi-modal perception models for personal smart devices; studied LLaMA-2 compression and quantization for mobile platforms and robotic agents.

- **Robotics Algorithm Research Intern, AI Lab, ByteDance** — May 2022 - Jul 2023, Beijing (mentored by [Dr. Tao Kong](https://www.taokong.org/))
  - Curated large-scale humanoid manipulation pre-training datasets (COCO, Visual Genome, Ego4D) adapted to embodied settings.
  - Evaluated vision backbones (CLIP, MoCo-v3, MAE) for VLA models with multi-modal masking and ablation studies.
  - Co-designed 3D online scene reconstruction for mobile manipulation service robots, validated in real-world trials.

## Research Interests

- **Multi-modal Large Models & VLA Pre-training:** training vision-language-action foundation models for target robot tasks
- **Data Auto-labeling & Mixture Optimization:** automated data annotation, data ratio optimization (DRO) for pre-training pipelines
- **Embodied Intelligence:** visual language navigation, mobile manipulation, scene understanding

{% include_relative _includes/projects.md %}

{% include_relative _includes/talks.md %}

{% include_relative _includes/services.md %}

## Resources

- <a href="assets/files/APG.zip" target="_blank">*An Efficient Accelerated Proximal Gradient (APG) Method for Large Scale SVM*</a> by Qie Sima
