---
title: ''
summary: 'Keyuan Luo — robot learning, memory-augmented vision-language-action models, and multimodal perception.'
type: landing

sections:
  - block: resume-biography-3
    id: about
    content:
      username: me
      text: |-
        I am a PhD student at the Technical University of Munich, advised by [Prof. Ziyue Li](https://bonaldli.github.io/), and a lecturer at Hainan Bielefeld University of Applied Sciences.

        My research focuses on **robot learning**, especially **memory evaluation in vision-language-action (VLA) systems** and **long-horizon decision-making**. I also study multimodal policy adaptation. Previously, I worked on pedestrian crossing intention prediction at Technische Universität Berlin.
      button:
        text: Email
        url: 'mailto:luokeyuanstu@163.com'
      headings:
        about: About Me
        education: Education
        interests: Research Interests
    design:
      spacing:
        padding: ['0', '0', '0', '0']
      background:
        gradient_mesh:
          enable: true
      name:
        size: md
      avatar:
        size: medium
        shape: circle

  - block: markdown
    id: papers
    content:
      title: Papers and Preprints
      subtitle: ''
      text: |-
        [Google Scholar](https://scholar.google.com/citations?user=n-qWn-QAAAAJ&hl=zh-CN)

        ### 2026

        **[Beyond Success Rate: Interventional Evaluation of Memory in Vision-Language-Action Systems](https://arxiv.org/abs/2610.23372)**

        **Keyuan Luo**, Yi Xie, Wanyun Ling, Yuanzhe Li, Ziyue Li, Zhuoqi Zeng.

        *arXiv preprint, 2026* · [PDF](https://arxiv.org/pdf/2610.23372) · [Research overview](/#research)

        ---

        **[Retrieval-triggered Action Projection Adjustment for Frozen VLA Policies: An Empirical Study and Failure Analysis](https://arxiv.org/abs/2610.24573)**

        Jinming Wang, Ruiheng Zhang, Yong Wang, Zipan Xiong, **Keyuan Luo**.

        *arXiv preprint, 2026* · [PDF](https://arxiv.org/pdf/2610.24573)

        ---

        **[From Sliding Windows to Self-evolving Lifelong Memory: A Dual-perspective Survey of Memory Paradigms for Long-Horizon Robotics VLA Models](https://arxiv.org/abs/2610.23319)**

        Yong Wang, Boyu Shen, Xinwei Zhang, Yizheng Li, **Keyuan Luo**.

        *arXiv preprint, 2026* · [PDF](https://arxiv.org/pdf/2610.23319)
    design:
      columns: '1'

  - block: markdown
    id: research
    content:
      title: Featured Research
      subtitle: ''
      text: |-
        ### IMEP and ChainBench

        **When a robot's memory changes its behavior, is it actually using the stored facts?**

        <a href="/media/imep-overview.pdf" aria-label="View the original IMEP overview figure as a PDF"><img src="/media/imep-overview-hd.png" alt="IMEP overview: four evaluation questions and experiments with within-episode, cross-episode, and agentic memory" width="3200" height="1892" loading="lazy" decoding="async" style="width:100%;height:auto;"></a>

        *Figure 1 from the preprint. All experiments use simulated robotic environments; interpretation details are given in the paper.*

        **Approach.** IMEP compares changes to task-relevant facts with control interventions, separating decision accuracy from motor execution. ChainBench is a LIBERO-based benchmark that requires information from earlier episodes.

        **Main finding.** The evaluated learned memory banks showed behavioral sensitivity without established fact-specific memory use. In the 202-chain ChainBench study, full memory achieved 74.3% task success versus 39.1% without memory, using shared recorded executions. These results apply to the tested configurations.

        **My contribution.** I led study design, implementation, experiments, analysis, and manuscript drafting. Coauthor support included overall research guidance from Ziyue Li, manuscript refinement from Yi Xie, and overview-figure refinement from Wanyun Ling.

        [Paper](https://arxiv.org/abs/2610.23372) · [PDF](https://arxiv.org/pdf/2610.23372) · [High-resolution figure](/media/imep-overview-hd.png) · [Original figure PDF](/media/imep-overview.pdf)

        *Code is not yet publicly available.*
    design:
      columns: '1'
      spacing:
        padding: ['48px', '0', '48px', '0']

  - block: markdown
    id: other-research
    content:
      title: Other Research
      subtitle: ''
      text: |-
        ### PCIT: Pedestrian Crossing Intention Prediction

        *Master's thesis, Technische Universität Berlin*

        My master's research investigated multimodal pedestrian crossing intention prediction using a cross-modal Transformer and uncertainty-based loss weighting for multi-task learning. The approach was evaluated on the JAAD and PIE datasets.
    design:
      columns: '1'

  - block: markdown
    id: competitions
    content:
      title: Robotics Competitions
      subtitle: ''
      text: |-
        ### AgiBot World Challenge 2026

        **Depth-augmented ACoT-VLA**

        **Role:** Team Lead · **Team:** BIUH_TUM · **Result:** Tenth Place

        *RoboChallenge ICRA Competition, ICRA 2026*

        I worked on adapting a pretrained pi0.5-LIBERO policy to the competition's robotic tasks. The project explored LoRA-based adaptation with depth information and iterative evaluation in Genie Sim 3.0.

        ![Depth-augmented ACoT-VLA inference architecture](https://keyuanluo.github.io/research/agibot/architecture.png)

        *Visual-language context, depth conditioning, and coarse-to-fine action generation.*

        **[Project details](/research/agibot/)** · [Architecture PDF](/research/agibot/architecture.pdf) · [View certificate](/research/agibot/#competition-result)
    design:
      columns: '1'

  - block: markdown
    id: teaching
    content:
      title: Teaching and Mentoring
      subtitle: ''
      text: |-
        I am a lecturer at Hainan Bielefeld University of Applied Sciences. My teaching covers robotics, introductory artificial intelligence, deep learning, Python, and C++. I also mentor students in robot-learning research.

    design:
      columns: '1'

  - block: markdown
    id: robotics-laboratory
    content:
      title: Robotics Laboratory
      subtitle: 'Hainan Bielefeld University of Applied Sciences'
      text: |-
        Explore the laboratory's humanoid platforms, mobile robots, vehicle platforms, and working environment.

        ![Robotic platforms at Hainan Bielefeld University of Applied Sciences](lab-platforms.jpg)

        *Robotic platforms at Hainan Bielefeld University of Applied Sciences.*

        **[Explore the laboratory →](/lab/)**
    design:
      columns: '1'

  - block: markdown
    id: contact
    content:
      title: Contact
      subtitle: ''
      text: |-
        For research enquiries, please contact me by email.

        **Email:** [luokeyuanstu@163.com](mailto:luokeyuanstu@163.com)

        **GitHub:** [github.com/keyuanluo](https://github.com/keyuanluo)

        **Google Scholar:** [Publication profile](https://scholar.google.com/citations?user=n-qWn-QAAAAJ&hl=zh-CN)
    design:
      columns: '1'
---
