# SearchHub 🔍

**Free search / fetch / embedding API credits — curated, claimed, and verified by hand.**

Every entry below was actually registered and tested by us: the credit landed, the API answered. No scraped lists, no expired promo codes dressed up as deals. Each entry says what it is, how much is free, whether a card is needed, the exact steps to claim it, and the traps we stepped on.

**搜索 / 抓取 / 嵌入 API 的免费额度合集——每一条都亲手注册、实测到账才收进来。** 写清薅多少、绑不绑卡、领取步骤和实测踩过的坑。

---

## The haul at a glance ｜ 总表

| Provider | What | Free | Card? | Renews |
|---|---|---|---|---|
| [Keenable](#keenable) | Search + page fetch API | **100,000 requests/mo** | No | Monthly (resets on the 21st) |
| [Exa](#exa) | Search API for AI agents | **$10 signup + $10 onboarding + $10/mo** | No | $10 monthly |
| [Tavily](#tavily) | Search API for AI agents | **1,000 credits/mo** | No | Monthly |
| [Tabstack](#tabstack) | Web access API (extract / research) | **10,000 credits** | No | One-time trial |
| [QuanticData](#quanticdata) | SERP + scraping APIs | **$2 credit/mo** | No | Monthly |
| [Voyage AI](#voyage-ai) | Embedding + rerank API | **200M tokens per model** | No | One-time per account |
| [Mixedbread](#mixedbread) | Embedding + rerank + search API | **$5 Starter credit** | No | One-time |

---

## Keenable

**What:** Web search and page-fetch API built for AI agents. One key covers search and fetch.

**Free:** 100,000 search/fetch requests per month on the free tier, resetting on the 21st. Worth about $400/mo at the $4-per-1k overage price.

**How to claim:**
1. Sign up at [https://keenable.ai](https://keenable.ai) with an email address and verify it.
2. Open the console at [https://app.keenable.ai](https://app.keenable.ai) and create an API key.
3. Call `POST https://api.keenable.ai/v1/search` with header `X-API-Key: <key>`.

**Traps (tested 2026-11-21):**
- Disposable / privacy email domains get only **1,000 requests/mo** instead of 100,000. Use a normal mailbox.
- A new key's full value is shown **once**, and only via the copy button — save it immediately or you will have to create another key.
- Rate limit 10 requests/second on the free tier.

**怎么薅：** 官网邮箱注册 → 邮箱验证 → 控制台建 key。注意别用临时邮箱域名注册，额度直接砍到每月 1,000 次；key 只显示一次，建完立刻存好。

---

## Exa

**What:** Search API designed for AI agents and RAG pipelines.

**Free:** $10 for signing up + $10 for finishing onboarding, then $10 free every month. When we claimed (2026-11), the codes `EXA20FREEBUFF` and `EXA20FIRESHIP` added $20 each — codes like these die without notice, test them at claim time, don't trust old posts.

**How to claim:**
1. Sign up at [https://exa.ai](https://exa.ai) — email code login, no password.
2. Finish the onboarding flow to release the second $10.
3. Create a key in the console and check each credit tranche's expiry date there.

**Traps (tested 2026-11-19):**
- Credit tranches expire separately — one of our $10 tranches expired on 2026-12-01 while the rest stayed. Spend the expiring tranche first; the console shows the dates.

**怎么薅：** 邮箱验证码登录注册 → 走完新手引导领第二笔 10 美元 → 控制台建 key。每笔额度有效期不一样，先花快到期的。

---

## Tavily

**What:** Search / extract / crawl API for AI agents.

**Free:** The Researcher plan is free forever: 1,000 credits per month (basic search = 1 credit, advanced search = 2), resetting monthly.

**How to claim:**
1. Sign up at [https://app.tavily.com](https://app.tavily.com) with email + password and verify the email.
2. The free plan is active immediately; create a key on the home page.
3. Call `POST https://api.tavily.com/search` with header `Authorization: Bearer <key>`.

**Traps (tested 2026-11-21):**
- The widely shared codes `GEEKROOM` (expired) and `GEEKROOM2` (fully redeemed) are **dead** — the "8,000 free credits" posts are stale. We verified both in the console; don't waste time on them.

**怎么薅：** 邮箱加密码注册 → 验证邮箱 → 免费档自动生效，首页建 key。网传的 8,000 额度码已实测全废，别试。

---

## Tabstack

**What:** Mozilla's web-access API for agents — Research / Extract / Generate / Automate. Roughly 1,000 Markdown extracts or 40 fast research runs on the free credits.

**Free:** 10,000 credits on signup, shown in the console as "10,000 credits remaining".

**How to claim:**
1. Sign up at [https://tabstack.ai](https://tabstack.ai) with an email address.
2. Click the verification link in the email, then set an organization name and a password.
3. The console at [https://console.tabstack.ai/dashboard](https://console.tabstack.ai/dashboard) shows the balance; create an API key there when you need one.

**Traps (tested 2026-11-22):**
- The console calls it a "free trial" and does **not** print an expiry date for the credits — don't hoard them forever, use them reasonably soon.

**怎么薅：** 邮箱注册 → 点邮件验证链接 → 填组织名和密码 → 控制台到账 10,000 credits。有效期控制台没标注，别囤太久。

---

## QuanticData

**What:** SERP, scraping, crawl and data APIs behind one key, billed per successful result only.

**Free:** $2 of credit every month, no card — about 2,222 plain SERP searches or ~1,300 scraped pages at list price. Failed or blocked calls are never billed.

**How to claim:**
1. Register at [https://app.quanticdata.io/register](https://app.quanticdata.io/register).
2. Create a key at [https://app.quanticdata.io/api-keys](https://app.quanticdata.io/api-keys).
3. Call `https://api.quanticdata.io/v1` with `Authorization: Bearer <key>`.

**Traps:**
- The $2 covers the **Data APIs** only. Residential proxies are a separate product — the separate 100 MB proxy trial asks for SMS verification.

**怎么薅：** 注册 → 建 key → 每月 2 美元自动到账，失败调用不扣费。代理是另一个产品，别混。

---

## Voyage AI

**What:** Embedding and reranking models (MongoDB's Voyage), the retrieval layer for search and RAG.

**Free:** A one-time allowance **per model, per account**: 200M tokens on each current model (voyage-4, voyage-4-large, voyage-4-lite, voyage-context-4, voyage-code-4, rerank-3, …), 50M on the domain models (voyage-finance-2, voyage-law-2, voyage-code-2), plus 200M text tokens and 150B pixels on the multimodal models.

**How to claim:**
1. Create an account at [https://dash.voyageai.com](https://dash.voyageai.com).
2. In the API keys section, create a secret key — the free tokens are spent before any paid usage automatically.

**Traps (tested 2026-11-21):**
- Free tokens do **not** apply to Batch API usage.
- The free tier's rate limits are low (we measured tier 0 at 3 RPM / 10k TPM) — fine for testing, not for bulk jobs.
- Free-tier content may be used for training unless you opt out.

**怎么薅：** 注册 → 建 key → 每个模型 2 亿 token 自动抵扣。一次性额度不是每月刷新；Batch API 不吃免费额度。

---

## Mixedbread

**What:** Embeddings, reranking and search APIs (mxbai models, Toast 1).

**Free:** $5 one-time Starter credit, no card required. It does not renew and its expiry is not published.

**How to claim:**
1. Sign up at [https://www.mixedbread.com](https://www.mixedbread.com) (we used GitHub login).
2. Create an API key in the platform console.
3. Call `https://api.mixedbread.com/v1` with `Authorization: Bearer <key>`.

**Traps (tested 2026-11-22):**
- One-time $5 only — our balance showed $4.98 after the first test calls.
- In the vendor's own words, data collected under the free tier is retained indefinitely.

**怎么薅：** 注册 → 建 key → 5 美元一次性额度，不续、有效期未公布，小额试用装。

---

## Rules of this list ｜ 本清单的规矩

- **Tested, not copied.** Every entry was registered by us and the credit was seen in the console before it was listed. Verification dates are in each section. （每条都亲手注册、控制台见到账才收录。）
- **Dead deals get marked, not deleted.** When a code or offer dies, we say so in the entry — stale "free credits" posts are how people waste evenings. （失效的会标注失效，不删，省得后来人再踩。）
- **No accounts, no keys, no referral tricks.** This repo shares sources and steps only. （只放来源和步骤，不放任何账号与钥匙。）

Last verified: 2026-11-22.
