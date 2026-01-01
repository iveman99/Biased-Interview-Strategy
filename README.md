# 🎯 The Biased Interview Strategy  
### An Optimal Decision Rule Under Information Constraints

---

## 🧩 Problem Overview

A company interviews **7 candidates** sequentially in a fixed order:

A, B, C, D, E, F, G


Each candidate has a unique hidden ability score from **1 (worst) to 7 (best)**.
After each interview, the hiring manager only learns the **relative ranking**
among candidates seen so far — absolute scores are never revealed.

Once a candidate is rejected, they **cannot be recalled**.
Exactly **one candidate must be hired**, with the goal of **maximizing the probability
of selecting the overall best candidate (score = 7)**.

---

## 🔍 Special Conditions

- Candidates **A–E** arrive in **strictly increasing quality order**  
  *(A < B < C < D < E)*  
- Candidates **F and G** arrive later and may be better or worse than E  
- All rankings consistent with these constraints are equally likely  

---

## ✅ Decision Rule

**Reject candidates A–E.**  
Use candidate **E** as a benchmark.

- Interview **F** and **hire F immediately if F is better than E**
- If **F is not better than E**, interview **G** and **hire G**

---

## 🧠 Justification (Rigorous Argument)

Because candidates A–E are strictly increasing in quality, **E is the best among
the first five candidates**. Therefore, none of A–D can be the optimal choice.

The overall best candidate must be **either E, F, or G**.

This strategy:
- Never selects a candidate worse than E
- Selects the **first candidate among F or G** who exceeds E, if such a candidate exists
- Defaults to hiring G only when no better option is possible

Thus, this rule **maximizes the probability of selecting the overall best candidate**
using only relative rankings and the information given.

---

## 📄 Deliverable

- `The Biased Interview Strategy.pdf`  
  Concise solution (≤150 words) with a logically complete justification

---

## 🛠️ Key Concepts Used

- Sequential decision-making
- Optimal stopping theory (variant)
- Relative ranking under uncertainty
- Probability maximization under constraints

---

## 📝 Notes

- No simulations or assumptions beyond the problem statement
- Focus is on **logical completeness and explainability**
- Solution is intentionally concise and interview-defensible

---

## 👨‍💻 Author

**Veman S Chippa**  
_Data Analyst / Data Engineer_

🌐 Portfolio: https://iveman.vercel.app/  
💼 LinkedIn: https://www.linkedin.com/in/veman-chippa  
