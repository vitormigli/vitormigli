<div align="center">

<img src="assets/banner-v2.svg" width="100%"/>

</div>

I build LLM systems and measure them properly: every project below has a real
evaluation — accuracy, cost, and latency, not vibes — comparing at least two
models or approaches on real numbers. Several run on zero API budget, entirely
on local compute.

<br>

## Featured projects

<table>
<tr>
<td width="50%" valign="top">

**[📄 doc-extraction-pipeline](https://github.com/vitormigli/doc-extraction-pipeline)**
<br>Structured JSON extraction from Brazilian documents (Claude vision + Pydantic), with retry-on-validation-failure.
<br><img src="https://img.shields.io/badge/field_accuracy-99.5%25-2ea44f?style=flat-square"/> <img src="https://img.shields.io/badge/Haiku_4.5-2.2x_cheaper-b8860b?style=flat-square"/>

</td>
<td width="50%" valign="top">

**[⚖️ llm-benchmark-ptbr](https://github.com/vitormigli/llm-benchmark-ptbr)**
<br>Reproducible benchmark of Claude model tiers on 3 real pt-BR tasks, cached so it reruns at zero cost.
<br><img src="https://img.shields.io/badge/intent_accuracy-100%25-2ea44f?style=flat-square"/> <img src="https://img.shields.io/badge/Haiku_4.5-2.9x_cheaper_than_Opus-b8860b?style=flat-square"/>

</td>
</tr>
<tr>
<td width="50%" valign="top">

**[🔍 hybrid-search-ptbr](https://github.com/vitormigli/hybrid-search-ptbr)**
<br>BM25 + dense embeddings + RRF fusion over Portuguese documents. 100% local, zero API cost.
<br><img src="https://img.shields.io/badge/recall%405-100%25-2ea44f?style=flat-square"/> <img src="https://img.shields.io/badge/inference-100%25_local-2ea44f?style=flat-square"/>

</td>
<td width="50%" valign="top">

**[🤖 sales-agent-evals](https://github.com/vitormigli/sales-agent-evals)**
<br>Tool-using sales + internal ops agents, evaluated with simulated customer conversations, not single-turn prompts.
<br><img src="https://img.shields.io/badge/task_completion-87.5%25-2ea44f?style=flat-square"/> <img src="https://img.shields.io/badge/guardrail_violations-0-2ea44f?style=flat-square"/>

</td>
</tr>
<tr>
<td width="50%" valign="top">

**[🔒 pii-redaction-ptbr](https://github.com/vitormigli/pii-redaction-ptbr)**
<br>Detects and redacts CPF, CNPJ, e-mail, phone, and names in pt-BR text before it reaches a log or an LLM prompt.
<br><img src="https://img.shields.io/badge/F1_score-91.7%25-2ea44f?style=flat-square"/> <img src="https://img.shields.io/badge/inference-100%25_local-2ea44f?style=flat-square"/>

</td>
<td width="50%" valign="top">

**[🧾 invoice-ocr-automation](https://github.com/vitormigli/invoice-ocr-automation)**
<br>PaddleOCR + rule-based extraction automating invoice intake: auto-approve or route to human review.
<br><img src="https://img.shields.io/badge/routing_accuracy-100%25-2ea44f?style=flat-square"/> <img src="https://img.shields.io/badge/inference-100%25_local-2ea44f?style=flat-square"/>

</td>
</tr>
<tr>
<td colspan="2" valign="top">

**[⚠️ rag-normas-regulamentadoras](https://github.com/vitormigli/rag-normas-regulamentadoras)**
<br>RAG over real Brazilian workplace-safety regulations (5 gov.br PDFs), hybrid retrieval on a real Postgres + pgvector database (Supabase), citing the exact item or refusing to answer when the context doesn't cover it.
<br><img src="https://img.shields.io/badge/refusal_accuracy-81.2%25-2ea44f?style=flat-square"/> <img src="https://img.shields.io/badge/citation_accuracy-75%25-2ea44f?style=flat-square"/> <img src="https://img.shields.io/badge/Postgres-pgvector-b8860b?style=flat-square"/>

</td>
</tr>
<tr>
<td colspan="2" valign="top">

**[🧪 promptcheck](https://github.com/vitormigli/promptcheck)**
<br>Cassette-based regression testing for LLM prompts — record a real response once, replay it for free forever in CI. YAML test suites, an assertion library, and baseline-vs-current regression detection.
<br><img src="https://img.shields.io/badge/CI_API_cost-%240.00-2ea44f?style=flat-square"/> <img src="https://img.shields.io/badge/tests-35_offline-2ea44f?style=flat-square"/> <img src="https://img.shields.io/badge/regressions_caught-1%2F1-b8860b?style=flat-square"/>

</td>
</tr>
<tr>
<td colspan="2" valign="top">

**[🛠️ n8n-sales-agent](https://github.com/vitormigli/n8n-sales-agent)**
<br>WhatsApp sales agent built entirely in n8n's canvas — RAG over a store's knowledge base (Supabase pgvector), lead capture, human escalation, per-conversation memory. Tested with promptcheck, which caught a real prompt bug before it shipped.
<br><img src="https://img.shields.io/badge/prompt_tests-6%2F6_passing-2ea44f?style=flat-square"/> <img src="https://img.shields.io/badge/regressions_caught-1%2F1-b8860b?style=flat-square"/> <img src="https://img.shields.io/badge/n8n-self--hosted-EA4B71?style=flat-square"/>

</td>
</tr>
<tr>
<td colspan="2" valign="top">

**[🚗 cv-traffic-counter](https://github.com/vitormigli/cv-traffic-counter)**
<br>YOLOv8 + ByteTrack over OpenCV — detects people/vehicles from any video source (file, webcam, RTSP), counts line crossings by direction, fires zone-entry alerts. Found and root-caused a real tracker ID-fragmentation bug mid-project (one crossing counted 3x); fixed at the tracker config, not papered over in the counting logic.
<br><img src="https://img.shields.io/badge/eval-3%2F3_checks_passing-2ea44f?style=flat-square"/> <img src="https://img.shields.io/badge/duplicate_events-cut_50%25-b8860b?style=flat-square"/> <img src="https://img.shields.io/badge/inference-100%25_local-2ea44f?style=flat-square"/>

</td>
</tr>
</table>

<div align="center">

Every repo ships a one-command demo (`docker compose up`), a CI pipeline, and an
honest README — including where the numbers surprised me and what I'd fix next.
Start with **[ai-project-template](https://github.com/vitormigli/ai-project-template)**
to see the shape every project above follows.

</div>

<br>

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=vitormigli&show_icons=true&theme=gruvbox&hide_border=true&count_private=true&hide_title=true" height="165"/>
<img src="https://streak-stats.demolab.com?user=vitormigli&theme=gruvbox&hide_border=true" height="165"/>

</div>

<div align="center">

**Stack**

<img src="https://skillicons.dev/icons?i=python,ts,nextjs,postgres,docker,supabase&theme=dark" />

</div>

<br>

<div align="center">

[![LinkedIn](https://img.shields.io/badge/-vitor--migliorini-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/vitor-migliorini)
[![Email](https://img.shields.io/badge/-vitormigli.vm%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:vitormigli.vm@gmail.com)

</div>
