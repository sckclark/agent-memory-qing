---
name: syntone-content-rules
description: "Hard content rules for anything published about Syntone — facts, names, contacts, confidential items"
metadata:
  node_type: memory
  type: project
  originSessionId: 9a11e7e4-2ed6-4c11-bb13-06bafd9765a1
  modified: 2026-10-28T16:20:05.018Z
---

- **Never invent facts.** Missing data → visible TODO + question to the departments ([[content-question-workflow]]).
- **Source of truth:** departments' answers in the 官网内容确认单 override the company profile 盛腾科技GEO2.0企业简介 (V1.0, 2026-08) / Syntone_Company_Profile_EN.
- **Contacts:** phone 0317-2976987 (zh pages) / +86 317 2976987 (en pages), email **info@syntone-tech.com** (changed 2026-10-28 from info@syntonechem.com, which must not appear). Never publish the mobile 138 9537 6161 found in the old site's JS bundle.
- **Customers:** only 中国石化, 中国石油, 黎明气体 may be named. No Samsung etc.; the 10-year toluene-blend supply is described as "国际知名电子元器件企业".
- **Toluene blend (甲苯混合液):** composition confidential — no CAS, components or ratio; identified by HS 3824999990; MLCC 专用, standard Q/ST 105 002-2026.
- **Company facts:** 注册资本 10.5 亿元（实收） (企查查 shows 实缴 6.5 亿 — asked the user to check 公示系统); employees 601 = 盛腾 + wholly owned 东方同信 by social-insurance count (R2, 2026-10-30; 453/375 elsewhere are 盛腾 alone); 18 products in 5 categories (异戊烷 added 2026-10-30, under the 80万吨 light-oil unit; 抽余油 not on the site); 8 main units + 完善的辅助设施; founded 2011-04; ISO 50001 issued 2023-12-11 covering only 石油混合二甲苯（含石油醚）、工业用苯乙烯 production; 省级绿色工厂 2024 (工信厅 notice 2024-09-12, entry 37); 先进级智能工厂 2026-05 (gxt.hebei.gov.cn 2026-05-27, entry 277); 沧州市基础级智能工厂 2025 (gxj.cangzhou.gov.cn 2025-12-24, entry 17); 河北省省级节水型企业 2023 (冀工信节〔2023〕261号, entry 93). Honours carry a government-source `url` where one exists.
- **Registry facts (Baidu Baike old entry / licence):** 法定代表人 郑宗尧; 有限责任公司(自然人投资或控股); USCC 91130982572802957J; names 河北盛腾化工 → 盛腾科技有限公司 (2018-09) → 盛腾科技集团有限公司 (2019-02) → 盛腾科技有限公司 (2021-12). Timeline conflict flagged: Baike says 2015-06 project start / 2017-01 phase 1 / 2019-05 styrene; site says 8 units completed 2015.
- **Found but NOT on the site until the company OKs:** 2020 制造业民营企业100强 #83; 光明日报 2022-04-04 (盛腾 hydrogen purification supplied Winter Olympics hydrogen, Zhangjiakou/Yanqing). Unverified: old-Baike rankings for 2018/19/21/23/24 (2024 #96 may be 河北盛卓).
- **Plant location:** Amap/GCJ-02 116.149079, 38.768182 = staff (car) entrance, east side of 北海路; trucks enter from the west. Map chooser offers 高德/百度/腾讯/Google.
- **Images:** company photos only (from 钉钉 knowledge base), EXIF stripped. **PDFs** of certificates go in `public/certificates/`, personal names stripped from metadata.
- **Transport permit (user, 2026-11-11, from the certificate):**
  - Official name: **道路危险货物运输许可证**, 冀交运管许可沧字 130982300021号, held by 河北东方同信化工股份有限公司. Scope: 普通货运, 危险货物运输 (2类1项、第3类). Valid 2024-03-26 to 2028-03-25. Issued by 沧州市行政审批局.
  - EN: Road Transport Permit for Dangerous Goods.
  - Phrasing: "全资子公司东方同信拥有危化品运输车队，持有道路危险货物运输许可证". The fleet is the subsidiary's, not 盛腾's. (2026-11-24, user: the fleet is a 自有采购车队 bringing raw materials in — 原料质量可控、可溯源; customers such as 中国石化/中国石油/黎明气体 collect product themselves, so never say the fleet delivers to them.)
  - Brochures, the digital PDF and the interview doc are updated. Website updated and live 2026-11-11 (commit 8377e22; capabilities shows number, scope, validity; the LAN demo VM is not yet deployed).
- **Star products (user, 2026-11-16):** the products to promote are **异构体二甲苯 (石油混合二甲苯异构体), 顺酐, 甲苯, 苯乙烯** (苯乙烯 added a minute later). Note: the site currently says the "3 种核心出口产品" are 苯, 甲苯, 异构二甲苯 (benzene/toluene/mixed-xylene-isomers pages) — user said "官网改成 4 个" (11-16): product pages now say 4 种核心产品 (commit 3dc4e67, live on HK + mainland, 8/8 checks). Export sections (FAQ export, capabilities export table, About, company.yaml export.main_products) still list 苯/甲苯/异构二甲苯 because 确认单 R6 said 顺酐/聚苯乙烯 are NOT key export products — asked sales to confirm before changing.

**Low ethylbenzene = lead selling point of 混合二甲苯异构体 (user, 2026-11-23):** "乙苯低于5%是和市场上其他混合二甲苯异构体的最大区别", spread on the site and all external brochures. Published spec stays **乙苯≤3%** (确认单 R6); owner confirmed ≤3% on 11-23 (no change). Wording: "低乙苯", no 唯一/最低/naming competitors (ad law); no COA-per-batch promise (still TODO). Done 11-23: site product page + home featured block + FAQ `low-ethylbenzene-xylene` (commit e70343d, both servers), profile PDF page 4 feature band. Next print of any brochure must carry it too.

**Website slogan after the ad-law fix (小芳, 2026-11-25, commit f88e6e2):** "以国内外知名客户验证的质量标准，为全球合作伙伴提供稳定、合规的化工新材料解决方案" (EN "…to quality standards proven by major customers at home and abroad"). The fix removed 世界级/world-class and "leading companies" (now "major companies"). "行业标杆企业" is still waiting for the owner's decision. Use the same wording in any external text.
