<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/pangaea-wordmark-light.svg">
  <img alt="Pangaea Healthcare" src="assets/pangaea-wordmark-dark.svg" width="520">
</picture>

<br/>
<br/>

### *One continent. One standard. One healthcare.*

<br/>

[![Status](https://img.shields.io/badge/STATUS-BUILDING_IN_STEALTH-0B3D91?style=for-the-badge&labelColor=000000)](#)
[![Sector](https://img.shields.io/badge/SECTOR-HEALTHCARE-1F2937?style=for-the-badge&labelColor=000000)](#)
[![Mode](https://img.shields.io/badge/MODE-HEADS_DOWN-111827?style=for-the-badge&labelColor=000000)](#)

<br/>

# The infrastructure of American healthcare

# *is quietly on fire.*

<br/>

<img src="assets/explosion.gif" alt="Detonation" width="420" />

<sub>*[↗ Open the .stl model](assets/explosion.stl) — GitHub renders it as an interactive 3D viewer.*</sub>

<br/>

</div>

---

<div align="center">

## ✦ &nbsp; The system was never designed.

</div>

It accreted. Forty years of acquisitions, regulations, vendor lock‑in, and 3 a.m. patches stacked into something that *technically* moves money and records — until it doesn't. The result is the most expensive healthcare apparatus on earth, and one of the most fragile.

<br/>

<table align="center">
<tr>
<td align="center" width="33%">
<h1>$4.9T</h1>
<sub>U.S. HEALTHCARE SPEND, ANNUALLY<sup><a href="#fn-cms-nhe">[1]</a></sup></sub>
<br/><br/>
≈ <b>17.6% of GDP</b> — more than education, defense, and energy <i>combined</i>.<sup><a href="#fn-cms-share">[2]</a></sup>
</td>
<td align="center" width="34%">
<h1>725M+</h1>
<sub>PATIENT RECORDS BREACHED SINCE 2010<sup><a href="#fn-ocr-portal">[3]</a></sup></sub>
<br/><br/>
A single industry has lost more PHI than the population of the United States — <b>twice</b>.
</td>
<td align="center" width="33%">
<h1>1 in 4</h1>
<sub>DOLLARS SPENT ON ADMIN — NOT CARE<sup><a href="#fn-admin">[4]</a></sup></sub>
<br/><br/>
The largest line item in the world's largest healthcare system is <b>overhead</b>.
</td>
</tr>
</table>

---

<div align="center">

## ✦ &nbsp; The price of fragility

<sub>*Six numbers that should not exist in a functioning supply chain.*</sub>

</div>

<br/>

<table align="center">
<tr>
<td align="center" width="28%">
<h1><code>$9.77M</code></h1>
</td>
<td valign="middle">
<b>Average cost of a healthcare data breach.</b><br/>
Highest of any industry — and has been for <b>14 consecutive years</b>.<sup><a href="#fn-ibm-2024">[5]</a></sup>
</td>
</tr>
<tr>
<td align="center">
<h1><code>$408</code></h1>
</td>
<td valign="middle">
<b>Cost per breached patient record</b> — roughly <b>3× the cross‑industry average</b>.<sup><a href="#fn-ibm-perrec">[6]</a></sup> Each leaked chart is a line item, a lawsuit, and a regulator.
</td>
</tr>
<tr>
<td align="center">
<h1><code>277 days</code></h1>
</td>
<td valign="middle">
<b>Mean time to identify and contain a breach.</b><br/>
Nine months of dwell time inside systems holding the most sensitive data a person owns.<sup><a href="#fn-ibm-mttc">[7]</a></sup>
</td>
</tr>
<tr>
<td align="center">
<h1><code>~190M</code></h1>
</td>
<td valign="middle">
<b>Americans exposed in a single 2024 incident</b> when one upstream clearinghouse went down.<sup><a href="#fn-ch-190m">[8]</a></sup><br/>
<b>Roughly one in two people in the country.</b> One vendor. One blast radius.
</td>
</tr>
<tr>
<td align="center">
<h1><code>$2.87B</code></h1>
</td>
<td valign="middle">
<b>Direct cost of that single outage</b> to its parent company through Q3 2024 — before settlements, before fines, before the next one.<sup><a href="#fn-uhg-cost">[9]</a></sup>
</td>
</tr>
<tr>
<td align="center">
<h1><code>725+</code></h1>
</td>
<td valign="middle">
<b>Major healthcare breaches reported to OCR in 2023 alone.</b><sup><a href="#fn-ocr-2023">[10]</a></sup><br/>
Roughly <b>two new ones every day</b>. The baseline isn't <i>if</i>. It's <i>which Tuesday</i>.
</td>
</tr>
</table>

<br/>

> **The sector spends more defending the perimeter than most countries spend on their militaries —**
> and still loses, on average, *two breaches a day, every day, all year.*

<br/>

<div align="center">

### How a single upstream failure becomes a national one

</div>

```mermaid
%%{init: {'theme':'base','themeVariables':{'primaryColor':'#0B3D91','primaryTextColor':'#fff','primaryBorderColor':'#1F2937','lineColor':'#6B7280','fontFamily':'ui-sans-serif'}}}%%
flowchart LR
    A[🏛️ One upstream<br/>clearinghouse] --> B[💳 Payments halt]
    A --> C[📋 Eligibility checks halt]
    A --> D[💊 Pharmacy claims halt]
    B --> E[🏥 Hospitals]
    C --> E
    D --> F[💊 Pharmacies]
    C --> G[🩺 Clinics]
    E --> H{{🇺🇸 ~190M Americans<br/>affected}}
    F --> H
    G --> H

    classDef root fill:#0B3D91,stroke:#000,stroke-width:2px,color:#fff
    classDef mid fill:#1F2937,stroke:#000,color:#fff
    classDef leaf fill:#111827,stroke:#000,color:#fff
    classDef boom fill:#7F1D1D,stroke:#000,stroke-width:2px,color:#fff
    class A root
    class B,C,D mid
    class E,F,G leaf
    class H boom
```

---

<div align="center">

## ✦ &nbsp; What's actually broken

</div>

<table>
<tr>
<td width="50%" valign="top">

### 🩸 &nbsp; The clinical layer

- Records that don't follow the patient
- Eligibility checked and re‑checked at every door
- Prior authorization queues measured in **weeks**[^pa]
- Care delayed because a *fax* didn't arrive

</td>
<td width="50%" valign="top">

### 💸 &nbsp; The financial layer

- Claims denied for reasons no human can articulate
- 30‑day appeal cycles for 30‑second decisions
- **Tens of billions** written off annually as *uncollectable*[^bad-debt]
- Patients billed twice, providers paid once

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🗝️ &nbsp; The trust layer

- Identity reinvented at every vendor boundary
- Audit logs that don't audit
- "Compliance" as a quarterly performance, not a property
- One outage upstream, one nation downstream

</td>
<td width="50%" valign="top">

### 🛠️ &nbsp; The engineering layer

- Mission‑critical systems on platforms older than the engineers maintaining them
- Integrations measured in **quarters**, not sprints
- Resilience theater dressed up as redundancy
- An entire sector waiting for someone to ship a real platform

</td>
</tr>
</table>

---

<div align="center">

## ✦ &nbsp; Where the money actually goes

</div>

```mermaid
%%{init: {'theme':'base','themeVariables':{'pie1':'#0B3D91','pie2':'#1F2937','pie3':'#374151','pie4':'#6B7280','pieTitleTextSize':'20px','pieSectionTextSize':'16px','pieLegendTextSize':'14px','fontFamily':'ui-sans-serif'}}}%%
pie showData
    "Hospital & physician care" : 51
    "Prescriptions & devices" : 16
    "Other clinical services" : 8
    "Administration & overhead" : 25
```

<div align="center">

<sub>*Approximate share of U.S. national health expenditures.*<sup><a href="#fn-cms-shares">[11]</a></sup></sub>
<br/>
<sub><b>One in every four U.S. healthcare dollars never touches a patient.</b></sub>

</div>

---

<div align="center">

## ✦ &nbsp; Why this still happens

<br/>

> ### The hard parts of healthcare aren't medicine.
> ### They're **identity, policy, isolation, audit, and continuity** —
> ### and the industry has been treating them as *features* for forty years.
>
> ### They were never features. They're ***properties of the substrate.***

</div>

---

<div align="center">

## ✦ &nbsp; Pangaea

</div>

We're a small team of engineers and operators who looked at the supply chain of American healthcare, recognized it for what it is — *a single point of failure with a marketing budget* — and decided that the right response wasn't another vendor.

It was a different kind of foundation.

We don't talk much about what we're building, and we won't here. The work has to speak first.

What we *will* say:

- It is **cloud‑native**, **standards‑first**, and built for **failure as a default condition**.
- It treats security, identity, and tenancy as **load‑bearing properties of the platform** — not optional middleware.
- It is designed to be the layer everyone *else* in healthcare can finally build on top of.

---

<div align="center">

## ✦ &nbsp; Currently

### **Heads down. &nbsp;Shipping. &nbsp;Hiring quietly.**

If you've spent a career being the person who actually had to make healthcare infrastructure *work* — and you're tired of patching the same wound — we'd like to talk.

<br/>

[![Careers](https://img.shields.io/badge/CAREERS-support%40pangaeahealthcare.com-0B3D91?style=for-the-badge&logo=maildotru&logoColor=white&labelColor=000000)](mailto:support@pangaeahealthcare.com)
[![Contact](https://img.shields.io/badge/CONTACT-support%40pangaeahealthcare.com-1F2937?style=for-the-badge&logo=protonmail&logoColor=white&labelColor=000000)](mailto:support@pangaeahealthcare.com)

<br/>
<br/>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/icon-glass.svg">
  <img alt="Pangaea" src="assets/icon-glass.svg" width="72">
</picture>

<br/>
<br/>

<sub>© Pangaea Healthcare &nbsp;·&nbsp; *Continental in scope. Atomic in detail.*</sub>

</div>

---

## Sources

<sub>

<a id="fn-cms-nhe"></a>**[1]** CMS, *National Health Expenditure Accounts — Historical (NHE 2023)*: total U.S. health spending of **$4.9 trillion** in 2023. <https://www.cms.gov/data-research/statistics-trends-and-reports/national-health-expenditure-data/historical>

<a id="fn-cms-share"></a>**[2]** CMS, *NHE Highlights 2023*: health spending accounted for **17.6 % of U.S. GDP**. <https://www.cms.gov/data-research/statistics-trends-and-reports/national-health-expenditure-data/nhe-fact-sheet>

<a id="fn-ocr-portal"></a>**[3]** U.S. Department of Health & Human Services, Office for Civil Rights, *Breach Portal* (cumulative breaches reported under HITECH since 2009; cumulative individuals affected exceeds **725 million**). <https://ocrportal.hhs.gov/ocr/breach/breach_report.jsf>

<a id="fn-admin"></a>**[4]** Himmelstein D.U., Campbell T., Woolhandler S., *Health Care Administrative Costs in the United States and Canada, 2017*, **Annals of Internal Medicine** 172 (2): 134–142 (2020) — U.S. administrative costs estimated at **~25–34 %** of total health spending. <https://www.acpjournals.org/doi/10.7326/M19-2818>

<a id="fn-ibm-2024"></a>**[5]** IBM Security & Ponemon Institute, *Cost of a Data Breach Report 2024*: average healthcare breach cost **USD 9.77 M**, the highest of any sector for the **14th consecutive year**. <https://www.ibm.com/reports/data-breach>

<a id="fn-ibm-perrec"></a>**[6]** IBM, *Cost of a Data Breach Report 2024*: per‑record cost in healthcare materially above the cross‑industry mean of ~$165/record. <https://www.ibm.com/reports/data-breach>

<a id="fn-ibm-mttc"></a>**[7]** IBM, *Cost of a Data Breach Report 2024*: mean time to identify + contain a healthcare breach = **277 days**. <https://www.ibm.com/reports/data-breach>

<a id="fn-ch-190m"></a>**[8]** UnitedHealth Group / Change Healthcare, statement on the February 2024 cyberattack: estimated **~190 million individuals** affected (updated 2025‑01‑24). <https://www.unitedhealthgroup.com/newsroom/2024/2024-02-22-uhg-statement-on-change-healthcare-cyberresponse.html>

<a id="fn-uhg-cost"></a>**[9]** UnitedHealth Group, *Q3 2024 earnings disclosure*: cumulative direct response costs from the Change Healthcare cyberattack reported at **~$2.87 B** (response and business‑disruption costs combined). <https://www.unitedhealthgroup.com/newsroom/posts/2024-10-15-uhg-reports-3q-results.html>

<a id="fn-ocr-2023"></a>**[10]** HHS OCR Breach Portal, calendar year 2023: **725+** reported breaches affecting 500 or more individuals (≈ 2 per day). <https://ocrportal.hhs.gov/ocr/breach/breach_report.jsf>

<a id="fn-cms-shares"></a>**[11]** CMS, *NHE 2023 — distribution of national health spending by type of service*: hospital + professional services ≈ **51 %**, prescription drugs and durable medical equipment ≈ **16 %**, other personal health care ≈ **8 %**, government administration + net cost of insurance + program admin ≈ **~25 %**. Pie‑chart values rounded for visual clarity. <https://www.cms.gov/data-research/statistics-trends-and-reports/national-health-expenditure-data/nhe-fact-sheet>

[^pa]: AMA, *2023 Prior Authorization Physician Survey*: 24 % of physicians report prior authorization led to a serious adverse event for a patient; PA decisions routinely take days to weeks. <https://www.ama-assn.org/system/files/prior-authorization-survey.pdf>

[^bad-debt]: American Hospital Association, *2024 Cost of Caring* report: U.S. hospitals provided **$130 B+** in uncompensated care in 2022; nationwide bad‑debt write‑offs sit in the tens of billions annually. <https://www.aha.org/costsofcaring>

</sub>
