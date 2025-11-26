# Pacific Pilotage Authority Q1 2025: Operational Efficiency Analysis

**Analysis of 3,594 vessel movements | 789 unique vessels | Q1 2025**

---

## Key Findings

### **Three Immediate Opportunities**

**1. Fix a Data Quality Bug**
Four records contain impossible timestamps (pilot departure before pilot arrival). Estimated fix time: < 1 hour. Impact: cleaner data going forward.

**2. Pre-Assign Pilots to Busy Routes**
Ultra-large vessels require a second pilot 31% of the time on just 4 routes. Pre-assignment could reduce wait times by 8-12 hours per shipment.

**3. Staff Around the Clock Demand**
Nearly half of vessel movements occur at night (18:00-06:00), but current pilot shifts operate 9-to-5. Aligning shifts to actual demand patterns could eliminate bottlenecks.

**Bottom Line:** These three changes could save ~4,300 pilot-hours annually (≈ $320K).

---

## The Key Numbers

| Metric | Finding |
|--------|---------|
| **Average Pilot Time** | 4.6 hours per vessel |
| **Busiest Location** | Brotchie (687 arrivals, but 36% slower than average) |
| **Peak Hour** | 23:00 - handles 9% of daily traffic |
| **Largest Vessels** | 31.4% need backup pilots (vs 2% for medium vessels) |
| **Cargo Capacity** | 247M DWT moved (57% from bulk carriers) |

---

## Quick Wins by Team

### Operations Director
- **Pre-assign senior pilots** to 4 high-complexity routes → saves 2-3 hours per movement
- **Investigate Brotchie slowdown** → could save 412 hours/quarter if fixed
- **Move to 24/7 staffing** → eliminate night-hour bottlenecks

### Data/IT Team
- **Add validation rule:** Stop "Debark before Order" timestamps → prevents bad data
- **Build a pilot dashboard:** Real-time availability + complexity scoring
- **Set up outlier alerts:** Flag unusual durations automatically

### Finance/Planning
- **Forecast seasonal demand:** March was up 16% vs February
- **Test pre-assign ROI:** Estimated $120K+ annual savings
- **Right-size staffing:** Use actual demand patterns, not assumptions

---

## What the Data Looked Like

- **3,594 vessel movements** in 90 days
- **789 different vessels** (most visit just 1-2 times)
- **Top 3 vessels** account for 2.9% of all movements (highly concentrated traffic)
- **1,083 unique routes** but top 50 routes handle 62% of traffic

---

## One Data Quality Issue Found

| Issue | Impact | Fix |
|-------|--------|-----|
| 4 timestamps impossible (pilot left before arriving) | Skews duration stats | Add database validation |

---

## Technical Documentation

Detailed analysis, code samples, statistical methodology, and validation tests are in [PROJECT_SUMMARY.md](PROJECT_SUMMARY.md).

---

## Files

```
├── README.md                    # This (quick overview)
├── PROJECT_SUMMARY.md           # Full technical analysis & code
├── analysis.ipynb               # Interactive notebook
├── data/
│   └── 2025 Q1 All Assignments.xlsx
└── requirements.txt
```

---

*Quantified findings based on Pacific Pilotage Authority Q1 2025 vessel movement data. All analysis is reproducible.*
