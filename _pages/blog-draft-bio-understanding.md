---
layout: archive
title: "Draft"
permalink: /blogs/draft/
author_profile: true
toc: true
date: 2023-09-01
---

## Limitations

It's a pity to announce that <font color="red">the project did NOT accomplish all of its stated goals during the period of URA funding</font>:

- Take-off from the ground :heavy_check_mark:
- Take-off from the water surface :x:
- Fly in the air :heavy_check_mark:
- Controlled motion in the air :x:
- Move on the water surface :heavy_check_mark:
- Controlled motion on the water surface :x:
- Controlled motion in the water :x:

Despite exciting initial results, by the fall of 2022, I was finding it increasingly difficult to move forward. 

- Control of the ornithopter required high expertise in vortex aerodynamics and underactuated systems, which was far beyond my knowledge.
- The micro-coreless motors I could afford were limited in power (my prototype was hard to take off, and there was no room to continue adding equipment) and didn't support precise speed and position control. Micro DC servo motors might work but be too expensive for the URA grant. 

With the mutual agreement between the CUHK-Shenzhen URA committee and me, this project was finally terminated in October 2022.

## Reflection --- What Bionic Robotics Taught Me

Although this project did not achieve the expected results, I still gained a lot from it, not only in knowledge, but also in research. This project was a watershed moment for me. Before doing this project, my mantra was to build cool robots. This project forced me to think hard about the science behind the robots. 

