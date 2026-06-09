<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:023e8a,100:00b4d8&height=220&section=header&text=ADARSH%20S%20MONI&fontSize=52&fontColor=ffffff&fontAlignY=38&animation=fadeIn&desc=Data%20Engineering%20Lead%20%7C%20Lakehouse%20Architect&descAlignY=58&descColor=90e0ef&descSize=18" width="100%"/>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=15&duration=2500&pause=800&color=00B4D8&center=true&vCenter=true&width=700&lines=📊+2.4B%2B+records+in+the+Lakehouse+%7C+20M+ingested+daily;⚡+1-hour+data+freshness+SLA+across+US+%2B+India;🏗️+PostgreSQL+→+Redshift+→+Apache+Iceberg;🚀+60x+backfill+speedup+%7C+5+days+→+2+hours;🔧+PySpark+%7C+AWS+Glue+%7C+Argo+Workflows+%7C+Iceberg" alt="Typing SVG" />

</div>

<br/>

<div align="center">

<table>
  <tr>
    <td align="center"><img src="https://img.shields.io/badge/Lakehouse_Records-2.4B%2B_&_Growing-00b4d8?style=for-the-badge&logoColor=white"/></td>
    <td align="center"><img src="https://img.shields.io/badge/Daily_Ingestion-20M_rec%2Fday-0077b6?style=for-the-badge&logoColor=white"/></td>
    <td align="center"><img src="https://img.shields.io/badge/Freshness_SLA-1_Hour-023e8a?style=for-the-badge&logoColor=white"/></td>
    <td align="center"><img src="https://img.shields.io/badge/Backfill_Speed-60x_Faster-03045e?style=for-the-badge&logoColor=white"/></td>
  </tr>
  <tr>
    <td align="center"><img src="https://img.shields.io/badge/Cost_Saved-₹28.5L%2Fyr-00b4d8?style=for-the-badge&logoColor=white"/></td>
    <td align="center"><img src="https://img.shields.io/badge/Platform-US+%2B+India-0077b6?style=for-the-badge&logoColor=white"/></td>
    <td align="center"><img src="https://img.shields.io/badge/Experience-7%2B_Years-023e8a?style=for-the-badge&logoColor=white"/></td>
    <td align="center"><img src="https://img.shields.io/badge/Team_Built-0_→_6-03045e?style=for-the-badge&logoColor=white"/></td>
  </tr>
</table>

</div>

<br/>

---

## 🏢 Skit AI &nbsp;·&nbsp; Senior Data Engineer &nbsp;·&nbsp; `Aug 2022 – Present`

> *Series B Voice AI company. De facto Data Engineering Lead — owned full platform strategy, cost governance, and multi-region reliability.*

<br/>

### `V3 Apache Iceberg Lakehouse`

```
  [PostgreSQL · 23 tables]
          │
          ▼  near-real-time CDC
  [AWS DMS] ──────────────────────► [Argo Workflows · Orchestration]
          │
          ▼
  [AWS Glue · PySpark]
          │
          ▼
  [Apache Iceberg on S3 · Medallion]
   Raw → Silver → Gold
   2.4B+ records · 20M/day · US + India
          │
          ▼
  [Athena · Redshift Spectrum · BA Self-Service]
```

- Ingesting **23 production tables** via near-real-time CDC with PySpark and AWS Glue
- **2.4B+ records** — 1.6B+ conversations, 771M campaign leads, 329M calls — and growing
- Reduced worst-case data lag from **24 hours → 1-hour committed SLA** (67% reliability improvement)
- Spark shuffle partition tuning **8 → 200** — per-chunk time: 420s → 21s; 30M-record backfill: 5 days → 2 hours **(60x)**
- Migrated cron orchestration from AWS Glue triggers to **Argo Workflows** — eliminated DPU scheduling costs entirely

<br/>

### `Data Purging & Disaster Recovery Tool`

> *PII compliance tool triggered on client contract termination — anonymizes sensitive data across production systems.*

- Built a **factory-pattern purging engine** — anonymizes PII across 8 tables: `calls`, `conversations`, `call_contexts`, `reported_errors`, `normalized_calls`, `intents`, `campaigns_call`, `campaigns_lead`
- Built a paired **disaster recovery module** — restores original records if purging fails mid-run, ensuring no data loss
- Deployed as a Docker image on **AWS ECR** — triggered via **Argo Workflows** through Integration Proxy
- CI/CD via GitLab — new image generated automatically on every MR merge

