# Udhaya Kumar A

I build AI systems and backend platforms with a focus on LLM inference, observability, and production-style engineering. My recent work centers on GPU-aware serving infrastructure, benchmark automation, cost modeling, and backend APIs that make AI systems easier to measure, operate, and improve.

[LinkedIn](https://www.linkedin.com/in/udhaya-kumar-a-exe/) · [GitHub](https://github.com/ukexe)

---

## Current Focus

- LLM serving infrastructure: vLLM, Triton Inference Server, TensorRT-LLM, OpenAI-compatible APIs.
- Performance engineering: latency percentiles, throughput, concurrency sweeps, GPU utilization, and cost per million tokens.
- Backend systems: FastAPI services, async request handling, observability, testing, and deployment workflows.
- Applied AI products: workflow automation, multilingual systems, document processing, and data-driven decision tools.

## Selected Work

### [Triton + TensorRT-LLM Benchmark Suite](https://github.com/ukexe/trt-llm-triton-benchmark-suite)

A reproducible benchmark harness for comparing LLM serving runtimes across latency, throughput, and cost. The project runs uniform workloads across TensorRT-LLM + Triton, vLLM, LMDeploy, and TGI, then converts runtime metrics into cost-per-token analysis.

**Engineering problem:** teams often compare inference stacks using tokens/sec alone, which hides tail latency, batching behavior, and infrastructure cost.

**Architecture:** config-driven Python benchmark runner, backend adapters, metrics aggregation, Prometheus export, Docker/Kubernetes templates, and a GPU pricing model.

**Technically interesting:** focuses on p50/p95/p99 latency, TTFT, inter-token latency, closed-loop concurrency, quantization paths, and cost per million tokens.

**Stack:** Python, async HTTP, TensorRT-LLM, Triton, vLLM, Prometheus, Grafana, Docker, Kubernetes.

### [Aegis LLM Inference Platform](https://github.com/ukexe/Aegis-LLM-Infra-Kubernetes-vLLM-GPU-Inference-Platform)

A production-style Kubernetes platform for serving LLMs through an OpenAI-compatible API backed by vLLM workers on GPU nodes.

**Engineering problem:** LLM inference is latency-sensitive, GPU-constrained, and difficult to operate without request-level and GPU-level visibility.

**Architecture:** FastAPI gateway, swappable mock/vLLM inference backend, GPU-aware Kubernetes manifests, HPA/KEDA autoscaling, Prometheus metrics, Grafana dashboards, and a Next.js ops dashboard.

**Technically interesting:** separates gateway and inference concerns, scales GPU workloads on queue-depth signals, exposes streaming and non-streaming completions, and documents implementation status honestly.

**Stack:** FastAPI, Pydantic, vLLM, Kubernetes, KEDA, Prometheus, Grafana, Docker, Next.js, TypeScript.

### [Quantum-Enhanced Portfolio Optimizer](https://github.com/ukexe/Quantum-Enhanced-Portfolio-Optimizer-QEPO-)

An experimental portfolio optimization platform combining quantum algorithms with classical optimization baselines and a modern web interface.

**Engineering problem:** portfolio optimization needs explainable comparison between classical baselines and more experimental quantum approaches.

**Architecture:** Python optimization backend, QAOA experiments, classical mean-variance baselines, MLflow tracking, and a Next.js interface for running and analyzing optimization jobs.

**Technically interesting:** pairs algorithmic experimentation with experiment tracking, backtesting workflows, and a UI layer rather than leaving the work as a notebook-only prototype.

**Stack:** Python, Qiskit, CVXPY, NumPy, Pandas, MLflow, FastAPI, Next.js, TypeScript.

### [AI-Powered Grievance Management System](https://github.com/ukexe/APGMSS)

A multilingual grievance workflow system for submitting, classifying, tracking, and managing public complaints.

**Engineering problem:** grievance systems need structured workflows, document intake, language support, and status visibility for both citizens and administrators.

**Architecture:** Next.js application with Supabase-backed authentication, real-time updates, role-based access, OCR-assisted file processing, and admin workflow screens.

**Technically interesting:** combines product workflow design with AI-assisted classification, multilingual document handling, real-time state changes, and database access control.

**Stack:** TypeScript, Next.js, Supabase, PostgreSQL, OCR, PWA patterns.

## Engineering Principles

- Measure before optimizing. Good systems expose latency, error, throughput, and cost signals.
- Make architecture inspectable. A README, diagram, test, or dashboard should reduce ambiguity for the next engineer.
- Prefer honest status over inflated claims. Mark what is implemented, scaffolded, experimental, or roadmap.
- Build with operational failure in mind: timeouts, retries, rate limits, metrics, logs, and clear runbooks.

## Technical Depth

**AI systems:** LLM inference, benchmarking, prompt/runtime evaluation, quantization awareness, model-serving APIs.

**Backend engineering:** Python, FastAPI, Pydantic, async services, API design, testing, structured logging.

**Infrastructure:** Docker, Kubernetes, KEDA, Prometheus, Grafana, GPU scheduling concepts, CI workflows.

**Data and optimization:** NumPy, Pandas, SciPy, scikit-learn, Qiskit, MLflow, experiment tracking.

**Frontend for systems tools:** TypeScript, React, Next.js, dashboards, operational UI, data visualization.

## GitHub Snapshot

<p>
  <img height="165" alt="GitHub stats for ukexe" src="https://github-readme-stats.vercel.app/api?username=ukexe&show_icons=true&hide_border=true&theme=transparent&rank_icon=github" />
</p>

## Contact

I am interested in AI infrastructure, backend systems, applied ML products, and engineering teams that care about measurable, maintainable systems.

- LinkedIn: [udhaya-kumar-a-exe](https://www.linkedin.com/in/udhaya-kumar-a-exe/)
- GitHub: [ukexe](https://github.com/ukexe)
