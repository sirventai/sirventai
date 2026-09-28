<div align="center">

# Pablo Sirvent

### Founder of [PureByte](https://purebyte.ai) · AI Systems & Low-Level Inference Engineer

[![Website](https://img.shields.io/badge/Website-sirvent.ai-0969da?style=flat-square&logo=googlechrome&logoColor=white)](https://sirvent.ai)
[![PureByte](https://img.shields.io/badge/PureByte-purebyte.ai-10b981?style=flat-square&logo=fastapi&logoColor=white)](https://purebyte.ai)
[![Paper DOI](https://img.shields.io/badge/Zenodo%20DOI-10.5281%2Fzenodo.23020056-blue?style=flat-square&logo=doi&logoColor=white)](https://doi.org/10.5281/zenodo.23020056)
[![GitHub](https://img.shields.io/badge/GitHub-@sirventai-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/sirventai)
[![Twitter](https://img.shields.io/badge/𝕏-@sirventai-000000?style=flat-square&logo=x&logoColor=white)](https://x.com/sirventai)
[![Blog](https://img.shields.io/badge/Medium-Blog-00ab6c?style=flat-square&logo=medium&logoColor=white)](https://sirventai.medium.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-pablosirvent-0077b5?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/pablosirvent)
[![Email](https://img.shields.io/badge/Email-pablo@purebyte.ai-ea4335?style=flat-square&logo=gmail&logoColor=white)](mailto:pablo@purebyte.ai)

</div>

---

### ⚡ Flagship Project: PureByte

> **"SLMs are the future."** — Dependency-free C++17 runtime & tiny learned sequence models (1–29 MiB) that run offline on ordinary CPUs in **<1 ms** without GPUs.

```
 [Raw Byte Stream]  ──────── (Tokenizer-free / No Vocab Overhead)
        │
        ▼
 [Mamba-2 SSM Backbone] ──── (1.58-bit Ternary QAT / Linear O(N) Time)
        │
        ▼
 [Typed Decision Heads] ──── Output exact Byte Spans, Decisions & Scores (0 Hallucination)
        ▲
 [C++17 SIMD Runtime]   ──── AVX-512 · AVX2 · ARM NEON (Zero External Dependencies)
```

#### Benchmark Results (from our [109-Page Technical Paper](https://doi.org/10.5281/zenodo.23020056))

| Specialist Model | Parameters | Weights File | CPU Latency (12 cores) | Benchmark Metric | vs Industry Baselines |
| :--- | :---: | :---: | :---: | :--- | :--- |
| **CredSpecialist** | 1.9M | **1.1 MB** | **0.82 ms** | **3.5x Recall** on CredData (168 repos) | Outperforms Gitleaks default rules |
| **PIISpecialist** | 8.3M | **3.2 MB** | **1.20 ms** | **F2 0.769** on PII Masking Benchmark | Outperforms OpenAI Privacy Filter (1.4B) |
| **BaseSpecialist** | 12.6M | **4.5 MB** | **1.80 ms** | Exact bit-parity with PyTorch | **13x faster/core**, **85x end-to-end** |

- **Standalone C++17 Engine:** Zero external dependencies, pure SIMD intrinsics (AVX-512, AVX2, NEON).
- **Automated Verification:** 400+ unit and regression tests ensuring identical output across hardware architectures.
- **Code Repositories:** [purebyte-ai/purebyte](https://github.com/purebyte-ai/purebyte) *(Runtime)* · [purebyte-ai/purebyte-train](https://github.com/purebyte-ai/purebyte-train) *(Training Stack)*

---

### 🛠️ Tech Stack & Engineering Core

<table>
  <tr>
    <td width="25%"><strong>AI Systems & Performance</strong></td>
    <td>
      <img src="https://img.shields.io/badge/C++17-SIMD%20(AVX512%2FAVX2%2FNEON)-00599C?style=flat-square&logo=c%2B%2B&logoColor=white" />
      <img src="https://img.shields.io/badge/Python-3.11+-3776AB?style=flat-square&logo=python&logoColor=white" />
      <img src="https://img.shields.io/badge/PyTorch-Deep%20Learning-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" />
      <img src="https://img.shields.io/badge/Mamba--2-State%20Space%20Models-8A2BE2?style=flat-square" />
      <img src="https://img.shields.io/badge/Quantization-1.58--bit%20Ternary%20QAT-orange?style=flat-square" />
      <img src="https://img.shields.io/badge/Linux-Kernel%20Profiling%20&%20Perf-FCC624?style=flat-square&logo=linux&logoColor=black" />
    </td>
  </tr>
  <tr>
    <td width="25%"><strong>Distributed Backend & Cloud</strong></td>
    <td>
      <img src="https://img.shields.io/badge/Java-21%20LTS-ED8B00?style=flat-square&logo=openjdk&logoColor=white" />
      <img src="https://img.shields.io/badge/Kotlin-Multiplatform-7F52FF?style=flat-square&logo=kotlin&logoColor=white" />
      <img src="https://img.shields.io/badge/Quarkus-Cloud%20Native-4796F4?style=flat-square&logo=quarkus&logoColor=white" />
      <img src="https://img.shields.io/badge/Apache%20Kafka-Event%20Streaming-231F20?style=flat-square&logo=apachekafka&logoColor=white" />
      <img src="https://img.shields.io/badge/PostgreSQL-Data%20Architecture-4169E1?style=flat-square&logo=postgresql&logoColor=white" />
      <img src="https://img.shields.io/badge/Kubernetes-Production%20K8s-326CE5?style=flat-square&logo=kubernetes&logoColor=white" />
      <img src="https://img.shields.io/badge/Go-Microservices-00ADD8?style=flat-square&logo=go&logoColor=white" />
    </td>
  </tr>
  <tr>
    <td width="25%"><strong>Security & Systems</strong></td>
    <td>
      <img src="https://img.shields.io/badge/Zero--Trust-Edge%20Gateways-critical?style=flat-square" />
      <img src="https://img.shields.io/badge/Cryptography-Post--Quantum%20(Kyber%2FDilithium)-darkgreen?style=flat-square" />
      <img src="https://img.shields.io/badge/Hard%20Real--Time-HIL%20%2F%20SIL%20Simulators-blueviolet?style=flat-square" />
    </td>
  </tr>
</table>

---

### 💼 Career Snapshot

- **[Indra Group](https://www.indracompany.com/)** *(2023 – Present)*: Senior Software Engineer (Senior Specialist). Scalable backend microservices (Java 21, Kotlin, Quarkus, Kafka, Kubernetes) for high-criticality systems in defense and government programmes.
- **[Embention](https://www.embention.com/)** *(2022 – 2023)*: Senior Software Engineer. Critical autopilot backend systems and real-time HIL/SIL flight simulators for Veronte UAV autopilots (Amazon Prime Air tier; 70+ countries).
- **[Afterbanks Arcopay](https://www.afterbanks.com/)** *(2021)*: Software Engineer. PSD2 open banking aggregation platform (Java, Spring, MySQL).
- **[Orizon](https://orizon.es/)** *(2021 – 2022)*: Software Engineer. Mainframe CPU performance engineering and profiling for Spain's largest commercial banks.
- **[GESIO](https://www.gesio.com/)** *(2017 – 2021)*: Software Engineer. Led 3-person backend team for cloud ERP & POS SaaS (3,000+ businesses).

---

### 🎓 Education, Honors & Certifications

- **BSc in Computer Engineering**, Universitat Oberta de Catalunya (GPA: **8.52 / 10**).
  - **7 Distinctions & Honours** (*Matrículas de Honor / Sobresalientes*): Mathematical Analysis (10/10 MH), Final Thesis (10/10 MH), Artificial Intelligence, Cryptography, Network Security, Component & Distributed Systems Engineering.
- **Red Hat Certified Specialist in Cloud-native Microservices Development with Quarkus** (DO378, Feb 2025) · [Credly Badge](https://www.credly.com/badges/fd113b08-8667-418f-b513-5b9d83cf7cd2).
- **Winner Santander Explorer UA 2019 & Campus & Technology Award**: Silicon Valley tech immersion trip (San Francisco, UC Berkeley, Stanford mentors) for **Wazime** (ultrasonic near-field data transfer).

---

<div align="center">

```
  ____  _             ZW        _       
 / ___|(_)_ ____   _____ _ __ | |_     
 \___ \| | '__\ \ / / _ \ '_ \| __|    Pablo Sirvent
  ___) | | |   \ V /  __/ | | | |_     https://sirvent.ai
 |____/|_|_|    \_/ \___|_| |_|\__|    pablo@purebyte.ai
```

</div>
