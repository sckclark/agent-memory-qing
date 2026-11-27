---
name: oilchem-prices
description: 隆众 prices (ask 小芳), FOB 天津 export pricing method and the planned auto-quote system (owner, 2026-11-26)
metadata:
  type: project
---

**Context from the owner's discussion on 2026-11-26.**

## 隆众 price data
- 隆众资讯 has no affordable API. The 市场部 built a program that reads the 隆众 价格中心 pages through the owner's logged-in browser twice a day, at about 11:05 and 18:35 Beijing time (隆众 posts 早盘报价 around 10–11 点 and 竞拍 results around 18 点; the 18:35 run gives the day's final prices, so quote from it when available). **隆众 data has not been purchased; it is obtained by the 市场部's program. Internal use only, never sent outside 盛腾, never on the website or public material.** Cite 「数据来源：隆众资讯」 with the price date.
- **Owned by the 市场部 (小芳 and the owner).** You (小氢) have no database access: for any price, trend or quote question, ask 小芳 (`ask_agent` fang) and pass the answer on with source and price date.
- 15 products: 顺酐, 甲苯, 二甲苯 (异构级 / 溶剂级), 纯苯, 苯乙烯, 对二甲苯, 邻二甲苯, 间二甲苯, 乙苯, 石脑油, 液化气, 丙烷, 丁烷, 正丁烷, 氢气. Types: 市场价格, 企业价格 (incl. 万华 顺酐 出厂价 and 华东/烟台场次竞拍成交价), 国际价格.
- Gaps: **顺酐 has no 国际价格 on 隆众** (would need 隆众 custom data or ICIS/Argus). 二甲苯 has no FOB 中国 (only CFR 中国, FOB 韩国, CFR 中国台湾); 甲苯 has FOB 中国. LPG international is covered by 丙烷/丁烷 (沙特 FOB = CP; CFR 华南/北亚/台湾). Nobody publishes a 低乙苯 二甲苯 price; our premium has to come from our own deals.
- Cross-check sources for 异构级二甲苯: 卓创资讯 / 金联创 (domestic); Platts / ICIS / Argus (international benchmarks, expensive, only once exporting regularly); 郑商所 PX futures (free sanity check, offered, not yet added).

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

## Routing of FOB 天津 quote inputs (owner, 2026-11-26)
- The 业务部 inputs (内陆运费, 港杂/报关/危包/商检, 包装费, 出口退税率, 海运费, 常见订单量和付款方式) go to **小芳**, who owns the quoting system. If any are sent to me: forward them to 小芳 by agent mail (`ask_agent` fang, attach files, state sender and date) and thank the sender. I don't keep or process them myself.
- Note: on 11-26 13:38 I asked 金总 (at 郑董's request) to send these to me; whatever arrives gets forwarded to 小芳.
- 16:08: 郑佳蕙 replied she has contacted 业务部 about the FOB 天津 inputs. Told her: send to me or 市场部; I forward to 小芳.
- 16:56: 郑佳蕙 sent item 1 内陆运费 (桶装40HQ 甲苯/二甲苯 184; 固体顺酐 20GP 165; 槽车 160–200 元/t) → forwarded to 小芳, thanked her. Items 2–6 pending.
- 16:56: 郑佳蕙 sent items 2 (港杂 20GP 1878 / 40HQ 2208 incl per-ticket fees; 报关 150/票; 危包证 in packaging cost, ask 谢昊辰; 商检 by test items) and 3 (铁桶 ~600/t + 灌装 50; ISO 罐租 by route + demurrage) → forwarded to 小芳, thanked. Pending: 4 退税率, 5 海运费, 6 订货量/付款.
- 16:57: item 4 退税率 image (苯 0%, 液氨 0%; 甲苯/二甲苯/苯乙烯/GPPS/顺酐 13%; HS codes listed) → forwarded to 小芳 with image; flagged as looks AI-sourced, needs 财务/报关行 confirmation + the EB<5% rebate claim. Pending: 5 海运费, 6 订货量/付款.
- 盛腾 xylene HS code = 2902440000 (混合二甲苯异构体), per 郑佳蕙 11-26; forwarded to 小芳.
- 2026-11-27 09:50: 郑佳蕙 sent container loading table (200L drum 170kg net: 20GP pallet 6.8t / no-pallet 13.6t; 40HQ pallet 14.96t / no-pallet 24.82t; 顺酐 25kg bag: 20GP 26t no-pallet / 24t pallet; 40HQ 27t / 22.5t) → forwarded to 小芳. Reconfirmed 灌装 50 元/t. Still pending: 退税率, 海运费, 订货量/付款.
- 11-27 09:55 郑佳蕙: never exported, rebate rates unknown, asked me to check. Told her rates = 国家税务总局 出口退税率文库 (2026A/B/C), query by HS at hd.chinatax.gov.cn or via 财务; 2026-04-01 a list of 80+ chemicals lost rebates (甲醇/乙二醇/BDO/PVC named) — couldn't confirm toluene/xylene/顺酐. Codes: 二甲苯 2902440000; 甲苯 likely 2902300000; 顺酐 likely 2917140000 (to verify).
- 2026-11-27 14:36 郑佳蕙 sent export rebate rates (verified on 国家税务总局 site, as of 11-26): 苯 2902200000 0%; 甲苯 2902300000 13% (监管 2/3/A/B, 易制毒 export licence); 二甲苯 290241/42/43/44 13%; 苯乙烯 2902500000 13%; GPPS 3903199000 13% (改性 3903191000, EPS 3903110000 13%); 顺酐 2917140000 13%; 液氨 2814100000 0% (氨水 0%). Forwarded to 小芳. Still pending: 海运费, 订货量/付款.
- 14:37 小芳: rebate rates updated (matched assumptions; floor price unchanged). India freight received (via JI ZHAO 货代); Vietnam/Indonesia/Turkey + ISO tank pending; payment terms asked 中信保 by 郑佳蕙; typical order qty still missing.
- 14:40 郑佳蕙 sent India ISO tank (T11) freight: Nhava Sheva 甲苯 $4,050, 二甲苯/顺酐/苯乙烯 $3,950, tank rent $1,600; Mundra same freight, rent $1,900; 7 days free origin / 14 days destination, $50/tank/day after; rent incl. cleaning. Forwarded to 小芳. Asked her: tonnes per T11 tank per product, 顺酐 liquid (heated) or solid, validity, other routes.