<br/>

### `Cost Optimization`

- Led RDS audit — deleted 15+ legacy snapshots; storage **33,814 GB → ~9,000 GB**; monthly cost **$3,317 → $448** (**86% reduction · INR 28.5L/yr saved**)
- Driving Redshift deprecation — aligned E2E, ML, BA stakeholders; targeting **$3K+/month additional savings**
- Delivered **Canada Analytics via PostgreSQL FDW** — cross-database dashboards at a fraction of a full analytics layer cost

<br/>

### `Team & Platform Leadership`

- Built the **Analytics vertical from 0 → 6 contributors**: 4 Business Analysts (US, India, E2E) + 2 Data Engineers
- Defined structured regional ownership, dedicated BI Lead role, and career paths for each contributor
- Championed **Medallion Architecture** with config-driven table flattening — BA self-service analytics without engineering involvement per request
- Designed **multi-tier alerting** (Slack channel alerts + DM escalation) — maintained V2 Redshift stability during V3 rollout with zero disruption to live NLP bots

<br/>

---

## 🏢 IBM &nbsp;·&nbsp; Backend Developer &nbsp;·&nbsp; `Jan 2022 – Aug 2022`

> *Cognitive Process Automation team — financial services automation.*

- Built **REST APIs** for Financial Record-to-Report and Onboarding automation workflows
- Implemented **distributed async task processing with Celery** — decoupled ingestion from processing for scalable financial workflows
- Developed **containerized microservices** (Docker) for scalable financial onboarding pipelines

<br/>

---

## 🏢 Mphasis &nbsp;·&nbsp; Backend Python Developer &nbsp;·&nbsp; `Dec 2019 – Jan 2022`

> *Digital Transformation division — internal tooling and process automation.*

- Built **iPG** (internal project governance microservice) using Python Flask (restx) + MongoDB — automated metric computation and reporting pipelines with APScheduler
- **Recognized by VP of Mphasis** for eliminating manual data aggregation across delivery teams through automated upload-to-metrics workflows
- Earlier: modernized legacy AIG financial applications from Windows Server 2008 to Citrix virtual hosting (AIG W2k8 Remediation)

<br/>

---

## `> stack --production`

<div align="center">

<img src="https://skillicons.dev/icons?i=python,aws,postgres,mongodb,docker,kubernetes,git,linux&theme=dark" />

<br/><br/>

![Apache Spark](https://img.shields.io/badge/Apache_Spark-E25A1C?style=flat-square&logo=apachespark&logoColor=white)
![Apache Iceberg](https://img.shields.io/badge/Apache_Iceberg-3A7BD5?style=flat-square&logoColor=white)
![AWS Glue](https://img.shields.io/badge/AWS_Glue-FF9900?style=flat-square&logo=amazonaws&logoColor=white)
![Argo Workflows](https://img.shields.io/badge/Argo_Workflows-EF7B4D?style=flat-square&logoColor=white)
![Amazon Redshift](https://img.shields.io/badge/Amazon_Redshift-8C4FFF?style=flat-square&logo=amazonredshift&logoColor=white)
![Athena](https://img.shields.io/badge/AWS_Athena-FF9900?style=flat-square&logo=amazonaws&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)
![Celery](https://img.shields.io/badge/Celery-37814A?style=flat-square&logo=celery&logoColor=white)

</div>

<br/>

---

## `> git log --stats`

<div align="center">

<img src="metrics-core.svg" width="100%" />

<br/>

<img src="metrics-calendar.svg" width="100%" />

</div>

<br/>

---

## `> connect --remote`

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-adarshsmoni-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/adarshsmoni)
[![Tech Blog](https://img.shields.io/badge/Tech_Blog-Coming_Soon-00b4d8?style=for-the-badge&logo=hashnode&logoColor=white)](https://github.com/adarshmoni23)
[![Email](https://img.shields.io/badge/Email-adarshsunther@gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:adarshsunther@gmail.com)

<br/>

![Profile Views](https://komarev.com/ghpvc/?username=adarshmoni23&color=00b4d8&style=flat-square&label=PROFILE+VIEWS)

</div>

<br/>

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:00b4d8,50:023e8a,100:0d1117&height=100&section=footer" width="100%"/>
</div>

