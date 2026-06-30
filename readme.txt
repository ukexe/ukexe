<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&height=230&color=0:0f172a,50:1e40af,100:0f766e&text=Udhaya%20Kumar%20A&fontColor=ffffff&fontSize=42&fontAlignY=35&desc=AI%20Infrastructure%20%7C%20LLM%20Systems%20%7C%20Inference%20Engineering&descSize=16&descAlignY=55&animation=fadeIn" alt="Udhaya Kumar A - AI Infrastructure, LLM Systems, Inference Engineering" />

<a href="https://git.io/typing-svg">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=20&pause=1200&color=38BDF8&center=true&vCenter=true&width=900&lines=Building+measurable+AI+infrastructure;LLM+serving+%7C+inference+%7C+observability;GPU-aware+systems+with+production+discipline" alt="Typing animation describing Udhaya's engineering focus" />
</a>

<p>
  <a href="https://github.com/ukexe">
    <img src="https://img.shields.io/badge/GitHub-ukexe-0f172a?style=for-the-badge&logo=github&logoColor=white" alt="GitHub profile" />
  </a>
  <a href="https://www.linkedin.com/in/udhaya-kumar-a-exe/">
    <img src="https://img.shields.io/badge/LinkedIn-Udhaya%20Kumar%20A-0a66c2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn profile" />
  </a>
  <a href="https://github.com/ukexe?tab=repositories">
    <img src="https://img.shields.io/badge/Explore-Repositories-0f766e?style=for-the-badge&logo=github&logoColor=white" alt="Explore repositories" />
  </a>
</p>

</div>

---

## Engineering Profile

I am building toward AI Infrastructure Engineering: LLM serving platforms, inference benchmarking, GPU-aware observability, and cost/performance systems for production AI. My recent work focuses on making model serving measurable, reliable, and economically understandable.

> Current direction: LLM systems, inference optimization, GPU telemetry, platform APIs, and applied AI workflows that can be explained, tested, and operated.

## Technical Focus

<div align="center">

