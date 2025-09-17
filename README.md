# Drug Safety Analysis

In this project, we analyze clinical trial data to determine whether a drug has a significant effect on participants.  

---

## 📊 Dataset Description
The dataset includes both **treatment (Drug)** and **control (Placebo)** groups.  

- **Control Group (Placebo):** Participants who did not receive the actual drug. This group helps us measure natural changes or psychological effects (placebo effect).  
- **Treatment Group (Drug):** Participants who received the actual drug. Differences between this group and the control group indicate the drug’s potential effects.  

### Features
- **age** → Age of the participant  
- **sex** → Gender of the participant (male or female)  
- **trx** → Treatment group:  
  - `"Drug"` → Received the actual drug  
  - `"Placebo"` → Received a placebo (control group)  
- **week** → Week number in the study  
- **wbc** → White blood cell count (WBC) measurement  
- **rbc** → Red blood cell count (RBC) measurement  
- **adverse_effects** → Presence of adverse effects (Yes or No)  
- **num_effects** → Number of adverse effects experienced by the participant  

---

## 📐 Methodology
We used **hypothesis testing** to evaluate the safety and effectiveness of the drug:  

- **Null Hypothesis (H₀):** The drug has an effect.  
- **Alternative Hypothesis (H₁):** The drug has no significant effect.  

We tested this by calculating **p-values** for different comparisons between the treatment and control groups.  

---

## 🔎 Key Concepts

### ✅ Hypothesis Testing
Hypothesis testing is a statistical method used to decide whether the observed data provides enough evidence to reject the null hypothesis.  
- If the evidence strongly contradicts H₀, we reject it in favor of H₁.  
- Otherwise, we fail to reject H₀ (i.e., we don’t have enough evidence to say the drug has no effect).  

### ✅ P-value
The **p-value** represents the probability of observing the given data (or something more extreme) under the assumption that the null hypothesis (H₀) is true.  
- A **small p-value (e.g., < 0.05)** suggests strong evidence against H₀ → we reject the null hypothesis.  
- A **large p-value** suggests weak evidence against H₀ → we fail to reject the null hypothesis.  

---

## 🎯 Conclusion
By analyzing mean outcomes, standard deviations, and p-values, we determined whether the **drug’s effects** (both beneficial and adverse) are statistically significant compared to the placebo group.
