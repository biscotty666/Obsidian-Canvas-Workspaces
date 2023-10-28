---
aliases:
---
%%
topic:: [[Occitan]]
related:: 
created:: October 22, 2023
last edit:: `$= moment(dv.current().file.mtime.toString()).format("YYYY-MM-DD")`
type:: diagram
action:: false
%%


# Contents

<h2 class="title-tag-2">Linguistic classification</h2>

^79f20e

```mermaid
flowchart RL

Itl(Italic)
Oc{{Occitan}}
Fr(French)
It(Italian)
Es(Spanish)
Pr(Provencal)
R(Romance)
WR(Western Romance)
OR(Occitano-Romance)
GR(Gallo-Romance)
GI(Northern Italian)
IW(Italo-Western)
Rom(Romanian)
Sar(Sardinian)
CV(Catalan/Valencian)
IR(Iberian Romance)
Ven(Venetian)
Itl --> R
R --> Rom
R --> Sar
Sar <-.-> It
Sar <-.-> Fr
Sar <-.-> Pr
R --> IW
It <-.-> Oc
Fr <-.-> Oc
Es <-.-> Oc
Pr <-.-> Oc
Ven <-.-> It
IW --> WR
IW --> It
WR --> GR
WR --> IR
WR --> Ven
IR --> Es
GR --> OR
GR --> Fr
GR --> Pr
GR --> GI
GR --> Romansch
OR --> Oc
OR --> CV
CV <-.-> Oc

class Oc target
class Itl,OR,GR,R,WR,IW direct
class Fr,It,Pr,Sar,Es,CV indirect
classDef target stroke:#f00,stroke-width:3px
classDef direct stroke:#0f0
classDef indirect stroke:#00f
```


# References