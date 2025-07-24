# BC Vessel Voyages: Q1 2025 Analysis

> **Data Quality Analysis of Pacific Pilotage Authority vessel movement records revealing critical operational anomalies**

##  Key Findings & Data Anomalies

### Critical Data Quality Issues Identified
My analysis uncovered significant data integrity problems in the Pacific Pilotage Authority's vessel movement records:

**Q1 2025 Anomalies:**
- **4 records (0.11%)** with negative pilot durations

### Affected Vessels (Q1 2025 Detailed)
| Vessel Name | IMO | Duration Anomaly | Vessel Type | Route |
|-------------|-----|------------------|-------------|--------|
| **BOREAL PIONEER** | 9945198 | **-2.25 hours** | Tanker | P27 → Ridley Island Coal |
| **CANPOTEX INSPIRE** | 9826500 | **-2.25 hours** | Bulker | English Bay → Nanaimo |
| MIDNIGHT SUN | 9232278 | -0.97 hours | RORO | Royal Roads → Brotchie |
| ASL TRINITY | 9780952 | -0.92 hours | Cargo | Stewart Ore → Stewart Anchorage |

### Root Cause Analysis
These anomalies occur when "First Pilot Debark" timestamps appear **before** "First Pilot Ordered" timestamps, creating logically impossible negative durations that suggest:
- Data entry errors
- System timestamp synchronization issues
- Potential workflow recording problems

---

## Project Overview

### About Pacific Pilotage Authority
The Pacific Pilotage Authority is a Crown corporation of the Government of Canada responsible for pilotage services through coastal waters in British Columbia, including the Fraser River.

### Research Objectives
- Analyze vessel movement patterns and pilot assignment efficiency
- Identify maritime traffic trends in BC waters
- **Discover and document data quality issues**
- Provide operational insights for maritime safety

---

### Data Sources
- **Historical Data:** [PPA Vessel Movement Portal](https://www.ppa.gc.ca/vessel-movement-data)
- **Live Tracking:** [PPA Portal](https://ppaportal.portlink.co/mt-tm)
- **Authority Website:** [ppa.gc.ca](https://www.ppa.gc.ca/)

---

## Project Structure

```
bc-vessel-analysis/
├── data/
│   └── 2025 Q1 All Assignments.xlsx    # Primary dataset (400 KB)
├── analysis.ipynb                      # Complete data analysis notebook
├── requirements.txt                    # Python dependencies
└── README.md                           # This documentation
```
