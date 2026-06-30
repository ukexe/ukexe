# AI Positioning And Rendering Research

## Rendering Fix

The custom project cards were not broken because of their animation logic. They were referenced with profile-local paths such as `./triton-llm-card.svg`. On the GitHub profile page, repository-local SVGs can fail or render as alt text because GitHub serves raw SVG files with restrictive content handling unless they are sanitized.

Fix applied:

- Replaced relative image paths with absolute sanitized raw GitHub URLs:
  - `https://raw.githubusercontent.com/ukexe/ukexe/main/triton-llm-card.svg?sanitize=true`
  - `https://raw.githubusercontent.com/ukexe/ukexe/main/aegis-llm-card.svg?sanitize=true`
  - `https://raw.githubusercontent.com/ukexe/ukexe/main/qepo-card.svg?sanitize=true`
  - `https://raw.githubusercontent.com/ukexe/ukexe/main/apgmss-card.svg?sanitize=true`
- Kept the SVG files local to the profile repository so the assets are controlled, versioned, and not dependent on a third-party animation service.
- Kept the animations as embedded SVG/CSS animation, which GitHub supports when SVGs are rendered as images. No JavaScript is used.

Sources:

- GitHub Markup issue on relative SVG rendering and `?sanitize=true`: https://github.com/github/markup/issues/556
- Relative SVG README image behavior and `?sanitize=true`: https://github.com/Haroenv/packages-with-readme-relative-images
- CSS-Tricks on SVGs and animation support in GitHub READMEs: https://css-tricks.com/custom-styles-in-github-readmes/
- Eamonn Cottrell on animated SVGs for GitHub READMEs: https://blog.eamonncottrell.com/animate-svgs-for-github-readmes

## Role Market Research

### Selected Positioning

Chosen target positioning:

**AI Infrastructure Engineer focused on LLM Systems and Inference Engineering**

Why this fits best:

- Your strongest projects are not generic software projects. They are about LLM serving, runtime benchmarking, vLLM/Triton/TensorRT-LLM, GPU-aware Kubernetes, Prometheus/Grafana observability, latency metrics, and cost-per-token modeling.
- Research consistently shows that production AI deployment, inference optimization, GPU infrastructure, and LLM platform work command strong demand and compensation premiums.
- The title is more credible for your current portfolio than Research Scientist or Foundation Model Engineer, which usually require frontier research output, publications, or direct model-training work.
- It avoids broad, generic, or incorrect identities that do not reflect the AI infrastructure focus.

## Role Evaluation

| Role | Typical Compensation Signal | Demand / Outlook | Prestige / Depth | Fit With Current Projects | Verdict |
|---|---:|---|---|---|---|
| AI Infrastructure Engineer | US senior often reaches high six figures in top firms; staff/principal can exceed $500K+ TC | Very strong; scarce GPU/model-serving talent | High systems depth | Excellent: vLLM, Triton, K8s, observability, cost modeling | Best fit |
| LLM Systems Engineer / Inference Engineer | Premium niche; inference specialists often command 30-50% premiums | Very strong as inference costs grow | Very high technical depth | Excellent: benchmark suite and serving platform map directly | Strong supporting subtitle |
| AI Platform Engineer | Strong, especially at AI-native and enterprise AI teams | Strong; companies need internal AI platforms | High applied systems depth | Excellent: platform APIs, metrics, deployment, dashboards | Strong alternative |
| ML Systems Engineer | Senior US TC commonly $220K-$350K; staff at top labs can clear $500K | Strong, especially C++/Rust/inference infrastructure | Very high | Good, but current portfolio is more LLM infrastructure than low-level ML runtime code | Good future target |
| Machine Learning Engineer | Mainstream AI/ML roles often $170K-$245K+; top firms higher | Strong, broad market | Medium-high | Partial: fewer custom model-training artifacts | Too broad |
| LLM Engineer | US TC often cited around $170K-$420K depending level/company | Strong with RAG, evals, serving, agents | High | Good, but can imply application-layer work more than infrastructure | Good but less precise |
| Applied AI Engineer | Senior applied roles often $230K-$350K+ TC | Strong across startups and enterprises | Medium-high | Good for applied product systems, less focused on GPU/inference | Good but broader |
| Generative AI Engineer | Strong short-term demand | Strong but title can be buzzword-heavy | Medium | Partial | Use only as keyword, not core identity |
| Agentic AI Engineer | Emerging and high-demand for agent systems | Growing fast | Emerging prestige | Partial: current projects are more infrastructure than agents | Future expansion area |
| AI Research Engineer | Frontier labs pay very high; research-adjacent engineering is prestigious | Strong but competitive | Very high | Partial: needs more research output or model work | Aspirational, not current best label |
| Research Scientist (AI) | Highest top-lab compensation, often $500K-$1M+ TC | Strong but tiny market | Highest research prestige | Weak current fit without publications/PhD-level research proof | Not current positioning |
| Foundation Model Engineer | Very high at frontier labs | Strong but scarce openings | Very high | Partial: current work serves models rather than trains foundation models | Long-term aspirational |
| AI Software Engineer | Strong general compensation | Broad demand | Medium | Good but too generic | Secondary keyword only |
| AI Architect | High senior/enterprise role | Strong for experienced architects | High | Premature as a primary identity | Future senior title |
| Distributed Systems Engineer | Strong at infrastructure companies | Durable long-term | High systems prestige | Good conceptual fit, but less AI-specific | Supporting skill |
| GPU Systems Engineer | Very high at NVIDIA/frontier labs | Strong as compute demand grows | Very high | Good but current code is not low-level GPU/kernel heavy enough | Future specialization |
| High Performance Computing Engineer | Strong but more specialized | Durable in science/AI/HPC | High | Partial | Useful adjacent keyword |
| Quantum Computing Engineer | Niche, high prestige but smaller market | Growing but less broad than AI infra | High | Partial through QEPO only | Not primary |
| Quantum ML / Quantum AI Researcher | Very niche; research-heavy | Uncertain near-term market | High academic prestige | Weak current fit | Not primary |
| Computational Scientist | Strong in research/science orgs | Durable but domain-specific | High | Partial | Not primary |
| Computer Vision Engineer | Strong applied demand | Strong in autonomy/medical/robotics | High | Weak current portfolio fit | Not primary |
| NLP Engineer | Strong but many NLP roles now folded into LLM roles | Strong but title is evolving | Medium-high | Partial | Secondary keyword |
| Multimodal AI Engineer | High-growth frontier/applied area | Strong future outlook | High | Weak current portfolio fit today | Future expansion |
| Robotics AI Engineer / Autonomous Systems Engineer | Strong in robotics/autonomy | Strong long-term | High | Weak current portfolio fit | Not primary |
| Reinforcement Learning Engineer | High prestige, smaller market | Strong in labs/robotics but narrow | Very high | Weak current portfolio fit | Not primary |
| Deep Learning Engineer | Strong but broad | Strong | High | Partial | Secondary keyword |
| Forward Deployed AI Engineer | High compensation at frontier labs and applied AI startups | Strong for customer-facing deployment | High business impact | Partial; profile is more infrastructure than customer deployment | Possible later |
| AI Quality / Evals Engineer | Emerging role around eval harnesses | Growing | Medium-high | Good if you add stronger eval projects | Future add-on |

