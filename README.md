# Erdős Problem #614: a Turán-type reformulation

This repository contains a short note and computational code related to **Erdős Problem #614** (see the Erdős Problems website).

## Contents

- `notes/erdos614_note.pdf`  
  A self-contained note describing the Turán reformulation and related observations.

- `code/compute_Fkmin.nb`  
  Mathematica notebook that computes \(\mathcal F_k^{\min}\) for a given \(k\) using graph6 input.

- `data/graph6/graph3.g6` … `graph9.g6`  
  graph6 files containing (non-isomorphic) simple graphs on 4–9 vertices, used by the notebook.

## How to run the code

1. Open `code/compute_Fkmin.nb` in Mathematica.
2. Set `k` (so the required graph size is \(m=k+2\)).
3. The notebook loads the corresponding `data/graph6/graph<m>.g6` file and outputs:
   - the family \(\mathcal F_k^{\min}\) as Graph objects, and
   - their `Graph6` encodings (for easy reuse).

### Dependency note

The notebook assumes the directory layout in this repository and loads graph6 files via a **relative path**:
`../data/graph6/graph<m>.g6`.



