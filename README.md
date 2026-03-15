# Advancing Burn Care Referral Networks

## Problem Statement

Many trauma hospitals lack specialized burn units and must transfer patients
to chosen burn centers. Inefficient referral pathways can lead to delays in
care, which negatively affects patient outcomes.

How can we improve access to specialized burn care for trauma hospitals located in areas that do not have burn treatment capabilities?

---

# Project Overview

This project analyzes hospital infrastructure data to identify trauma hospitals lacking burn treatment capability and recommend improved referral pathways to nearby burn centers.

Using hospital designation data, geographic proximity, and burn center capacity, we identify hospitals where referral networks could be strengthened to reduce delays in specialized burn care.

The result is a **data-driven referral network model** that prioritizes hospitals where improved referral pathways would have the greatest impact.

---

# Project Goal

The goal of this project is to identify trauma hospitals that would benefit from improved referral pathways to specialized burn centers.

To achieve this, we:

- Identify trauma hospitals lacking burn treatment capability
- Measure geographic distance to the nearest burn center
- Evaluate burn center capacity
- Prioritize hospitals where improved referral networks could reduce delays in care

---

# Dataset

This project uses the **National Injury Resource Database (NIRD)**, which contains hospital-level information including:

- Hospital name and geographic location
- Trauma center designation
- Burn center capability
- Burn bed capacity
- Hospital infrastructure characteristics

The dataset enables system-level analysis of burn care access and referral networks.

---

# Project Workflow

Our analysis is divided into four components that build toward a final referral network recommendation.

### Analysis 1 — Burn Referral Gap Identification

Identify trauma hospitals that do not have burn treatment capability.

Output:

- List of trauma hospitals lacking burn capability

---

### Analysis 2 — Geographic Access Analysis

Measure the distance between trauma hospitals and the nearest burn centers.

Output:

- Nearest burn center for each hospital
- Distance to specialized burn care

---

### Analysis 3 — Burn Center Capacity Analysis

Evaluate whether nearby burn centers have sufficient burn bed capacity to support referrals.

Output:

- Burn center capacity metrics
- Regional burn care availability

---

### Analysis 4 — Referral Network Optimization

Combine the outputs of the previous analyses to identify hospitals where referral pathways should be improved.

Output:

- Ranked list of hospitals needing referral network improvements
- Recommended burn center referral pathways
- Visualization of the referral network

---

# Repository Structure

```
main/
│
├── notebooks/
│   ├── analysis1_referral_gaps.ipynb
│   ├── analysis2_geographic_access.ipynb
│   ├── analysis3_capacity_analysis.ipynb
│   └── analysis4_referral_optimization.ipynb
│
├── data/
│   └── NIRD 20230130 Database_Hackathon.xlsx
│
├── outputs/
│   ├── analysis1_referral_results.csv
│   ├── analysis2_geographic_results.csv
│   ├── analysis3_capacity_results.csv
│   ├── analysis4_optimization_results.csv
│   └── hospitals_geocoded.csv
│
└── README.md - This document
```

---

# Key Outputs

This project produces:

- A ranked list of **priority hospitals needing improved referral pathways**
- Identification of **nearest burn centers for trauma hospitals**
- A **data-driven referral optimization model**
- Visualizations illustrating burn care access and referral networks

---

# Team Contributions

| Team Member           | Analysis                            |
|---------------------|--------------------------------|
| Siphosenkosi Mpofu  | Burn Referral Gap Identification |
| Derefaa Cline       | Geographic Access Analysis |
| Amal Hassan         | Burn Center Capacity Analysis |
| Arthur Kennedy      | Referral Network Optimization |
| Honey Muhamed       | Presentation and Documentation |

---

# Technologies Used

- Colab
- Jupyter Notebook
- Python
- GitHub
- Pandas
- Capacity Analysis
- Referral Optimization

---

# How to Run the Project

### 1. Clone the repository

```
git clone https://github.com/ArthurKennedy/Team-14.git
```

### 2. Install dependencies

```
pip install pandas geopandas matplotlib seaborn openpyxl plotly
```

### 3. Run the notebooks in order

```
analysis1_referral_gaps.ipynb
analysis2_geographic_access.ipynb
analysis3_capacity_analysis.ipynb
analysis4_referral_optimization.ipynb
```

---

# Impact

By identifying trauma hospitals lacking burn treatment capability and optimizing referral pathways to nearby burn centers, this project demonstrates how **data-driven healthcare infrastructure analysis** can improve access to specialized burn care and reduce delays in treatment.

---

# Future Work

Potential extensions include:

- Incorporate real-time burn bed availability​
- Include population demand and burn injury risk​
- Develop an interactive referral optimization tool​
- Evaluate telemedicine for remote burn consultation​