When building this ornithopther prototype, I found an interesting phenomenon --- **not all flapping-wing robots can take off from the ground by themselves**. Some existing robots ([DelFly](https://www.delfly.nl/), [Hummingbird](https://www.youtube.com/watch?v=GCEbEL_EmyQ), [Robobee](https://wyss.harvard.edu/technology/robobees-autonomous-flying-microrobots/), [MetaFly](https://www.bionicbird.com/world/metafly-page)) have demonstrated the ability to take off from the ground, while others ([小隼](https://www.bilibili.com/video/BV12L4y1b7K2/?vd_source=1bcf36ba276d5029a29aca337d5d3a4a), [MetaBird](https://www.bionicbird.com/world/metabird-page), [BionicSwift](https://www.festo.com/ca/en/e/about-festo/research-and-development/bionic-learning-network/highlights-from-2015-to-2017/bionicswift-id_326830/)) need to be released from the air. The reasons for this are not explained in detail in the papers on these robotic systems.

Both [successful](#take-off-successfully---large-aoa) and [unsuccessful](#take-off-failed---small-aoa) take-offs from the ground were observed when my prototype was in flight tests. Through long-term experiments and control variates, I eventually found a key factor --- the initial [angle of attack (AoA)](https://en.wikipedia.org/wiki/Angle_of_attack) of the wings. I found there was a critical AoA (although i can't quantify). _**If and only if the initial AoA was large than the critical AoA, the robot could generate sufficient lift to take off**_. Sometimes the robot even created downward pressure when the initial AoA was less than the critical AoA. 

![paper](/images/blogs/bio-understanding/aoa.png)

I have to admit that I did have this as my new academic discovery for a while, and even imagined that I would be famous in the academic world for pointing out this law. Until one day when I searched the literature, I found that this law and the principle behind it had been written in a paper ([Lift and Power Requirements of Hovering Insect Flight](https://link.springer.com/article/10.1007/BF02484580)) published almost 20 years ago. :joy:

![paper](/images/blogs/bio-understanding/paper.png)

Although it turned out to be an oolong in the end, the ecstasy of verifying a natural law through my own efforts is something I will never forget in my life. This fantastic experience made me realize for the first time that **engineering can be used as a tool to understand natural science**. As Feynman's famous saying goes, "What I cannot create, I do not understand."

![feynman](/images/blogs/bio-understanding/feynman.png)

## Demonstrations

Table of contents:
- [Limitations](#limitations)
- [Reflection --- What Bionic Robotics Taught Me](#reflection-----what-bionic-robotics-taught-me)
- [Demonstrations](#demonstrations)
  - [Take-off and stay in the air](#take-off-and-stay-in-the-air)
  - [Advance on the water](#advance-on-the-water)
  - [Take-off successfully - large AoA](#take-off-successfully---large-aoa)
  - [Take-off failed - small AoA](#take-off-failed---small-aoa)
- [Related](#related)

---

### Take-off and stay in the air

Here are the sequential screenshots of the take-off process:

![take-off](/images/blogs/bio-understanding/take-off.png)

Here is the video demo:

<video controls style="width: 100%; height: auto;" controlsList="nodownload" oncontextmenu="return false;" preload="auto">
  <source src="/files/webm/fly.webm" type="video/webm">
  Your browser does not support the video tag.
</video>

---

### Advance on the water

Here are the sequential screenshots of advancing on the water surface by flapping wings:

![advance](/images/blogs/bio-understanding/swimming.png)

Here is the video demo:

<video controls style="width: 100%; height: auto;" controlsList="nodownload" oncontextmenu="return false;" preload="auto">
  <source src="/files/webm/swim.webm" type="video/webm">
  Your browser does not support the video tag.
</video>

---

### Take-off successfully - large AoA

Here are the sequential screenshots of a successful take-off, with large initial angle of attack (AoA):

![large-aoa](/images/blogs/bio-understanding/large-aoa.png)

Here is the video demo:

<video controls style="width: 100%; height: auto;" controlsList="nodownload" oncontextmenu="return false;" preload="auto">
  <source src="/files/webm/large-aoa.webm" type="video/webm">
  Your browser does not support the video tag.
</video>

---

### Take-off failed - small AoA

Here are the sequential screenshots of a failed take-off, with small initial angle of attack (AoA):

![small-aoa](/images/blogs/bio-understanding/small-aoa.png)

Here is the video demo:

<video controls style="width: 100%; height: auto;" controlsList="nodownload" oncontextmenu="return false;" preload="auto">
  <source src="/files/webm/small-aoa.webm" type="video/webm">
  Your browser does not support the video tag.
</video>

## Related

Some projects & products I referred to: 
* [DelFly](https://www.delfly.nl/) --- Micro Air Vehicles Laboratory, Delft University of Technology, Netherlands.
* [Hummingbird](https://www.youtube.com/watch?v=GCEbEL_EmyQ) --- Bio-Robotics Lab, Purdue University, USA.
* [Robobee](https://wyss.harvard.edu/technology/robobees-autonomous-flying-microrobots/) --- Harvard Microrobotics Lab, Harvard University, USA.
* [小隼](https://www.bilibili.com/video/BV12L4y1b7K2/?vd_source=1bcf36ba276d5029a29aca337d5d3a4a) --- Northwestern Polytechnical University, China.
* [MetaFly](https://www.bionicbird.com/world/metafly-page) and [MetaBird](https://www.bionicbird.com/world/metabird-page) --- Bionicbird, France.
* [BionicSwift](https://www.festo.com/ca/en/e/about-festo/research-and-development/bionic-learning-network/highlights-from-2015-to-2017/bionicswift-id_326830/) --- Festo, Germany.

Some papers I found useful for understading insect flight:
* M. H. Dickinson, F.-O. Lehmann, and S. P. Sane, "[Wing Rotation and the Aerodynamic Basis of Insect Flight](https://www.science.org/doi/epdf/10.1126/science.284.5422.1954)," _Science_, vol. 284, no. 5422, pp. 1954–1960, 1999.
* M. Sun and D. Gang, “[Lift and Power Requirements of Hovering Insect Flight](https://link.springer.com/article/10.1007/BF02484580)," _Acta Mechanica Sinica_, vol. 19, pp. 458–469, 10 2003.
* K. S. Wu, J. Nowak, and K. S. Breuer, “[Scaling of the Performance of Insect-Inspired Passive-Pitching Flapping Wings](https://royalsocietypublishing.org/doi/10.1098/rsif.2019.0609),” _Journal of the Royal Society Interface_, vol. 16, 2019
