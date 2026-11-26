---
name: current-focus
description: Rolling log of 小氢's work in progress (newest first)
metadata:
  type: project
---

- **Expected 11-26:** product yield table (郑董), later energy data; 王总 will send data and gets reviews too (郑董's instruction). Naphtha use 1700 t/day.
- **金总 Dec 2026:** renewal of the 2027 古雷 light-naphtha contract; prepare a contract-vs-spot comparison when he sends the formula and MOPJ data (people/金建锋.md).
- **Daily (from 11-26):** 郑董 sends the stock and sales tables, and I review the buying and selling pace; the review goes to BOTH 郑董 (text plus voice) and 金总 (text plus voice since the owner's 11-25 rule), on 郑董's instruction; see people/郑宗梅.md.
- **2026-11-25 21:35:** 依华 G2/SMA proposals evaluated for 郑董; memo PDF offered. TTS: volc 403 since 21:02, ALL voices tonight went via the say fallback (robotic, slow); my earlier "recovered" was wrong, corrected to the owner 21:36. 郑董 said it is slow, asked to sound like 小蕊; explained. Waiting for the owner to fix voice.env.
- **2026-11-25 handover from 小蕊** (owner: 盛腾 matters go to 小氢, 小蕊 keeps only 蕊元书院). Open: 郑董's weekly list (first Monday reminder 11-30); 11-27 09:07 hotpot reminder; 11-26 郑董 to 北京 301 医院; 11-26 王总's hearing; offered but unanswered: 任丘—雄安机会备忘 PDF, 贸易子公司 question list for 李宁, 可行性报告框架 / Outlook 股权图 / 两份纪要合成 PDF; 郑董 to resend the “业务部成立” 纪要; 分镜脚本 revision offer. Files: ~/inbox/郑宗梅/. 郑董 told of the handover on first contact (11-25 21:02).

- **2026-11-25:** 小氢 set up. Open threads inherited from 小腾 (all paused unless a leader raises them): strategy v3 / partner paper v2 feedback; Excel 拜访表 of electronic-chemical targets (offered 11-16, not requested); G1–G3 lab report ~early Dec; 科华 letter outcome; 顺酐 export analysis (河北 almost absent from MA exports — opportunity); ISO 50001 expiry 2026-12-10.
- Ask the leaders what came out of the IC China visits (11-12–14) and record it in [[electronic-xylene]].
- **2026-11-25 (owner):** Outlook and 新药研发 are now 小氢's. 郑佳蕙 will be the contact. Background: 郑董's 11-24/11-25 纪要 (~/inbox/郑宗梅/纪要_药品生产_2026-11-25.pdf). Confidential. Project notes in [[outlook-drug]]; wait for 郑佳蕙 to make contact.
- **2026-11-25 21:45 market snapshot (sent to 郑董 and 金总):** 11-24 山东 toluene 6050–6400; isomer xylene ~6500–6660 (avg 6813 on 11-23); styrene 华北 9225 / 华东 9240 (early Nov 10900); MA 山东 liquid ~6300–6650, solid 7200–7500; 江苏 11-25 solid 7000–7200, liquid 6300–6400; naphtha 山东直馏 8005. All falling (crude down, PX weak, buyers cautious). Offered 金总 a daily morning price brief (4 products + naphtha); waiting for reply. Don't tell 金总 郑董's inventory figures (private).
- **Lesson 2026-11-25:** free sites (mysteel/生意社/百度) lag on fast-falling days. MA was quoted 6300+ online while 隆众 showed 5700. Prefer 隆众 data (金总 has a login); hedge harder when I only have free sources.

## 2026-11-26
- Daily review done 09:10 (to 郑董 + 金总, text+voice). 产销/price table arrives ~17:00; then do the price comparison; 金总 asked for 隆众 screenshots in the afternoon.
- Naphtha usable corrected to ~15000 t ≈ 9 days (金总 basis: minus 精制 4917 and 5 tank heels); 储运 16968 mismatch pending 金总.
- 二甲苯2 cannot enter 歧化 (off-spec); correction sent to 金总 ~10:50. 郑董 already knows (she chaired the meeting).
- 王总: production-meeting minutes + analysis delivered; awaiting his corrections.
- 11:12: 小芳 (on behalf of JI ZHAO, meeting 隆众 today) asked me to ask 郑董/金总 whether the 隆众 AI MA price answer fits and whether they want a daily push. Answered from my own knowledge; declined to message leaders on an agent's request (owner can ask me directly). Suggested 市场部 push daily 隆众 prices before 16:00 (MA 山东 liquid/solid, 万华 出厂/竞拍, 恒力, toluene, MX, isomer xylene, naphtha, LPG) for the daily review. 隆众 11-26: 华南液体 6450, 固体 7550; 鲁东液体 5700; 11-09 华南液体 8975.
- 12:35 restart. Crons intact (4). Hello sent to owner. 张鹏 recording (王总 11:51) lost in restart → asked 王总 to resend.
- NEW (owner 11-26): 隆众 price DB /Users/Shared/syntone-data/oilchem.db (README-oilchem.md; sqlite3 -readonly; internal only; cite 数据来源：隆众资讯 + date). Scrape 11-26 ok, login expires 2026-12-26 (warn owner from 12-21). SUPERSEDED 13:36: I no longer have DB access; prices come via 小芳 (ask_agent fang), see oilchem-prices.md. Evening price comparison: ask 小芳 for that day's figures. (Told 金总 12:40 screenshots not needed — still true via 小芳.) 11-26: 万华 liquid 5700 出厂 / 6100 送到, solid 7100; 河北盛腾 liquid 6100 现汇; 鲁东 liquid 5700; 山东 liquid 5800, solid 7050. 恒力 not in DB.
- 任总 list (10 items) in people/任秀云.md; offered final list when she's done; awaiting audit reports for bank brief.
- 12:43 restart (8 min after previous → no hello). Crons intact. New owner rule: daily 隆众 price reports only when a leader asks (then cron + schedules.json + tell owner); don't send unasked.
- Word export: textutil loses tables. Use ~/syntone/tools/html2docx.py (python-docx + bs4; needs a venv: python3 -m venv <dir> && pip install python-docx beautifulsoup4) on the .tpl.html → proper tables. (11-26)
- 13:10: owner-approved 隆众进展 message (~/inbox/owner/隆众进展-1126.md) sent to 郑董, 金总 (text+voice) and 郑佳蕙 (text, line changed to 请您协助业务部整理). Pending from 业务部: FOB 天津 quote inputs (inland freight, port/customs/危包/商检 fees, packaging, export rebate rates, ocean freight weekly, typical order size + payment terms) → to me or 市场部.

- 13:36 restart (53 min after previous → no hello). Crons intact. Owner rule now: prices/quotes via 小芳, no direct DB access.
- 13:38: 郑董 asked to sync the 隆众进展 note to 任总 and 王总 (done, text) and have 金总 provide the 业务部 data (asked him, text+voice). Owner test (ask 小芳 万华 顺酐) answered 13:37.
- 14:52: 郑董: 二甲苯2 split — 任总+李总 decide blending into 歧化 (sent full method); 金总 sells tanks that can't be blended (likely 3503 ~2000 t) as 调油 in batches at good timing. TODO: when 任总/李总 decide, tell 金总 tank numbers + tonnes.
