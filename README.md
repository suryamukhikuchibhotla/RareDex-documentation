<div align="center">

<img src="image1.png" alt="RareDex" width="100%">

## *"When you hear hoofbeats, think horses, not zebras."*

### 🧬 Rare disease case retrieval for clinical decision support

<sub>🏛️ University Medicine Greifswald &nbsp;·&nbsp; Institute of Bioinformatics</sub>


---

![Status](https://img.shields.io/badge/Status-Live-brightgreen?style=flat-square)
![GA4GH](https://img.shields.io/badge/GA4GH-Phenopackets_v2-orange?style=flat-square)
![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-14-black?style=flat-square&logo=next.js)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)

---

| 🧪 9,688 patient cases | 🦓 643 rare diseases | 🧬 641 genes | 📋 GA4GH Phenopackets |
|:---:|:---:|:---:|:---:|

---

[🔍 Live Platform](https://raredex.nube.uni-greifswald.de/) • [📖 Overview](#overview) • [⚙️ Architecture](#architecture) • [✨ Features](#features) • [📬 Contact](#contact)

</div>

---

### 🎯 The Mission

<p>In medicine, the proverb <em>"think horses, not zebras"</em> reminds clinicians to favor common diagnoses. But for the <strong>estimated hundreds of millions of people</strong> worldwide living with a rare disease, the <strong>zebra is the reality</strong>.</p>

<p>Reaching a diagnosis takes an average of <strong>4.8 years</strong>, often involving a diagnostic odyssey of misdiagnoses and unnecessary investigations. <strong>RareDex</strong> bridges this gap — giving clinicians an infrastructure to systematically compare patient phenotypes against thousands of documented cases, and surface what happened next.</p>

---

### 📖 Overview

<p><strong>RareDex</strong> is a phenotype-driven rare disease case retrieval system built for clinical research. Given a patient's symptoms, it searches a corpus of <strong>9,688 structured rare disease cases</strong> across <strong>643 diseases</strong> to surface phenotypically similar prior cases — together with their pathogenic variants, management evidence, and clinical trial data.</p>

<p>Built on the <a href="https://github.com/monarch-initiative/phenopacket-store">GA4GH Phenopacket Store</a>, a curated collection of structured rare disease cases encoded in the <a href="https://phenopackets.org">GA4GH Phenopacket schema</a>.</p>

---

#### ⚙️ Architecture

```mermaid
flowchart TD
    %% Node Definitions
    User([👨‍⚕️ Clinician Input])
    Input{Query Type}
    
    subgraph Engine [RareDex Processing Engine]
    Mapping[🧠 Semantic HPO Mapping]
    Review[✅ Physician Validation]
    Search[[🔍 Ontology-Aware Retrieval]]
    end
    
    subgraph Data [Data Foundations]
    Pheno[(📋 GA4GH Phenopackets)]
    Onto[(🧬 HPO Graph)]
    end
    
    subgraph Output [Clinical Decision Support]
    Ranked[📊 Ranked Case Dossiers]
    Details[💊 Evidence Synthesis]
    AI[🤖 AI Case Summary]
    end

    %% Connections
    User --> Input
    Input -->|Plain Text| Mapping
    Input -->|Gene/Variant| Search
    
    Mapping --> Review
    Review --> Search
    
    Onto -.-> Mapping
    Onto -.-> Search
    Pheno -.-> Search
    
    Search --> Ranked
    Ranked --> Details
    Ranked --> AI

    %% Styling
    style Engine fill:#f9f9f9,stroke:#009688,stroke-width:2px
    style Output fill:#f0fdfa,stroke:#009688,stroke-width:2px
    style Data fill:#fff7ed,stroke:#ea580c,stroke-width:1px
    style User fill:#009688,color:#fff,font-weight:bold
```
