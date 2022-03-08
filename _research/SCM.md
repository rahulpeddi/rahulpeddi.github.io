---
title: "Sim2Real/Real2Real Transfer Learning with Conformal Mapping"
tease: "enabled"
layout: single-portfolio
excerpt: "<img src='/images/research/SCM-teaser.png' alt='drawing' width='400px'/>"
collection: research
order_number: 30
brief: 'Planning and control methods developed in simulations can behave differently on real systems due to the gap between sim and real. However, such mismatches are usually not too significant that can potentially be corrected by stretching/extruding the input space in sim to match with the action in real. Inspired by this idea, we deliver a conformal-mapping-based frame work for transferring planning and control methods between sim-to-real/real-to-real.'
---
<style>
    o { color: #ff8e14 }
</style>


## Motivation 
Robotic applications are typically built considering specific systems. Nowadays, most of the control and the planning algorithms are developed through simulators which offer a practical and inexpensive means to create and test. However, the <o>robotic system models</o> used in simulators <o>cannot</o> perfectly <o>represent</o> what they are in <o>the real world</o>. Even though the models are well built, the <o>environment</o> that the robots interact within the simulator <o>cannot capture</o> all the <o>features</o> that happen in the reality (e.g. wind disturbance, frictions, etc.,). Due to the reasons mentioned above, when deploying the newly developed algorithms, the system can be different from the desired behaviors. This is known as **<o>Sim-to-Real gap</o>** in the field of Robotics. Besides the Sim-to-Real problem, similar gaps can also be seen when:
- Transferring planning and control method from one robot to another similar robot.
- The same system needs to be adjusted over time or under different working environments

## Goal
- **<o>Reduce the sim-to-real gap</o>** allowing a developer to quickly transfer motion planning and control methods onto a real platform.
- **<o>Transfer knowledge</o>** designed for a specific robot onto a different robot.
- **<o>Compensate for system deterioration/failures</o>** by learning quickly the limits and the proper input mapping to continue an operation.
<!-- end of the list -->

## Methodology

Typically, for a robot, the motion of the system can be characterized by a corresponding control input. Assume we treat the system in the simulator as the teacher and the system in the reality as the learner. If we can stretch the control input domain of the teacher to overlap with the control input domain of the learner so that the control input domain is geometrically identical. By considering the new stretched control input domain, the output of the teacher's controller should be able to make the teacher and the learner perform the same motion.

<p float="left">
  <img src="/images/research/SCM_intro.png" width="47%" />
  <img src="/images/research/SCM_dough.gif" width="45%" />
  <figcaption align = "left">The idea is very similar to stretch <b><i>the dough on the left</i></b>(source system's input domain) so that it will look like <b><i>the dough on the right</i></b>(target system's input domain).</figcaption>
</p>

### More details
If you are interested and want to know more details about this work, you can check [my paper](/files/pdf/publications/A_Conformal_Mapping-based_Framework_for_Robot-to-Robot_and_Sim-to-Real_Transfer_Learning.pdf) or watch my oral presentation at IROS21 in the video below. A copy of the slides showed in the video can be downloaded [here](/files/pdf/talks/IROS20_presentation_shijie_web.pdf).

<a name="SCM_youtube"></a>

<iframe width="560" height="315" src="https://www.youtube.com/embed/kPN5emkd85Q?start=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


<!-- You can find the slides in the video below and download the slides [here](/files/pdf/talks/IROS20_presentation_shijie_web.pdf)
<iframe src="/files/pdf/talks/IROS20_presentation_shijie_web.pdf#toolbar=1" width="100%" height="500" frameborder="no" border="0" marginheight="0"></iframe> -->


