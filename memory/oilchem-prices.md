---
name: oilchem-prices
description: 隆众 price database, FOB 天津 export pricing method and the planned auto-quote system (owner, 2026-11-26)
metadata:
  type: project
---

**Context from the owner's discussion on 2026-11-26.**

## 隆众 price data
- 隆众资讯 has no affordable API. The 市场部 built a program that reads the 隆众 价格中心 pages through the owner's logged-in browser every day at about 10:05 Beijing time. **隆众 data has not been purchased; it is obtained by the 市场部's program. Internal use only, never sent outside 盛腾, never on the website or public material.** Cite 「数据来源：隆众资讯」 with the price date.
- Database: `/Users/Shared/syntone-data/oilchem.db` (read-only, `sqlite3 -readonly`). Guide: `/Users/Shared/syntone-data/README-oilchem.md`. Code and daily data backup: GitHub sckclark/syntone-marketing (private), folder `oilchem/` (one subfolder per 市场部 app).
- 15 products: 顺酐, 甲苯, 二甲苯 (异构级 / 溶剂级), 纯苯, 苯乙烯, 对二甲苯, 邻二甲苯, 间二甲苯, 乙苯, 石脑油, 液化气, 丙烷, 丁烷, 正丁烷, 氢气. Types: 市场价格, 企业价格 (incl. 万华 顺酐 出厂价 and 华东/烟台场次竞拍成交价), 国际价格.
- Gaps: **顺酐 has no 国际价格 on 隆众** (would need 隆众 custom data or ICIS/Argus). 二甲苯 has no FOB 中国 (only CFR 中国, FOB 韩国, CFR 中国台湾); 甲苯 has FOB 中国. LPG international is covered by 丙烷/丁烷 (沙特 FOB = CP; CFR 华南/北亚/台湾). Nobody publishes a 低乙苯 二甲苯 price; our premium has to come from our own deals.
- Cross-check sources for 异构级二甲苯: 卓创资讯 / 金联创 (domestic); Platts / ICIS / Argus (international benchmarks, expensive, only once exporting regularly); 郑商所 PX futures (free sanity check, offered, not yet added).
- Login lasts about 30 days (current one until 2026-12-26); the owner rescans. If `scrape_runs` shows a failure or expiring login, tell the owner.

## Leaders
- On 2026-11-26 小氢 sent 郑董, 金总 (text + voice) and 郑佳蕙 the progress note: daily data, ask 小氢 directly, daily push on request, basis for the auto-quote system, and the data list below. **Each leader decides whether and when to get a daily price report; never send unasked.**

## Terms (owner asked; explain this way)
- **FOB X**: price when loaded on a ship at port X (X = loading port); buyer pays freight. FOB 韩国 = Korea's export price, the Asian benchmark.
- **CFR X**: price delivered to port X (X = destination); seller pays freight. 「韩国 CFR」 = 「CFR 韩国」 = import price into Korea. CIF = CFR + insurance. DES = delivered ex ship at destination.
- Under FOB and CFR, risk passes to the buyer when goods are loaded at the departure port. For containers, Incoterms recommend FCA rather than FOB (ask 业务部/货代 which to use in contracts).

## FOB 天津 export pricing (all exports will be quoted FOB 天津)
- **Floor** (below this, selling domestically pays better): (华北内销价 ÷ 1.13 + 内陆运费到天津港 + 港杂/报关/危包/商检 − 出口退税额) ÷ 美元汇率.
- **Ceiling** (above this, buyers take Korean cargo): 目的地 CFR − 天津到目的地运费; where no CFR quote exists, FOB 韩国 + 韩国到目的地运费. Freight is not part of the FOB price, only the competitiveness check; ask the forwarder once a week for the 2–3 main lanes.
- Quote per quantity tier: drums 5–15 t (most expensive per t), ISO tank about 20–24 t (orders of 1/2/5/10 tanks), parcel tanker 1000 t+. Fixed fees ÷ tonnes make small lots dearer. 5 吨起订 today. 二甲苯/甲苯 are Class 3 dangerous goods. Low-EB premium on top.
- **Auto-quote system (planned)** sources the 隆众 DB + PBOC USD mid-rate automatically. **Waiting on 业务部** (via 郑佳蕙 / leaders): 内陆运费到天津港, 天津港杂费/报关/危包证/商检 (per shipment vs per t), 包装费 (桶, ISO 罐), 出口退税率 per product (with 财务), weekly main-lane freight, common order quantities and payment terms.
