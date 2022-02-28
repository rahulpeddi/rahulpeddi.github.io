---
title: "Sim2Real/Real2Real Transfer Learning with Conformal Mapping"
tease: "enabled"
layout: single-portfolio
excerpt: "<img src='/images/research/SCM-teaser.png' alt='drawing' width='400px'/>"
collection: research
order_number: 30
brief: 'Planning and control methods developed in simulations can behave differently on real systems due to the gap between sim and real. However, such mismatches are usually not too significant that can potentially be corrected by stretching/extruding the input space in sim to match with the action in real. Inspired by this idea, we deliver a conformal-mapping-based frame work for transferring planning and control methods between sim-to-real/real-to-real.'
---

<!-- Robotic applications are typically built considering specific systems. Nowadays, most of the control and the planning algorithms are developed through simulations which offer a practical and inexpensive mean to create and test. However, as the simulation cannot be perfectly the same as the real world, there are always mismatches between the simulated world and the reality. The  researchers have to spent a good amount of time to dep
Besides the **Sim-to-Real gap**, similar gaps can also be seen when:
-  -->


This paper presents a novel method for transferring motion planning and control policies between a teacher and a learner robot. With this work, we propose to reduce the sim-to-real gap, transfer knowledge designed for a specific system into a different robot, and compensate for system aging and failures. To solve this problem we introduce a Schwarz–Christoffel mapping-based method to geometrically stretch and fit the control inputs from the teacher into the learner command space. We also propose a method based on primitive motion generation to create motion plans and control inputs compatible with the learner's capabilities. Our approach is validated with simulations and experiments with different robotic systems navigating occluding environments.


<a name="SCM_youtube"></a>

<iframe width="560" height="315" src="https://www.youtube.com/embed/kPN5emkd85Q?start=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


You can find the slides in the video below and download the slides [here](/files/pdf/talks/IROS20_presentation_shijie_web.pdf)
<iframe src="/files/pdf/talks/IROS20_presentation_shijie_web.pdf#toolbar=1" width="100%" height="500" frameborder="no" border="0" marginheight="0"></iframe>


