---
title: "Data Center Cooling System Optimization Using Offline Reinforcement Learning"
author: "Xianyuan Zhan, Xiangyu Zhu, Peng Cheng, et al."
conference: "ICLR 2025"
layout: default
---
<style>
  .l-text {
    font-size: 24px;
  }
  .m-text{
    font-size: 20px;
  }
  .s-text {
    font-size: 16px;
  }
</style>

<center>
<span class="l-text">
<b>
Data Center Cooling System Optimization Using Offline Reinforcement Learning
</b>
</span>
<br><br>
Xianyuan Zhan<sup>1,2∗†</sup>, Xiangyu Zhu<sup>1∗</sup>, Peng Cheng<sup>1</sup>, Xiao Hu<sup>1</sup>, Ziteng He<sup>1</sup>, Hanfei Geng<sup>1</sup>, Jichao Leng<sup>1</sup>, Huiwen Zheng<sup>3</sup>, Chenhui Liu<sup>3</sup>, Tianshun Hong<sup>3</sup>, Yan Liang<sup>3</sup>, Yunxin Liu<sup>1,2†</sup>, Feng Zhao<sup>1†</sup>
<br><br>
<sup>1</sup> Institute for AI Industry Research, Tsinghua University

<sup>2</sup> Shanghai Artificial Intelligence Laboratory 

<sup>3</sup> Global Data Solutions Co., Ltd.
<br><br>
{zhanxianyuan, liuyunxin}@air.tsinghua.edu.cn, fz@alum.mit.edu 

**Publication:** The Thirteenth International Conference on Learning Representations (ICLR 2025) 

**[📄 论文链接](https://arxiv.org/html/2501.15085v1)**  
</center>


<center>
<span class="m-text">
<b>Abstract</b>
</span>

The recent advances in information technology and artificial intelligence have fueled a rapid expansion of the data center (DC) industry worldwide, accompanied by an immense appetite for electricity to power the DCs. In a typical DC, around 30-40% of the energy is spent on the cooling system rather than on computer servers, posing a pressing need for developing new energy-saving optimization technologies for DC cooling systems. However, optimizing such real-world industrial systems faces numerous challenges, including but not limited to a lack of reliable simulation environments, limited historical data, and stringent safety and control robustness requirements. In this work, we present a novel physics-informed offline reinforcement learning (RL) framework for energy efficiency optimization of DC cooling systems. The proposed framework models the complex dynamical patterns and physical dependencies inside a server room using a purposely designed graph neural network architecture that is compliant with the fundamental time-reversal symmetry. Because of its well-behaved and generalizable state-action representations, the model enables sample-efficient and robust latent space offline policy learning using limited real-world operational data. Our framework has been successfully **deployed and verified** in a large-scale production DC for closed-loop control of its air-cooling units (ACUs). We conducted a total of **2000 hours** of short and long-term experiments in the production DC environment. The results show that our method achieves **14-21%** energy savings in the DC cooling system, without any violation of the safety or operational constraints. We have also conducted a comprehensive evaluation of our approach in a real-world DC testbed environment. Our results have demonstrated the significant potential of offline RL in solving a broad range of data-limited, safety-critical real-world industrial control problems.
</center>

<center>
<span class="m-text">
<b>Method</b>
</span>

The physics-informed offline RL framework for energy-efficient DC cooling control
</center>

![alg_fram](./doc/alg_framework.png)

<center>
<span class="m-text">
<b>
Experimental Results
</b>
</span>
</center>

Comparison of conventional PID control and our approach under comparable server load settings on two server rooms of the commercial DC. “AEP” and “EC” denote average electric power and energy consumption, respectively. We use the offline RL policy to control 4, 6, and all the ACUs in each room. ACLF is the air-side cooling load factor, calculated as the ratio of energy consumption of ACUs to servers, the lower the better.
![table1](./doc/table.png)

**a**, ACLF values under varying total server loads from the 14-day long-term experiment in Server Room B. **b, c**, the energy-saving impact of controlling different numbers of ACUs through our approach, conducted over seven morning periods (10:30 - 13:30) in Server Room A and B.
![long_term](./doc/long_term_exp.png)

<center>
<span class="m-text">
<b>
Citation (BibTeX)
</b>
</span>
</center>

```bibtex
@inproceedings{
zhan2025data,
title={Data Center Cooling System Optimization Using Offline Reinforcement Learning},
author={Xianyuan Zhan, Xiangyu Zhu, Peng Cheng, Xiao Hu, Ziteng He, Hanfei Geng,
Jichao Leng, Huiwen Zheng, Chenhui Liu, Tianshun Hong, Yan Liang, Yunxin Liu, Feng Zhao},
booktitle={The Thirteenth International Conference on Learning Representations},
year={2025},
url={https://arxiv.org/html/2501.15085v1}
}
```
