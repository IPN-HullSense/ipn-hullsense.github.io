---
layout: subpage
title: VAROS Future Design
---

# Master's Project Opportunities: Shaping the Future of Subsea Autonomy through VAROS

The subsea industry is transitioning from manual ROV operations toward fully autonomous underwater robots. However, the *Sim-to-Real gap* remains a massive hurdle. By prioritizing high-fidelity environmental and physical accuracy, **VAROS (Underwater Robotics Simulation Dataset)** provides the research community with the complex multi-sensor data required for robust underwater perception, uncertainty-aware estimation and AI-analysis.

We are seeking Master's students to push the boundaries of the VAROS simulator. Your work will expand the capabilities, precision, and complexity of synthetic multi-sensor data, transforming VAROS into a world-class environment for training the next generation of underwater AI. Each project track offers several sub-topics; students may choose to specialize in one or combine multiple areas based on their interests.

![VAROS Outputs]({{ '/resources/varos/varos-outputs.jpg' | relative_url }})
*Visualization of VAROS synthetic data outputs.*

## Project 1: Complex Environments & Optical Realism

Standard simulations are often too "clean." This project focuses on extending the VAROS dataset generator to support realistic simulation of close-range underwater inspection scenarios relevant to ship hulls and harbour environments, with the **goal** of enabling systematic generation of labelled, repeatable and realistic datasets that are otherwise costly or impractical to collect. This could include:

* **Infrastructure & Harbor Ecosystems:** Integrate high-detail 3D models of ship hulls and functional harbor environments. This includes realistic textures, weld seams, frame structures, industrial markings, mooring chains, and submerged navigation hazards.
* **Turbidity:** Model backscatter and suspended particles to mimic the murky reality of coastal waters.
* **Generative Enhancement:** Explore using *Generative Models* (e.g., GANs or Diffusion) to bridge the visual gap by "style-transferring" real-world underwater noise onto synthetic frames [2].

![VAROS GAN Example]({{ '/resources/varos/varos-codealgo.jpg' | relative_url }})
*Example from previous master project using a GAN for generating realistic synthetic data outputs [2].*

## Project 2: Advanced Sensor Synthesis

Autonomy is only as good as its perception. This project focuses on expanding the VAROS multi-sensor suite with synthetic versions of high-end industrial sensors, with the **goal** of unlocking a wider range of sensor data to facilitate development of novel methods for close-range underwater inspection scenarios. This could include:

* **Acoustic Perception:** Develop a simulation model for a *3D multibeam imaging sonar* that generates realistic point clouds, accounting for acoustic noise, beam patterns, and surface reflections.
* **Multi-Camera Systems:** Implement synchronized *stereo camera* rigs to enable research into underwater visual odometry, disparity mapping, and 3D depth estimation.
* **Precision Scanning:** Integrate a synthetic *line laser scanner* capable of highly accurate 3D reconstruction.

## Project 3: Intelligent Motion & Autonomous Control

This project focuses on the *Action* part of the loop—enabling robots to navigate complex, constrained environments autonomously.

* **Constrained Motion Control:** Develop motion control that allow an AUV to maintain a precise fixed offset and orientation while "crawling" or hovering along surfaces, such as ship hulls.
* **Agent-Based Autonomy:** Implement intelligent agents that can set waypoints and autonomously plan and execute inspection paths in complex, obstacle-heavy 3D spaces.

## Prerequisites

* **Background:** Cybernetics, Robotics, or Computer Science.
* **Programming:** Proficiency in **Python** (specifically for Blender API) and/or **C++**.
* **Tools:** Experience with **Blender** or **ROS** is a significant advantage.
* **Requirement:** An NDA must be signed with the industry partner for Project 1.

## Contact Information

**Learn more:** [https://www.ntnu.edu/arosvisiongroup/varos](https://www.ntnu.edu/arosvisiongroup/varos)

* **ITK Students:** Annette Stahl // [annette.stahl@ntnu.no](mailto:annette.stahl@ntnu.no)
* **IDI Students:** Rudolf Mester // [rudolf.mester@ntnu.no](mailto:rudolf.mester@ntnu.no)

## References

[1] Zwilgmeyer, P. G. O., Yip, M., Teigen, A. L., Mester, R., & Stahl, A. (2021). The VAROS synthetic underwater data set: Towards realistic multi-sensor underwater data with ground truth. In *Proceedings of the IEEE/CVF International Conference on Computer Vision* (pp. 3722–3730).

[2] Shamba, A. K. (2025). Towards Generating Realistic Underwater Images. *arXiv preprint* arXiv:2505.14296.