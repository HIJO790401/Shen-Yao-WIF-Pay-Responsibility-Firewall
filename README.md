# Shen-Yao WIF-Pay Responsibility Firewall

## 沈耀 WIF-Pay 金融責任鏈防火牆

**Shen-Yao WIF-Pay Responsibility Firewall** is a front-end demo for a payment responsibility chain system.  
**沈耀 WIF-Pay 金融責任鏈防火牆** 是一個純前端示範，用來展示付款事件如何被轉換成可追溯、可回放、可定責的責任鏈。

---

## Core Idea｜核心理念

Every payment should carry a traceable, replayable, and accountable responsibility chain.  
每一筆付款，都應該帶有一條可追溯、可回放、可定責的責任鏈。

This demo does not process real payments.  
It does not collect card numbers, CVV, passwords, or personal banking data.  
It only demonstrates how responsibility can be tracked across banks, payment platforms, service providers, and support systems.

本 Demo 不處理真實付款。  
不蒐集卡號、不保存 CVV、不要求密碼、不連接銀行 API。  
它只示範：當付款事件發生後，銀行、付款平台、服務商與客服系統之間的責任鏈，如何被記錄、追蹤、回放與審計。

---

## What It Solves｜它解決什麼問題

When payment disputes happen, responsibility often becomes unclear:

- The bank says: contact the platform.
- The platform says: contact the provider.
- The provider says: wait for support.
- Support replies with automated messages.
- The user is left without a clear accountable node.

當付款爭議發生時，責任常常變得模糊：

- 銀行說：請找付款平台。
- 付款平台說：請找服務商。
- 服務商說：請等客服。
- 客服只回 AI 自動信。
- 最後使用者找不到真正承接責任的節點。

WIF-Pay turns the payment event into a replayable responsibility object.

WIF-Pay 將付款事件轉換成可回放的責任物件。

---

## Demo Features｜Demo 功能

This demo includes three controlled scenarios:

本 Demo 內建三個固定示範情境：

1. **Normal Subscription｜正常訂閱**  
   A normal payment flow with a closed responsibility chain.  
   正常付款流程，責任鏈完整閉環。

2. **Suspicious Gift Subscription｜禮物訂閱疑似盜刷**  
   A payment event where a gift subscription is activated for an unknown recipient.  
   禮物訂閱送往陌生帳號，觸發高風險責任審計。

3. **Liability Shirking Case｜三方互相推責**  
   A dispute case where bank, platform, provider, and support shift responsibility to each other.  
   銀行、平台、服務商與客服彼此推諉，觸發聯合審計。

---

## Responsibility Nodes｜責任節點

The demo tracks four responsibility nodes:

本 Demo 追蹤四個責任節點：

- **BANK｜銀行責任位**  
  Authorization, fraud risk, dispute handling, card lock, chargeback records.  
  授權、風控、爭議款、停卡、退款與後續攔截紀錄。

- **PLATFORM｜付款平台責任位**  
  Order routing, platform transaction ID, device/account checks, refund or retry records.  
  訂單路由、平台交易編號、裝置與帳號檢查、退款與重試紀錄。

- **PROVIDER｜服務商責任位**  
  Subscription activation, gift recipient, service account, billing notices, freeze actions.  
  訂閱開通、禮物接收帳號、服務帳號、付款通知與凍結紀錄。

- **SUPPORT｜客服責任位**  
  Support ticket, auto-reply, human escalation, response delay, post-report handling.  
  客服工單、自動回覆、真人升級、回覆延遲與通報後處理。

---

## Internal Logic｜內部邏輯

The demo uses a simplified front-end version of:

本 Demo 使用簡化版前端計算：

- **WIF Score**  
  Who / What / When / Where / Why / How / Responsibility / Replay / Anchor  
  誰、什麼、何時、何地、為何、如何、責任、回放、審計錨記。

- **SCBKR Score**  
  Subject, Causality, Boundary, Knowledge, Responsibility  
  主體、因果、邊界、依據、責任。

- **Risk Score**  
  Unauthorized payment, unknown recipient, support failure, replay missing, liability shirking.  
  未授權付款、陌生接收帳號、客服失靈、回放缺失、責任推諉。

- **Hash Replay Chain**  
  Each event step generates a hash-like replay record for audit demonstration.  
  每個事件節點都生成示範用 Hash Replay 紀錄，用於展示不可無痕竄改的責任鏈概念。

---

## Privacy and Safety｜隱私與安全

This is a safe front-end simulation.

這是一個安全的純前端示範。

It does not:

- process real payments
- connect to banks
- connect to payment platforms
- collect card numbers
- collect CVV
- collect passwords
- store personal financial data

它不會：

- 處理真實付款
- 連接銀行
- 連接付款平台
- 蒐集卡號
- 蒐集 CVV
- 蒐集密碼
- 保存個人金融資料

---

## Demo URL｜示範網址

GitHub Pages Demo:

https://hijo790401.github.io/Shen-Yao-WIF-Pay-Responsibility-Firewall/

If the page is not live yet, please enable GitHub Pages in repository settings.  
如果頁面尚未啟用，請至 GitHub 倉庫 Settings 啟用 GitHub Pages。

---

## Official Website｜官方網站

Shen-Yao Official Portal:  
沈耀官方入口：

https://hijo790401.github.io/shen-yao-portal/

For full API, PoC collaboration, or technical discussion, please contact through the official website.  
如需完整 API、PoC 合作或技術討論，請透過官方網站聯絡。

---

## Positioning｜產品定位

WIF-Pay is not a payment processor.  
It is not a bank replacement.  
It is not a legal judgment system.

WIF-Pay 不是支付處理器。  
不是銀行替代品。  
也不是法律判決工具。

It is a responsibility replay layer for payment events.  
它是付款事件的責任回放層。

Its purpose is to make payment responsibility traceable across:

它的目的，是讓付款責任能在以下節點之間被追溯：

- banks
- payment platforms
- service providers
- support systems
- user dispute reports

- 銀行
- 付款平台
- 服務商
- 客服系統
- 使用者爭議回報

---

## Creator｜創作者

Created by:

**Wen-Yao Hsu / Shen Yao 888π**  
**許文耀／沈耀888π**

Founder of Semantic Firewall  
語意防火牆創辦人

Taichung, Taiwan  
台灣台中

Official Website:  
https://hijo790401.github.io/shen-yao-portal/

---

## Final Statement｜最終說明

A payment is not a single transaction.  
A payment is a responsibility chain.

付款不是單點交易。  
付款是一條責任鏈。

When something goes wrong, every node should be traceable:

當事件出錯，每個節點都應該可追溯：

Who authorized?  
Who routed?  
Who received?  
Who activated?  
Who notified?  
Who handled support?  
Who failed to escalate?  
Who must provide replay?

誰放行？  
誰路由？  
誰收款？  
誰開通？  
誰通知？  
誰處理客服？  
誰沒有升級？  
誰必須提供回放？

Without WIF-Pay, responsibility can disappear into automated systems.  
With WIF-Pay, the responsibility chain can speak.

沒有 WIF-Pay，責任可能消失在自動化系統裡。  
有 WIF-Pay，責任鏈會自己說話。