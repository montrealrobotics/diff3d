---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

permalink: /
title: Home
layout: home
---

> With four parameters I can fit an elephant, and with five I can make it wiggle its trunk.
> – John Von Neumann (abridged)

“Differentiable programs” are parameterized programs that allow themselves to be rewritten by gradient-based optimization. They are ubiquitous in modern machine learning and computer vision. Recently, explicitly encoding our knowledge of the rules of the world in the form of differentiable programs has become quite popular. In particular, differentiable realizations of rendering, projective geometry, optimization to name a few, have enabled the design of several novel computer vision techniques. Many approaches have been proposed for unsupervised learning of depth estimation [1‒6] using differentiable image warping. Differentiable 3D reconstruction pipelines [7, 8] have demonstrated the potential for task-driven representation learning. A number of differentiable rendering approaches [9‒14] have been shown to enable single-view 3D reconstruction and other inverse graphics tasks (without requiring any form of 3D supervision). While these advances have largely occurred in isolation, recent efforts [15‒20] have attempted to bridge the gap between the aforementioned areas. Narrowing the gaps between these otherwise isolated disciplines holds tremendous potential to yield new research directions and solve long-standing problems, particularly in understanding and reasoning about the world.

Hence, we present the “workshop on differentiable 3D vision and graphics” to
* Narrow the gap and foster synergies between the computer vision, graphics, and machine learning communities.
* Debate the promise and perils of differentiable methods, and identify challenges that need to be overcome.
* Raise awareness about these techniques to the broader CV community.
* Discuss the broader impact of such techniques, and any ethical implications thereof.

The primary focus areas of this workshop are:
* **Differentiable geometric computer vision** techniques, including, but not limited to, differentiable depth and pose estimation, feature extraction and matching pipelines, pointset alignment, reconstruction pipelines, and their applications.
* **Differentiable geometry processing and graphics** tools which are increasingly being adopted into vision pipelines, including, but not limited to, differentiable mesh manipulation, rendering, higher-order light transport, and their applications.
* **Applications and limitations of differentiable methods**. Differentiable graphics and rendering might allow for more accurate novel viewpoint synthesis. Differentiable rendering is being used increasingly used for self-supervised 3D reconstruction from a single image. Implicit representations are being learned via differentiable rendering [21].  However, there are also limitations: gradients are not always useful in long-horizon scenarios; differentiable methods are often applicable only where precise process models are available; they also require good initializations. How can differentiable methods be combined with gradient-free optimization (or other techniques) to circumvent these issues?

Notably, most of the advances in our focus areas have occurred in the last 3-4 years, and the interest in this nascent field is fast growing (evident from the push towards the release of open-source tools such as Kaolin [18], PyTorch3D [19], Kornia [20] and more).

## Timeline

Please see our [call for papers](callforpapers) for more details. All deadlines below are 11.59 pm on the specified day, [anywhere-on-Earth time](https://www.timeanddate.com/time/zones/aoe).

|------------------------------------|---------------------------|-------------------------------|------------------|
|Event                               | Archival submission track | Non-archival submission track | Mentorship track |
|------------------------------------|---------------------------|-------------------------------|------------------|
|First-round deadline (if applicable)| N/A                       | N/A                           | 2 August 2021    |
|Final submission deadline           | 2 August 2021             | 1 September 2021              | 1 September 2021 |
|Decisions announced                 | 12 August 2021            | 15 September 2021             | 15 September 2021|
|Camera-ready submissions due        | 16 August 2021            | 1 October 2021                | 1 October 2021   |
|------------------------------------|---------------------------|-------------------------------|------------------|


### References

1. Garg R., B.G. V.K., Carneiro G., Reid I. Unsupervised CNN for Single View Depth Estimation: Geometry to the Rescue. ECCV 2016.
2. Zhou T., Brown M., Snavely N., Lowe D. Unsupervised Learning of Depth and Ego-Motion from Video. CVPR 2017.
3. Godard C., Aodha O., Brostow G. Unsupervised Monocular Depth Estimation with Left-Right Consistency. CVPR 2017.
4. Godard C., Aodha O., Firman M., Brostow, G. Digging into Self-Supervised Monocular Depth Prediction. ICCV 2019.
5. Guizilini V., Ambrus R., Pillai S., Raventos A., Gaidon A. PackNet-SfM: 3D Packing for Self-Supervised Monocular Depth Estimation. CVPR 2020.
6. Luo X., Huang, J., Szeliski R., Matzen K., Kopf J. Consistent Video Depth Estimation. SIGGRAPH 2020.
7. Zhou H., Ummenhofer B., Brox T. DeepTAM: Deep Tracking and Mapping. ECCV 2018.
8. Jatavallabhula K., Iyer G., Paull L. gradSLAM: Dense SLAM meets automatic differentiation.  ICRA 2020.
9. Loper M., Black M. OpenDR: An Approximate Differentiable Renderer. ECCV 2014.
10. Kato H., Ushiku Y., Tatsuya H. Neural 3D Mesh Renderer. CVPR 2018.
11. Liu S., Li T., Chen W., Li H. Soft Rasterizer: A Differentiable Renderer for Image-based 3D Reasoning. ICCV 2019.
12. Chen W., Gao J., Ling H., Smith E., Lehtinen J., Jacobson A., Fidler S. Learning to Predict 3D Objects with an Interpolation-based Differentiable Renderer. Neurips 2019.
13. Li T., Aittala M., Fredo D., Lehtinen J. Differentiable Monte Carlo Ray Tracing through Edge Sampling. SIGGRAPH Asia 2018.
14. Nimier-David M., Vicini D., Zeltner T., Jakob W. Mitsuba 2: A Retargetable Forward and Inverse Renderer. SIGGRAPH Asia 2019.
15. Guen V., Thome N. Disentangling Physical Dynamics from Unknown Factors for Unsupervised Video Prediction. CVPR 2020.
16. Jatavallabhula K., Macklin M., Golemo F., Voleti V., Petrini L., Wiess M., Considine B., Parent-Levesque J., Xie K., Erleben K., Paull L., Shkurti F., Fidler S., Nowrouzezahrai D. gradSim: Differentiable physics and rendering engines for parameter estimation from video.
17. Jaques M., Burke M., Hospedales T. Physics-as-inverse-graphics:Joint unsupervised learning of objects and physics from video. ICLR 2020.
18. Jatavallabhula K., Smith E., Lafleche J., Tsang C., Rozantsev A., Chen W., Xiang T., Lebaredian R., Fidler S. Kaolin: A PyTorch Library for Accelerating 3D Deep Learning Research. arXiv 2019.
19. Ravi N., Reizenstein J., Novotny D., Gordon T., Lo W., Johnson J., Gkioxari G. Pytorch3D (https://github.com/facebookresearch/pytorch3d).  2020 (accessed June 15 2020)
20. Riba E., Mishkin D., Ponsa D., Rublee E., Bradski G. Kornia: an Open Source Differentiable Computer Vision Library for PyTorch. WACV 2020.
21. Mildenhall B., Srinivasan P., Tanick M., Barron J., Ramamoorthi R., Ng R. Representing Scenes as Neural Radiance Fields for View Synthesis. ECCV 2020.
