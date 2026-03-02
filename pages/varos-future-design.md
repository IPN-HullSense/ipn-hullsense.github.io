---
layout: subpage
title: VAROS Future Design
---

# Master’s Thesis Opportunities: Shaping the Future of Subsea Autonomy Through VAROS

The subsea industry is transitioning from manual ROV operations toward fully autonomous underwater robots. However, the Sim-to-Real gap remains a massive hurdle. By prioritizing high-fidelity environmental and physical accuracy, *VAROS (Underwater Robotics Simulation Dataset)* provides the research community with the complex multi-sensor data required for robust underwater perception, uncertainty-aware estimation and AI-analysis.

We are seeking Master's students to push the boundaries of the VAROS simulator. Your work will expand the capabilities, precision, and complexity of synthetic multi-sensor data, transforming VAROS into a world-class environment for training the next generation of underwater AI. Each project track offers several sub-topics; students may choose to specialize in one or combine multiple areas based on their interests.

![VAROS Outputs]({{ '/resources/varos/varos-outputs.jpg' | relative_url }})
*Visualization of VAROS synthetic data outputs for underwater perception training.*
---

<a id="varos-track1"></a>
### Project Track 1: Complex AI- and Model-Driven Environments & Optical Realism
*Standard simulations are often too "clean." This track focuses on modeling the physical complexity of subsea infrastructure and the unique optical challenges of the water column.*

**Available focus areas:**
* **Infrastructure & Harbor Ecosystems:** Integrate high-detail 3D models of ship hulls and functional harbor environments. This includes realistic textures, weld seams, frame structures, industrial markings, mooring chains, and submerged navigation hazards.
* **Advanced Underwater Optics:** * **Refraction:** Incorporate the refraction phenomenon underwater (Ref: *An Optical Digital Twin for Underwater Photogrammetry*, 2021).
    * **Turbidity & Marine Snow:** Model backscatter and suspended particles to mimic the "murky reality" of the North Sea.
* **Generative Enhancement:** Explore using **Generative Models** (e.g., GANs or Diffusion) to bridge the visual gap by "style-transferring" real-world underwater noise onto synthetic frames (Ref: Towards Generating Realistic Underwater Images, 2025).

---

<a id="varos-track2"></a>
### Project Track 2: Advanced Sensor Synthesis
*Autonomy is only as good as its perception. This track focuses on expanding the VAROS multi-sensor suite with synthetic versions of high-end industrial sensors.*

**Available focus areas:**
* **Acoustic Perception:** Develop a simulation model for a **3D multibeam imaging sonar** that generates realistic point clouds, accounting for acoustic noise, beam patterns, and surface reflections.
* **Multi-Camera Systems:** Implement synchronized **stereo camera** rigs to enable research into underwater visual odometry, disparity mapping, and 3D depth estimation.
* **Precision Scanning:** Integrate a synthetic **line laser scanner** capable of millimeter-accurate 3D reconstruction for inspecting hull defects, welds, or biological growth.

---
<a id="varos-track3"></a>
### Project Track 3: Intelligent Motion & Autonomous Control
*This track focuses on the "Action" part of the loop—enabling robots to navigate complex, constrained environments autonomously.*

**Available focus areas:**
* **Constrained Motion Control:** Develop motion control that allow an AUV to maintain a precise fixed offset and orientation while "crawling" or hovering along curved ship hulls.
* **Agent-Based Autonomy:** Implement intelligent agents (using Reinforcement Learning or advanced path planning) that can autonomously plan and execute inspection paths in complex, obstacle-heavy 3D spaces.

---

### Prerequisites
We are looking for students with a background in **Cybernetics, Robotics, Computer Science, or Marine Engineering**.
* **Programming:** Strong proficiency in **Python** (specifically for API integration) and/or **C++**.
* **Tools:** Experience with **Blender** (the engine powering VAROS) is a significant advantage. Familiarity with **ROS** is highly relevant.

---

**Ready to dive in?**
**Learn more:** [ntnu.edu/arosvisiongroup/varos](https://www.ntnu.edu/arosvisiongroup/varos)  
**Contact:** [Insert Name/Email]