# LATC — Large Area Thermal Clutch

**将平面约束、键合界面选择性加热、焊料凝固及凝固后的即时传导冷却整合为一个连续工序的大面积先进封装键合架构**

[English](README.md) · [한국어](README_KR.md)

![LATC概念图](assets/LATC_monolithic_lid_concept_KR.png)

## Rubin Ultra 四芯粒级应用

**LATC 为在传统大面积键合可能受到多方向翘曲、局部未接触及焊点不均匀限制的尺度上，实现四颗 GPU 计算芯粒单封装集成提供了一条制造路径。**

行业报道曾将早期讨论中的 Rubin Ultra 四芯粒级方案与超大封装尺度及制造性限制联系起来。但 NVIDIA 并未公开确认任何产品架构调整是由翘曲直接造成。因此，Cools 将该案例作为基于公开行业信息的工程应用场景，而不是对 NVIDIA 非公开工艺历史的事实陈述。

![Rubin Ultra 四芯粒 LATC 工艺路径](assets/Rubin_Ultra_4Die_LATC_process_route.svg)

LATC 在焊料凝固全过程保持一体式平面约束，仅对键合界面进行选择性加热，并在凝固后立即切换至高速传导冷却。其目的，是防止四芯粒封装的几何形态在翘曲状态下被锁定。

**技术说明：** [面向 Rubin Ultra 四芯粒级封装的 LATC 工艺路径](briefs/Rubin_Ultra_4Die_LATC_ZH.md)

## LATC改变的是什么

在大面积中介层与封装基板的键合过程中，封装体会因加热、冷却及材料热膨胀差异而产生翘曲。焊料一旦凝固，该变形便会被锁定在封装结构中。

LATC并非单纯强化冷却装置，而是改变键合工序的时间顺序：

1. 通过一体式上盖或刚化构件对封装体实施平面约束；
2. 仅对键合界面进行选择性加热；
3. 焊料凝固后立即将热路径切换至高速传导冷却。

其目的不是在翘曲形成后再进行矫正，而是在键合过程中防止翘曲被固化。

## 一体式上盖为何重要

分段式上盖的各个区段能够独立移动，因此可以追随已经翘曲的封装表面。一体式上盖属于单一刚体，无法以同样方式吸收曲率分量。

因此，Cools认为，一体式上盖的采用强烈表明：上盖结合时点可能已经从键合完成后的独立工序，移动到键合工序内部。

## TSMC公开结构所显示的变化

公开报道的TSMC大面积封装结构显示出由分段式上盖向一体式上盖发展的趋势。

Cools认为，仅以焊料凝固后再安装上盖的传统顺序，很难完整解释这一结构变化。若实际工序在键合期间结合一体式上盖，则该工艺架构可能与Cools已布局的键合顺序及热路径专利架构形成技术重叠。

上述判断是基于公开可观察结构作出的工程推论，并不代表Cools已确认TSMC的非公开工艺顺序。

## Cools专利布局

Cools围绕以下三个技术轴建立了相关专利族：

- 刚化构件在键合界面凝固前与基板结合；
- 由基板下方进行波长选择性键合界面加热；
- 将上述两项技术整合于同一工序的集成结构。

三个专利族合计包含**150项权利要求**。相邻的热路径切换式加压冷却专利组合包括**4件申请、137项权利要求**。

## 全球技术合作

Cools计划面向三星电子、英特尔及其他全球半导体与先进封装企业，同时包括中国相关企业，推进LATC技术评估与联合开发讨论。

合作方式可包括专利许可、工艺架构提供以及联合工艺开发。

## 知识产权保护与交易范围

本代码库所披露的技术、工艺架构、图示及实施概念，视具体技术而定，受到已授权专利、在审专利申请及Cools Inc.专有技术诀窍的保护。

Cools可与具备资质的战略合作伙伴讨论以下交易结构：

- 独占或非独占专利许可；
- 按应用领域或地域限定的权利；
- 工艺架构转让与技术支持；
- 联合开发与商业化；
- 战略投资或相关技术业务转让；
- 在商业条件适当时，相关已授权专利、专利申请及附属权利本身的转让。

**谈判并不限于专利许可。如交易目的和条件适当，相关专利组合本身也可纳入交易范围。**

所有交易均以技术及法律尽职调查和最终书面协议为前提。

## 公开技术资料

- [Rubin Ultra 四芯粒 LATC 技术说明](briefs/Rubin_Ultra_4Die_LATC_ZH.md)
- [韩文公开技术立场文件](briefs/Cools_LATC_Public_Position_Brief_KR.docx)
- [英文公开技术立场文件](briefs/Cools_LATC_Public_Position_Brief_EN.docx)
- [中文技术摘要](briefs/Cools_LATC_Public_Position_Summary_ZH.md)

## 图示

- [Rubin Ultra 四芯粒 LATC 工艺路径](assets/Rubin_Ultra_4Die_LATC_process_route.svg)
- [一体式上盖核心概念图](assets/LATC_monolithic_lid_concept_KR.png)
- [三阶段新闻图](assets/LATC_three_step_press_figure_KR.png)
- [传统工序与LATC对比图](assets/LATC_process_comparison_KR.png)

## 联系方式

**赵镇贤（Jinhyun Cho）代表 · Cools Inc.**  
电子邮箱：[jhcho@cools.co.kr](mailto:jhcho@cools.co.kr)

如需进行技术评估、媒体采访、专利许可、包含专利权的交易、技术转让、投资或联合开发，请直接发送电子邮件。也可通过[GitHub Issues](https://github.com/jhcho9494/Cools_CoWos_No_WarpageSolution/issues)留言。

## 权利声明

本代码库的公开不授予任何许可、默示权利或实施所披露技术的权限。所有专利权、申请中权利、技术资料、图示及相关商业权利均由Cools Inc.保留。

© 2026 Cools Inc. All rights reserved.