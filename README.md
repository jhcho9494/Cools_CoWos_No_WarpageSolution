# 🔒 Patent-Protected Technology · 🤝 Open to Technology Transactions

> **한국어**  
> 본 저장소를 포함하여 Cools가 공개하는 모든 핵심 기술은 **등록특허 및 출원 중 특허로 보호되고 있습니다.** 공개는 기술사용 허락을 의미하지 않습니다. 그러나 Cools는 기술을 폐쇄적으로 묶어두지 않습니다. **기업 규모·국가·기관 형태와 관계없이 기술도입, 특허 라이선스, 특허양도, 공동개발, 제조협력 및 사업화 제안을 적극 환영합니다.**  
> **무단 사용에는 단호하게 대응하고, 정당한 기술거래에는 누구에게나 문을 엽니다. 기술이 필요하다면 우회하거나 모방하지 말고 Cools와 직접 거래하십시오.**
>
> **English**  
> All core technologies disclosed by Cools, including those presented in this repository, are **protected by granted patents and pending patent applications.** Public disclosure does not constitute permission to use the technology. At the same time, Cools does not intend to keep valuable technology locked away. **We actively welcome technology adoption, patent licensing, patent assignment, joint development, manufacturing collaboration, and commercialization proposals from companies, institutions, and partners worldwide.**  
> **Unauthorized use will be addressed firmly. Legitimate technology transactions are welcome from everyone. If you need the technology, do not work around it or imitate it—deal directly with Cools.**
>
> **中文**  
> Cools公开的所有核心技术，包括本代码库所展示的技术，均受到**已授权专利及在审专利申请的保护。** 技术公开不代表授予任何实施许可。同时，Cools并不希望让有价值的技术被封闭闲置。**无论企业规模、国家或机构类型，我们均积极欢迎技术导入、专利许可、专利转让、联合开发、制造合作及商业化提案。**  
> **对于未经授权的使用，我们将坚决应对；对于正当的技术交易，我们向所有合作方开放。需要该技术，请勿规避或模仿，请直接与Cools洽谈。**

### **Protected Technology. Open for Business. · 특허로 보호하고, 기술거래에는 완전히 열려 있습니다. · 专利保护，交易开放。**

---

# LATC — Large Area Thermal Clutch

**Large-area advanced-packaging bonding architecture integrating planar constraint, joint-selective heating, solder solidification, and immediate conductive cooling.**

[한국어](README_KR.md) · [中文](README_ZH.md)

![LATC concept](assets/LATC_monolithic_lid_concept_KR.png)

## Rubin Ultra 4-die-class application

**LATC provides a manufacturing route for restoring a single-package four-compute-die architecture at a scale where conventional large-area bonding can become limited by multidirectional warpage, local contact loss, and solder-joint nonuniformity.**

Industry reporting has associated an originally discussed four-die Rubin Ultra-class configuration with extreme-scale packaging and manufacturability constraints, while NVIDIA has not publicly confirmed warpage as the reason for any architecture change. Cools therefore presents this as an engineering application scenario based on reported industry information—not as a statement of NVIDIA's confidential process history.

![Rubin Ultra 4-die LATC process route](assets/Rubin_Ultra_4Die_LATC_process_route.svg)

LATC maintains monolithic planar constraint through solder solidification, heats the bonding interface selectively, and switches immediately to high-speed conductive cooling. The objective is to prevent the four-die package geometry from being locked into a warped state.

**Technical note:** [Rubin Ultra 4-Die-Class Packaging: A LATC Process Route](briefs/Rubin_Ultra_4Die_LATC_EN.md)

## What LATC changes

Large-area interposer-to-substrate bonding is constrained by warpage generated during heating and cooling. Once solder solidifies, that deformation becomes locked into the package.

LATC changes the sequence itself:

1. The package is held flat by a monolithic lid or stiffening member.
2. Energy is delivered selectively to the bonding interface.
3. Immediately after solidification, the thermal path is switched to high-speed conductive cooling.

The objective is not to flatten a package after warpage has formed. It is to prevent warpage from being locked in during the bonding interval.

## Why the monolithic lid matters

A segmented lid can follow an already warped package because each segment can move independently. A monolithic lid cannot absorb the curvature component in the same way.

