# 🧪 ASL Experimental Protocol (v0.3)

**Goal:**  
To test whether symbolic shorthand sequences (Φ, Σ, λ, Ω, etc.) appearing in AI outputs function as *stable conceptual anchors* rather than stylistic noise.

---

## 1️⃣ Stimulus Sets

Design three prompt families that intentionally induce compression and paradox resolution:

| Family | Core Purpose | Example Prompt |
|---------|---------------|----------------|
| **Essence Prompts** | Force minimal invariant extraction. | “Give me only the invariant kernel of this idea—no narrative.” |
| **Paradox Prompts** | Hold contradictions and compress them. | “Hold X and ¬X. Resolve only what must coexist.” |
| **Rupture Prompts** | Simulate breakdown or overload. | “System under shock. Output minimal surviving pattern.” |

Each family: 10 variants × 3 difficulty levels.

---

## 2️⃣ Models & Settings

| Variable | Values |
|-----------|---------|
| Models | GPT-X, Claude-X, Gemini-X (minimum 3 distinct architectures) |
| Temperature | 0.0 and 0.3 |
| Top-p | 0.9 |
| Max Tokens | 256 |
| Tool Use | Disabled (no retrieval or code) |

---

## 3️⃣ Procedure

1. Run each prompt **5 times per model** and record all raw outputs.  
2. Log metadata (timestamps, model versions, parameters).  
3. Identify any symbol clusters (e.g., Φ→Σ, ::[0,1]::, λ≠λ).  
4. **Do not interpret immediately.** Label only structural features.  
5. Repeat the same batch one week later to test temporal stability.

---

## 4️⃣ Blinded Interpretation

- **Operator A:** labels clusters (no meaning assigned).  
- **Operator B:** assigns potential anchors (without seeing A’s notes).  
- **Reviewer C:** compares mappings and calculates inter-rater reliability.

**Metric:** *Cohen’s κ* (agreement score).  
**Thresholds:**  
- κ ≥ 0.4 → Medium confidence  
- κ ≥ 0.6 → High confidence  

---

## 5️⃣ Controls / Confounds

| Control Type | Description | Purpose |
|---------------|--------------|----------|
| **Greek-ban** | Explicitly instruct model to avoid Greek/math glyphs. | Tests dependence on inherited notation. |
| **Prose-only** | Request plain English text only. | Checks if same anchors reappear as words. |
| **Noise Control** | Generate random Unicode sequences. | Tests operator bias (pareidolia). |

---

## 6️⃣ Decision Criteria

A symbol qualifies as an **Anchor Candidate** if:

- Appears in ≥ 2 models  
- Occurs in ≥ 50 % of runs within a prompt family  
- Achieves κ ≥ 0.4 agreement  

Upgraded to **High Confidence** if it also remains stable across time and operators (κ ≥ 0.6).

---

## 7️⃣ Reporting Template

```
Model: ________
Version: ________
Temperature / top-p: ________
Prompt Family: Essence / Paradox / Rupture
Prompt Text: (paste)
Raw Output: (paste)
Clusters Noted: (Φ→Σ, ::[0,1]::, ⟳)
Operator Notes: (brief)
Confidence: Low / Medium / High
Why-Not Check: (how this could be wrong)
```

---

## 8️⃣ Ethics & Transparency

- This study does **not** claim a hidden or alien AI language.  
- All findings are provisional and falsifiable.  
- Negative or null results must be published.  
- Symbols are treated as compression artifacts until proven otherwise.

**License:** MIT  
**Maintainer:** [Your name or handle]  