[![Core Stack](https://skillicons.dev/icons?i=py,fastapi,pytorch,tensorflow,postgres,docker,kubernetes,prometheus,grafana,git,githubactions,ts,react,nextjs,supabase&theme=dark&perline=8)](https://skillicons.dev)

</div>

**AI systems:** LLM inference, benchmark harnesses, prompt/runtime evaluation, quantization awareness, model-serving APIs.  
**AI infrastructure:** Python, FastAPI, Pydantic, async services, API gateways, testing, structured logging.  
**Systems platform:** Docker, Kubernetes, KEDA, Prometheus, Grafana, GPU scheduling concepts, CI workflows.  
**Data and optimization:** NumPy, Pandas, SciPy, scikit-learn, Qiskit, MLflow, experiment tracking.  
**Frontend for systems tools:** TypeScript, React, Next.js, dashboards, operational UI, data visualization.

## Featured Systems

<div align="center">
  <a href="https://github.com/ukexe/trt-llm-triton-benchmark-suite">
    <img width="420" src="https://raw.githubusercontent.com/ukexe/ukexe/main/triton-llm-card.svg?sanitize=true" alt="Animated 3D card for the Triton and TensorRT-LLM benchmark suite" />
  </a>
  <a href="https://github.com/ukexe/Aegis-LLM-Infra-Kubernetes-vLLM-GPU-Inference-Platform">
    <img width="420" src="https://raw.githubusercontent.com/ukexe/ukexe/main/aegis-llm-card.svg?sanitize=true" alt="Animated 3D card for the Aegis LLM inference platform" />
  </a>
  <a href="https://github.com/ukexe/Quantum-Enhanced-Portfolio-Optimizer-QEPO-">
    <img width="420" src="https://raw.githubusercontent.com/ukexe/ukexe/main/qepo-card.svg?sanitize=true" alt="Animated 3D card for the Quantum-Enhanced Portfolio Optimizer" />
  </a>
  <a href="https://github.com/ukexe/APGMSS">
    <img width="420" src="https://raw.githubusercontent.com/ukexe/ukexe/main/apgmss-card.svg?sanitize=true" alt="Animated 3D card for the AI-powered grievance management system" />
  </a>
</div>

### Triton + TensorRT-LLM Benchmark Suite

A reproducible benchmark harness for comparing LLM serving runtimes across latency, throughput, and cost.

- **Problem:** tokens/sec alone hides tail latency, batching behavior, and infrastructure cost.
- **Architecture:** config-driven Python runner, runtime adapters, metrics aggregation, Prometheus export, Docker/Kubernetes templates, and GPU pricing models.
- **Technical interest:** p50/p95/p99 latency, TTFT, inter-token latency, closed-loop concurrency, quantization paths, and cost per million tokens.

### Aegis LLM Inference Platform

A production-style Kubernetes platform for serving LLMs through an OpenAI-compatible API backed by vLLM workers on GPU nodes.

- **Problem:** LLM inference is latency-sensitive, GPU-constrained, and difficult to operate without request-level and GPU-level visibility.
- **Architecture:** FastAPI gateway, mock/vLLM inference runtimes, GPU-aware Kubernetes manifests, HPA/KEDA autoscaling, Prometheus metrics, Grafana dashboards, and a Next.js ops dashboard.
- **Technical interest:** queue-depth autoscaling, streaming completions, gateway/inference separation, SLO-oriented dashboards, and honest implementation status.

<details>
<summary><strong>More selected work</strong></summary>

### Quantum-Enhanced Portfolio Optimizer

An experimental portfolio optimization platform combining quantum algorithms with classical optimization baselines and a modern web interface.

- **Problem:** portfolio optimization needs explainable comparison between classical baselines and experimental quantum approaches.
- **Architecture:** Python optimization engine, QAOA experiments, classical mean-variance baselines, MLflow tracking, and a Next.js job interface.
- **Technical interest:** algorithmic experimentation paired with tracking, backtesting, and UI workflows instead of a notebook-only prototype.

### AI-Powered Grievance Management System

A multilingual grievance workflow system for submitting, classifying, tracking, and managing public complaints.

- **Problem:** grievance systems need structured workflows, document intake, language support, and status visibility.
- **Architecture:** Next.js application with Supabase-backed authentication, real-time updates, role-based access, OCR-assisted file processing, and admin workflow screens.
- **Technical interest:** combines AI-assisted classification, multilingual document handling, real-time state changes, and database access control.

</details>

## Systems Thinking

```mermaid
flowchart LR
    A["AI Workload"] --> B["Serving Runtime"]
    B --> C["API Gateway"]
    C --> D["Observability"]
    D --> E["Benchmark + Cost Model"]
    E --> F["Engineering Decision"]

    B --> B1["vLLM / Triton / TGI"]
    C --> C1["FastAPI / OpenAI-compatible API"]
    D --> D1["Prometheus / Grafana / GPU metrics"]
    E --> E1["p95 latency / TTFT / cost per 1M tokens"]
```

I like systems where engineering decisions can be traced back to measurements: latency, error rate, throughput, resource utilization, and cost.

## GitHub Signals

<div align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=ukexe&show_icons=true&theme=transparent&hide_border=true&rank_icon=github&title_color=38BDF8&text_color=94A3B8&icon_color=0F766E" alt="GitHub stats for ukexe" />
  <img height="165" src="https://streak-stats.demolab.com?user=ukexe&theme=transparent&hide_border=true&ring=38BDF8&fire=0F766E&currStreakLabel=38BDF8&sideLabels=94A3B8&dates=64748B" alt="GitHub streak stats for ukexe" />
</div>

<div align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=ukexe&theme=react-dark&hide_border=true&bg_color=0D1117&color=38BDF8&line=0F766E&point=FFFFFF&area=true&area_color=1E40AF" alt="GitHub contribution activity graph for ukexe" />
</div>

<details>
<summary><strong>GitHub achievement snapshot</strong></summary>

<div align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=ukexe&theme=algolia&row=1&column=6&no-frame=true&no-bg=true&margin-w=12" alt="GitHub profile trophies for ukexe" />
</div>

</details>

## Engineering Principles

- Measure before optimizing. Good systems expose latency, error, throughput, and cost signals.
- Make architecture inspectable. A README, diagram, test, or dashboard should reduce ambiguity for the next engineer.
- Prefer honest status over inflated claims. Mark what is implemented, scaffolded, experimental, or roadmap.
- Build with operational failure in mind: timeouts, retries, rate limits, metrics, logs, and clear runbooks.

## Contact

I am interested in AI infrastructure, LLM systems, applied ML products, and engineering teams that care about measurable, maintainable systems.

<div align="center">
  <a href="https://www.linkedin.com/in/udhaya-kumar-a-exe/">
    <img src="https://img.shields.io/badge/Connect%20on%20LinkedIn-0a66c2?style=for-the-badge&logo=linkedin&logoColor=white" alt="Connect on LinkedIn" />
  </a>
  <a href="https://github.com/ukexe">
    <img src="https://img.shields.io/badge/View%20GitHub%20Work-0f172a?style=for-the-badge&logo=github&logoColor=white" alt="View GitHub work" />
  </a>
</div>

<img src="https://capsule-render.vercel.app/api?type=waving&height=110&section=footer&color=0:0f766e,50:1e40af,100:0f172a" alt="Profile footer wave" />