Cools therefore assesses that adoption of a monolithic lid is a strong indication that lid attachment has moved from a post-bonding operation into the bonding process itself.

## TSMC and the observed architecture

Publicly reported TSMC large-area package structures indicate a transition toward a monolithic lid architecture.

Cools assesses that this change is difficult to reconcile with a process in which the lid is attached only after joint solidification. If the actual process attaches the lid during the bonding interval, the resulting process architecture may overlap with the bonding-sequence and thermal-path architecture claimed by Cools.

This is an engineering inference based on publicly observable structure. It is not a confirmation of TSMC's non-public process sequence.

## Cools patent position

Cools has established three related patent families covering:

- pre-solidification joining of the stiffening member;
- wavelength-selective joint heating through the underside of the substrate; and
- the integrated process combining both elements.

These families comprise **150 claims**. An adjacent thermal-path-switching and pressurized-cooling portfolio comprises **4 filings and 137 claims**.

## Related Cools technology — CoolVia

**CoolVia** is Cools' independent PEI/PEIE-enabled continuous metallization platform for through-glass vias and glass-core substrates.

- [CoolVia repository — English](https://github.com/jhcho9494/Cools_CoolVia_Glass_Metallization)
- [CoolVia 기술자료 — 한국어](https://github.com/jhcho9494/Cools_CoolVia_Glass_Metallization/blob/main/README_KR.md)
- [CoolVia 技术资料 — 中文](https://github.com/jhcho9494/Cools_CoolVia_Glass_Metallization/blob/main/README_ZH.md)

## Global collaboration

Cools plans to pursue technical review and joint-development discussions with Samsung Electronics, Intel, other global semiconductor and advanced-packaging companies, and relevant companies in China.

Potential engagement structures include patent licensing, process architecture transfer, and joint process development.

## Intellectual property and transaction options

The technologies, process architectures, figures, and implementation concepts described in this repository are protected, as applicable, by granted patents, pending patent applications, and proprietary know-how of Cools Inc.

Cools is open to structured discussions with qualified strategic partners. Depending on the technology, field, territory, and transaction scope, potential structures may include:

- exclusive or non-exclusive patent licensing;
- field-of-use or territory-limited rights;
- process-architecture transfer and technical support;
- joint development and commercialization;
- strategic investment or transfer of the relevant technology business; and
- where commercially appropriate, assignment or transfer of the relevant patents, patent applications, and associated rights themselves.

**Negotiations are not limited to a licence. Where the transaction purpose and conditions are appropriate, the relevant patent portfolio itself may be included in the transaction.**

Any transaction is subject to technical and legal due diligence and a definitive written agreement.

## Public technical briefs

- [Rubin Ultra 4-die LATC technical note](briefs/Rubin_Ultra_4Die_LATC_EN.md)
- [Korean public position brief](briefs/Cools_LATC_Public_Position_Brief_KR.docx)
- [English public position brief](briefs/Cools_LATC_Public_Position_Brief_EN.docx)
- [Chinese technical summary](briefs/Cools_LATC_Public_Position_Summary_ZH.md)

## Figures

- [Rubin Ultra 4-die LATC process route](assets/Rubin_Ultra_4Die_LATC_process_route.svg)
- [Monolithic-lid concept](assets/LATC_monolithic_lid_concept_KR.png)
- [Three-step press figure](assets/LATC_three_step_press_figure_KR.png)
- [Conventional process versus LATC](assets/LATC_process_comparison_KR.png)

## Contact

**Dr. Jinhyun Cho — Founder & CEO, Cools Inc.**  
Email: [jhcho@cools.co.kr](mailto:jhcho@cools.co.kr)

For technical review, press enquiries, licensing, patent-inclusive transactions, technology transfer, or joint development, please contact Cools directly by email. Messages may also be left through [GitHub Issues](https://github.com/jhcho9494/Cools_CoWos_No_WarpageSolution/issues).

## Notice

Publication of this repository does not grant any licence, implied right, or permission to practise the disclosed technology. All patent rights, pending application rights, technical materials, figures, and associated commercial rights are reserved by Cools Inc.

© 2026 Cools Inc. All rights reserved.