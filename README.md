# Mapping the Lexicon of Hate
### Offensive Language Structure in Korean Online Discourse
*Research Paper | University of Tübingen, 2025–2026*

## Overview
Korean offensive language is not random profanity — 
it is a structured system of framing strategies shaped 
by Korea's specific sociopolitical context.

This study analyzes the KOLD dataset (40,429 comments 
from NAVER and YouTube) across three progressively 
deeper questions:
- **Who** is attacked? (target group distribution)
- **Which groups** are attacked together? (co-targeting network)
- **How** are they attacked? (offensive framing patterns)

- 
## Approach
Three-layer analysis framework designed independently:

1. **Target group distribution** — EDA on 21 culturally 
grounded target categories
2. **Co-targeting network** — NetworkX-based network 
construction from 278 multi-target comments; 
node-level (weighted degree × betweenness centrality) 
and cluster analysis
3. **Offensive framing** — Concept taxonomy abstraction 
from offensive spans; normalized heatmap per target group


## Key Findings

**1. Ideology over identity**  
Unlike English datasets (HateXplain), where racial 
minorities top the rankings, *feminist* ranks first in 
KOLD — reflecting that Korean offensive discourse 
targets what people *believe* more than who they *are*.
This pattern is consistent with the intensification of 
Korea's culture war discourse since the mid-2010s.

**2. Gender as structural axis**  
Female holds the highest betweenness centrality (0.567), 
connecting race, religion, ideology, and sexuality within 
a single network. Gender conflict in Korea is not binary 
but a three-way ideological confrontation: 
female–feminist–male (co-targeting: 46, 18, 18).

**3. Target-specific framing strategies**  
| Target Group | Dominant Frame | Example |
|---|---|---|
| feminist, progressive | Pathologization | 정신병 (mental illness) |
| korean_chinese | Outsider framing (1.00) | ethnic slurs |
| female | Role stereotype (0.81) | 군대 (military service) |
| islam | Securitization (0.45) | 테러 (terrorism) |
| black | Criminalization (0.70) | imported Western bias |

**4. Locally generated vs. imported frames**  
Some frames are uniquely Korean — military service 
exemption (군대), 한남 (hannam), North Korea references 
in political attacks. Others, like criminalization of Black 
targets (0.70), are imported through global media despite 
Korea's small Black population — showing prejudice 
can transmit culturally without direct social experience.

**5. Structure and language converge**  
Q2 network clusters and Q3 framing strategies tell the 
same story:
- Ideology cluster → pathology framing
- Nationality cluster → outsider framing  
- Identity cluster → role stereotype + securitization


## Tech Stack
- Python, NetworkX, Pandas, Matplotlib
- Dataset: KOLD (Jeong et al., 2022)

## Cross-linguistic Context
Conducted in collaboration with peers analyzing 
Italian and Sinhala offensive language datasets, 
enabling structural comparison across language contexts.
