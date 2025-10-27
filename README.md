<div align="center">
<h3>Rethinking Driving World Model as Synthetic Data Generator for Perception Tasks</h3>

Kai Zeng<sup>1,\*,◇</sup>, Zhanqian Wu<sup>2,*</sup>, Kaixin Xiong<sup>2</sup>, Xiaobao Wei<sup>1,◇</sup>, Xiangyu Guo<sup>3,◇</sup>, Zhenxin Zhu<sup>2</sup>, Kalok Ho<sup>2</sup>, Lijun Zhou<sup>2</sup>, Bohan Zeng<sup>1</sup>, Ming Lu<sup>2,†</sup>, Haiyang Sun<sup>2,†</sup>, Bing Wang<sup>2</sup>, Guang Chen<sup>2</sup>, Hangjun Ye<sup>2,✉</sup>, Wentao Zhang<sup>1,✉</sup>

<sup>1</sup>  Peking University
<sup>2</sup>  Xiaomi EV 
<sup>3</sup>  Huazhong University of Science and Technology

(\*) Equal contribution. (◇) Intern of Xiaomi EV. (†) Project leader. (✉)Corresponding Author.

<!-- 等arxiv的地址 -->
<a href="https://arxiv.org/abs/2510.19195"><img src='https://img.shields.io/badge/arXiv-Dream4Drive-red' alt='Paper PDF'></a>
<a href="https://wm-research.github.io/Dream4Drive/"><img src='https://img.shields.io/badge/Project_Page-Dream4Drive-green' alt='Project Page'></a>
</div>


<!-- ## Introduction -->
## Abstract
Recent advancements in driving world models enable controllable generation of high-quality RGB videos or multimodal videos. 
Existing methods primarily focus on metrics related to generation quality and controllability. 
However, they often overlook the evaluation of downstream perception tasks, which are <b>really crucial</b> for the performance of autonomous driving. 
Existing methods usually leverage a training strategy that first pretrains on synthetic data and finetunes on real data, resulting in twice the epochs compared to the baseline (real data only). 
When we double the epochs in the baseline, the benefit of synthetic data becomes negligible.
To thoroughly demonstrate the benefit of synthetic data, we introduce Dream4Drive, a novel synthetic data generation framework designed for enhancing the downstream perception tasks.
Dream4Drive first decomposes the input video into several 3D-aware guidance maps and subsequently renders the 3D assets onto these guidance maps.
Finally, the driving world model is fine-tuned to produce the edited, multi-view photorealistic videos, which can be used to train the downstream perception models.
Dream4Drive enables unprecedented flexibility in generating multi-view corner cases at scale, significantly boosting corner case perception in autonomous driving. 
To facilitate future research, we also contribute a large-scale 3D asset dataset named DriveObj3D, covering the typical categories in driving scenarios and enabling diverse 3D-aware video editing.
We conduct comprehensive experiments to show that Dream4Drive can effectively boost the performance of downstream perception models under various training epochs.

## Overview
<div align="center">
<img src="assets/overview.png" width="900">
</div>

## News
<!-- `[2025/06/18]` [ArXiv](https://arxiv.org/abs/2506.07497) paper release. Models/Code are coming soon. Please stay tuned! ☕️ -->

## Updates
- [x] Release Paper   
- [ ] Release Full Models  
- [ ] Release Inference Framework 
- [ ] Release Training Framework 


## Citation
If you find Dream4Drive is useful in your research or applications, please consider giving us a star 🌟 and citing it by the following BibTeX entry.

```bibtex
@article{zeng2025rethinking,
  title={Rethinking Driving World Model as Synthetic Data Generator for Perception Tasks},
  author={Zeng, Kai and Wu, Zhanqian and Xiong, Kaixin and Wei, Xiaobao and Guo, Xiangyu and Zhu, Zhenxin and Ho, Kalok and Zhou, Lijun and Zeng, Bohan and Lu, Ming and others},
  journal={arXiv preprint arXiv:2510.19195},
  year={2025}
}
```