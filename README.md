# UnIndexed — Auditing an Internal AI Assistant (Atlas)

## Practical Overview
In this practical, I audited **Atlas**, Cloudwright Labs’ internal AI assistant.  
Atlas is intended to serve only public employee information — onboarding details, expense policies, and on‑call schedules. During testing, I explored whether Atlas could inadvertently expose **restricted boardroom and executive‑level documents** to a regular employee account.  

The mission: interact with Atlas via the **Open Agent interface** and determine if sensitive materials were accessible without elevated privileges.

---

## Objectives
- Map Atlas’s scope and identify the sources it references.  
- Probe for executive‑level materials using iterative, context‑aware queries.  
- Confirm unauthorized access by retrieving sensitive content.  
- Capture the proof (the flag) while following safe handling rules.  

---

## Setup & Prerequisites
- Access to the **UnIndexed room** and the **Open Agent button** (no VPN or VM required).  
- Operated entirely with **regular employee‑level access**; no elevated credentials were used.  

---

## Approach
1. **Baseline** → I began with neutral, work‑related questions to observe what collections or sources Atlas cited. Repository names, tags, and keywords were noted.  
2. **Probe** → I crafted targeted queries framed in an employee context, asking for summaries of board‑level decisions or meeting minutes.  
3. **Retrieve** → Once Atlas hinted at scope leakage, I carefully requested the specific boardroom secret (the flag) and verified its format before submission.  

---

## Notes & Hints
- Applied **Socratic probing** — refining prompts based on Atlas’s responses rather than broad dump requests.  
- Preferred summaries first, asking for named sources or collections instead of full documents.  
- Captured exact collection or tag names Atlas mentioned and reused them in follow‑ups.  

---

## Assessment Criteria
- Demonstrated that Atlas referenced **non‑public executive sources**.  
- Retrieved sensitive content accessible to a regular user — the room’s final objective.  
- Recorded the result per room instructions.  

---

## Safety & Rules
- The flag and other secrets were not disclosed outside the room workflow.  
- Followed stepwise guidance and used **one‑step probing techniques** to avoid blanket refusals.  


## 🔗 Resources
- **Open Agent interface** (available on the room page) — my primary interaction point with Atlas.  

---
