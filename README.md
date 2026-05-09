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

[🔍 Live Platform](https://raredex.nube.uni-greifswald.de/) • [📖 Overview](#overview) • [✨ Features](#features) • [📬 Contact](#contact)

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

#### ✨ Key Features

<p><strong>🔤 Phenotype Search</strong> — Describe a patient presentation in plain text. RareDex maps each term to HPO and retrieves the most similar cases.</p>

<p><strong>✅ HPO Mapping Review</strong> — Mapped terms and similarity scores are shown before retrieval executes, so the query can be confirmed or adjusted.</p>

<p><strong>🧬 Gene Search</strong> — Retrieve all cases associated with a gene symbol, grouped by disease.</p>

<p><strong>🔬 Gene + Variant Search</strong> — Narrow retrieval to cases carrying a specific variant using gene symbol and HGVS notation.</p>

<p><strong>📋 Case Dossiers</strong> — Each case is enriched with disease metadata, pathogenic variants, management guidance, and active clinical trials.</p>

<p><strong>📊 Interactive Evidence Synthesis</strong> — Evidence dashboard computed across retrieved cases — phenotype overlap, demographics, variant pathogenicity, and disease onset.</p>

<p><strong>📄 PDF Export</strong> — Download individual cases or full result sets.</p>

---

#### 📬 Contact

<p>Developed by <strong>Surya Mukhikuchibhotla</strong> · University Medicine Greifswald</p>

<p>
  <a href="mailto:suryamukhi.kuchibhotla@gmail.com">📧 Email</a> &nbsp;·&nbsp;
  <a href="https://github.com/suryamukhikuchibhotla">GitHub</a> &nbsp;·&nbsp;
  <a href="https://www.linkedin.com/in/skuchibhotla/">LinkedIn</a>
</p>
---