## Key Research Findings

- BLS projects software developer employment to grow 15% from 2024 to 2034, driven partly by AI, robotics, and automation demand.
- WEF identifies AI and Machine Learning Specialists, Big Data Specialists, and Software/Application Developers among the fastest-growing roles through 2030.
- Indeed reports job postings mentioning AI surged more than 130% by the end of 2025 despite broader hiring weakness.
- AI compensation has split into mainstream applied AI roles and frontier-lab roles, with frontier labs paying dramatically higher total compensation through equity.
- Inference infrastructure, vLLM, Triton, GPU scheduling, latency optimization, evals, and cost monitoring are repeatedly cited as premium, scarce skill areas.
- Hiring guidance for LLM roles emphasizes shipped work, non-trivial GitHub projects, evaluation harnesses, serving systems, and infrastructure depth over certificates.

## Citations

- U.S. Bureau of Labor Statistics, Software Developers outlook: https://www.bls.gov/ooh/computer-and-information-technology/software-developers.htm
- BLS Employment Projections 2024-2034: https://www.bls.gov/news.release/ecopro.nr0.htm
- World Economic Forum, Future of Jobs Report 2025: https://www.weforum.org/publications/the-future-of-jobs-report-2025/in-full/2-jobs-outlook/
- Indeed Hiring Lab, AI job postings growth: https://www.hiringlab.org/2026/01/22/january-labor-market-update-jobs-mentioning-ai-are-growing-amid-broader-hiring-weakness/
- Indeed Hiring Lab, GenAI roles: https://www.hiringlab.org/2025/02/27/ai-at-work-rise-of-the-genai-consultant/
- Cadence, AI engineer salary 2026: https://cadence.withremote.ai/blog/ai-engineer-salary
- Pin, AI compensation benchmarks 2026: https://www.pin.com/blog/ai-compensation-salary-guide/
- AY Automate, AI engineer salary guide 2026: https://www.ayautomate.com/blog/ai-engineer-salary-guide-2026
- FutureProofing, Senior AI engineer rates Q2 2026: https://www.futureproofing.dev/blog/ai-talent-index-q2-2026
- KORE1, AI engineer job description 2026: https://www.kore1.com/ai-engineer-job-description/
- KORE1, hiring LLM engineers in 2026: https://www.kore1.com/hire-llm-engineers-2026/
- Riem.ai, ML systems engineers and inference infrastructure: https://riem.ai/blog/how-to-find-ml-systems-engineers
- AgenticCareers, AI Infrastructure Engineer role guide: https://agenticcareers.co/blog/ai-infrastructure-engineer-role-guide
- AgenticCareers, LLM Engineer guide: https://agenticcareers.co/blog/what-is-llm-engineer
- JobDescription.org, LLM Engineer role: https://jobdescription.org/jobs/artificial-intelligence/llm-engineer
- JobDescription.org, GPU Infrastructure Engineer role: https://jobdescription.org/jobs/artificial-intelligence/gpu-infrastructure-engineer
- Levels.fyi, OpenAI Software Engineer compensation: https://www.levels.fyi/companies/openai/salaries/software-engineer
- Levels.fyi, OpenAI Research Scientist compensation: https://www.levels.fyi/companies/openai/salaries/software-engineer/title/research-scientist
- Sundeep Teki, Research Engineer vs Research Scientist: https://www.sundeepteki.org/advice/research-engineer-vs-research-scientist-at-frontier-ai-labs
