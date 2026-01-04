# Integrative Comparative Proteomic Analysis of Host-Virus Interactions

### 🦠 Project Abstract
SARS-CoV-2 and Influenza A (H1N1) are significant global health threats that rely on host cellular machinery for replication. This project utilizes a **comparative network biology approach** to identify "Conserved Host Factors" (shared targets) and "Bridge Proteins" (functional connectors) between these two distinct viral interactomes. By overcoming significant data bias in public repositories, we prioritized broad-spectrum antiviral targets.

---

## 📸 Key Research Visuals

### 1. The Computational Pipeline
*The methodology involved harmonizing heterogeneous AP-MS datasets, constructing human PPI networks, and performing topological analysis to identify central nodes.*

<div align="center">
  <img src="pipeline.png" width="60%" height="600px" alt="Workflow Diagram">
</div>

<br>

### 2. Results & Validation
*Below: (Top Left) The Venn diagram showing the "data bias" problem. (Top Right) The network graph revealing "Bridge Proteins" in green. (Bottom) Functional enrichment bubbles and the molecular docking validation of TCF12.*

<table width="100%">
  <tr>
    <td width="50%" align="center">
      <b>The Data Bias Problem</b><br>
      <img src="venn_diagram.png" width="100%" alt="Venn Diagram">
    </td>
    <td width="50%" align="center">
      <b>Bridge Protein Network</b><br>
      <img src="bridge_network.png" width="100%" alt="Network Graph">
    </td>
  </tr>
  <tr>
    <td width="50%" align="center">
      <b>Pathway Enrichment</b><br>
      <img src="pathway_enrichment.png" width="100%" alt="Pathway Analysis">
    </td>
    <td width="50%" align="center">
      <b>TCF12 Docking (-6.8 kcal/mol)</b><br>
      <img src="tcf12_docking.png" width="100%" alt="Docking Validation">
    </td>
  </tr>
</table>

---

## 🔬 Key Findings & Data

### A. Conserved Targets (Direct Overlap)
Analysis of high-confidence AP-MS data identified **4 conserved proteins** targeted directly by both viruses:

| Gene Symbol | UniProt ID | Functional Role |
| :--- | :--- | :--- |
| **HOOK1** | Q9UJC3 | Cytoskeletal Transport |
| **MIPOL1** | Q8TD10 | Cytoskeletal Organization |
| **EXOSC8** | Q96B26 | RNA Stability (Exosome Complex) |
| **TCF12** | Q99081 | Transcription Regulation |

### B. Therapeutic Validation (TCF12)
* **Target:** Transcription Factor 12 (TCF12)
* **Docking Score:** **-6.8 kcal/mol** (AutoDock)
* **Interactions:** Stable hydrogen bonds at residues **VAL186** and **SER192**.
* **Drug Potential:** Identified as a novel target not currently exploited by approved antivirals, minimizing resistance risks.

---

## 🛠 Methodology & Tools
* **Data Acquisition:** BioGRID, IntAct, STRING v11.5.
* **Network Construction:** Python (**NetworkX**) for graph theory metrics (Degree Centrality, Betweenness Centrality).
* **Enrichment Analysis:** g:Profiler for GO terms and KEGG pathways.
* **Structural Biology:** **AutoDock Tools** for virtual screening and **PyMOL** for interaction visualization.

---
> **📄 Full Documentation:**
> *The full project thesis is available upon request for interview purposes to protect intellectual property.*
