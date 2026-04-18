<div align="center">

# 🏥 TenzorX

### *The Kayak for Indian Healthcare*

**AI-powered decision intelligence that translates patient intent into clinical pathways, ranked providers, and transparent cost estimates — built for Bharat.**

<br/>

[![Made with ❤️ in India](https://img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F%20in-India-orange?style=for-the-badge)](https://github.com/TheyCallMeAnirban/tenzorX)
[![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)
[![Hackathon](https://img.shields.io/badge/Built%20For-Hackathon-blueviolet?style=for-the-badge)]()

<br/>

> *"We didn't build a chatbot. We built a structured intelligence layer that maps symptoms → conditions → providers → costs — with confidence scores you can trust."*

</div>

---

## 🎯 The Problem We're Solving

India has **1.4 billion people** and some of the most opaque healthcare pricing in the world.

A patient in **Nagpur, Patna, or Indore** facing a knee replacement or a cardiac event is left with three brutal unknowns:

| ❌ Without TenzorX | ✅ With TenzorX |
|---|---|
| "Which hospital should I go to?" | Ranked providers by capability, cost & distance |
| "How much will it cost?" | Itemized cost ranges with confidence scores |
| "Can I afford this?" | Financial implications mapped to clinical pathways |
| "Is this the right treatment?" | Standardized clinical mapping (ICD-10 / SNOMED CT) |

This matters beyond patients — **lenders and insurers** struggle to pre-approve healthcare loans without cost predictability. TenzorX provides that missing transparency layer.

---

## 🧠 How It Actually Works

TenzorX is not a search engine with a chat interface. It's a **4-stage decision intelligence pipeline**:

```
Patient Input (natural language)
       │
       ▼
 ┌─────────────────────────────────────┐
 │  Stage 1 — Clinical NLP Mapper      │
 │  Symptoms / conditions → ICD-10     │
 │  Standardized procedure categories  │
 └─────────────────┬───────────────────┘
                   │
                   ▼
 ┌─────────────────────────────────────┐
 │  Stage 2 — Provider Discovery       │
 │  Location + condition → ranked list  │
 │  Scoring: capability + reputation   │
 │  + accessibility + affordability    │
 └─────────────────┬───────────────────┘
                   │
                   ▼
 ┌─────────────────────────────────────┐
 │  Stage 3 — Cost Estimation Engine   │
 │  Procedure + city + patient profile │
 │  → itemized cost ranges             │
 │  Adjusts for age, comorbidities     │
 └─────────────────┬───────────────────┘
                   │
                   ▼
 ┌─────────────────────────────────────┐
 │  Stage 4 — Confidence-Aware Output  │
 │  Uncertainty indicators + caveats   │
 │  Decision support, NOT diagnosis    │
 └─────────────────────────────────────┘
```

---

## ✨ Key Features

### 🗣️ Natural Language Understanding
Query the system the way a real patient would:
- *"chest pain while climbing stairs"*
- *"best cancer hospital near Nagpur under ₹5 lakh"*
- *"knee replacement surgery cost in Patna"*

The system maps these to standardized medical concepts using **ICD-10** and **SNOMED CT** frameworks.

---

### 🏥 Transparent Provider Ranking

Every hospital recommendation is scored across **four explicit axes** — no black-box suggestions:

| Signal | What It Measures |
|---|---|
| 🔬 Clinical Capability | Specialization relevance, procedure volume |
| ⭐ Reputation | Public ratings, NLP-processed reviews, NABH accreditation |
| 📍 Accessibility | Distance from user, appointment availability |
| 💰 Affordability | Tier classification: Premium / Mid / Budget |

---

### 💸 Component-Level Cost Estimation

We don't give you a single number. We give you a **breakdown you can plan around**:

```
Condition: Coronary Artery Disease
Recommended Procedure: Angioplasty

🏥 ABC Heart Institute, Nagpur
   Rating: 4.5 ⭐  |  Distance: 5.2 km  |  NABH Accredited

Cost Breakdown:
  ├── Procedure/Surgery      ₹1,20,000 – ₹2,00,000
  ├── Hospital Stay (room)   ₹30,000  – ₹60,000
  ├── Medications            ₹15,000  – ₹30,000
  ├── Diagnostics (pre/post) ₹10,000  – ₹20,000
  └── Contingency            ₹15,000  – ₹40,000
                             ─────────────────────
  Total Estimated Range      ₹1.8L    – ₹3.5L

Confidence Score: 0.68 / 1.0

⚠️  Notes:
  • Costs may increase 20-30% if ICU care is required
  • Diabetic patients may face extended recovery periods
  • Estimate does not include post-discharge physiotherapy
```

---

### 🔀 Multi-Source Intelligence Fusion

| Data Type | Source | Usage |
|---|---|---|
| Structured | Hospital directories, procedure categories | Provider base data |
| Unstructured | Reviews, testimonials | NLP-based reputation scoring |
| Derived | Cost benchmarks, geographic adjusters | Realistic range estimation |
| Synthetic | Reasoned procedure cost proxies | Where public data is sparse |

The focus is **thoughtful data fusion** over raw data volume.

---

## 🛡️ Responsible AI Design

We took the ethical guardrails as seriously as the features.

- **No diagnosis, ever.** TenzorX is a decision-support tool, not a doctor.
- **Confidence scores** on every output — we never hide uncertainty.
- **Explicit disclaimers** at every cost and provider recommendation.
- **Symptom-to-condition mapping** is probabilistic, not deterministic — users are told this.
- **High variance in pricing** is surfaced as a range, not falsely collapsed into a single number.

---

## 🗂️ Project Structure

```
tenzorX/
│
├── 📁 core/
│   ├── nlp_mapper.py          # Symptom → ICD-10 / SNOMED CT mapping
│   ├── provider_ranker.py     # Multi-signal hospital scoring engine
│   └── cost_estimator.py      # Component-level cost range generator
│
├── 📁 data/
│   ├── hospital_directory/    # Structured hospital & specialty data
│   ├── procedure_benchmarks/  # Cost benchmarks by city/procedure
│   └── icd10_mappings/        # Condition-to-code reference tables
│
├── 📁 api/
│   └── routes.py              # REST API endpoints
│
├── 📁 frontend/
│   └── ...                    # User interface
│
├── 📁 tests/
│   └── ...                    # Unit + integration tests
│
└── README.md
```

---

## 🚀 Getting Started

### Prerequisites
- Python 3.10+
- pip / conda

### Installation

```bash
# Clone the repository
git clone https://github.com/TheyCallMeAnirban/tenzorX.git
cd tenzorX

# Install dependencies
pip install -r requirements.txt

# Run the application
python app.py
```

### Example Query (API)

```python
import requests

payload = {
    "query": "knee replacement surgery",
    "location": "Patna",
    "age": 58,
    "comorbidities": ["diabetes"],
    "budget": 300000
}

response = requests.post("http://localhost:5000/api/recommend", json=payload)
print(response.json())
```

---

## 📊 Evaluation Dimensions

| Criteria | Weight | Our Approach |
|---|---|---|
| Clinical Mapping Accuracy | 20% | ICD-10 + SNOMED CT normalization |
| Cost Estimation Logic | 25% | Component breakdown + comorbidity adjusters |
| Provider Ranking Quality | 20% | Transparent multi-signal scoring |
| Multi-Source Intelligence | 15% | Structured + unstructured data fusion |
| User Experience & Clarity | 10% | Conversational NL interface + clean outputs |
| Responsible AI Practices | 10% | Confidence scores, disclaimers, no diagnosis |

---

## 🌍 Real-World Impact

TenzorX is designed to evolve into:

- 🏦 **Pre-underwriting layer** for healthcare lending — predictable costs enable confident loan approvals
- 🔍 **Cost transparency tool** for patients across Tier 2/3 cities
- 📊 **Hospital comparison platform** — think Kayak, but for Indian healthcare decisions

---

## 👨‍💻 Team

Built with conviction at the hackathon by:

<table>
  <tr>
    <td align="center"><b>Anshuman Kumar Singh</b></td>
    <td align="center"><b>Anirban Goswami</b></td>
    <td align="center"><b>Shumaque Raza</b></td>
  </tr>
</table>

---

## ⚠️ Disclaimer

TenzorX is a **decision-support tool only**. It does not provide medical diagnosis, treatment advice, or definitive cost guarantees. All cost estimates are ranges based on public benchmarks and synthetic data. Always consult a qualified medical professional for health decisions.

---

<div align="center">

**If this solves a problem you've faced — or someone you love has faced — give it a ⭐**

*Built for India. Built for clarity. Built for the 1.4 billion.*

</div>
