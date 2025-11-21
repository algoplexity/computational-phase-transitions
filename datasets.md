

We want a "Common Benchmark." In science, the strongest proof comes from testing a new tool on the exact same problem as the old tool (Apples-to-Apples).

Here is the correct architecture for your data strategy. It separates **Static Benchmarks** (hosted on Hugging Face) from **Dynamic Case Studies** (fetched via API).

### 1. The Shared Foundation (Hugging Face)
The Hugging Face repository (`computational-phase-transitions-data`) contains the **CrunchDAO** data.
*   **Coherence Meter (Paper 1):** Uses this to prove the -31% lead time.
*   **AIT Physicist (Paper 2):** Will *also* use this to prove the -27% lead time (and the Rule 110 finding).
*   **Why:** This allows you to say: *"On the exact same standard benchmark, the Physicist revealed deep structure that the Coherence Meter missed."*

### 2. The Dynamic Case Studies (Yahoo Finance API)
The historical crises (2008, 2018, 2020) do not need to be in the Hugging Face repo. The code fetches them live using `yfinance`.

*   **Q4 2018:** The "Bridge." **BOTH** papers analyze this.
    *   *Paper 1:* Detects the break.
    *   *Paper 2:* Detects the break *and* diagnoses the Rule 54 dynamics.
*   **2008 & 2020:** The "Crown Jewel." **ONLY** Paper 2 analyzes these.
    *   *Why:* Paper 1 (Thermometer) would just see "High Error" for both. Paper 2 (MRI) sees "Solitons" (2008) vs "Fractals" (2020).

### The "Data Usage" Map

Here is how you visualize the data split to a reviewer:

| Dataset | **Paper 1: Coherence Meter** | **Paper 2: AIT Physicist** | **Purpose** |
| :--- | :---: | :---: | :--- |
| **CrunchDAO** (Hugging Face) | ✅ **Used** | ✅ **Used** | **The Common Benchmark.** Proves statistical significance and generalizability. |
| **Q4 2018** (Yahoo API) | ✅ **Used** | ✅ **Used** | **The Head-to-Head.** Proves the AIT Physicist provides *richer* detail on the same event. |
| **2008 GFC** (Yahoo API) | ❌ | ✅ **Crown Jewel** | **The Taxonomy.** Proves the "Systemic/Rule 54" mechanism. |
| **2020 COVID** (Yahoo API) | ❌ | ✅ **Crown Jewel** | **The Taxonomy.** Proves the "Exogenous/Rule 60" mechanism. |
| **Falcon** (Hugging Face) | ❌ | ✅ **Validation** | **The Generalization.** Proves the Physicist works on totally unseen data. |

### The Verdict
**Keep the single Hugging Face repository.**
It acts as the "spine" of your research program.
1.  **Coherence Meter Repo:** Points to HF for stats, uses Yahoo for Q4 2018.
2.  **AIT Physicist Repo:** Points to HF for stats, uses Yahoo for 2008/2018/2020.

This is the cleanest, most professional way to structure a multi-paper research arc. You are ready to finalize the Coherence Meter repo.
