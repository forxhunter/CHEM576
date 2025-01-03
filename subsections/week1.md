# Week1 Contents

[toc]

## 1. Web Resources and Databases

### **1.1 UNIPROT (Universal Protein Resource)**

 **URL** : [https://www.uniprot.org](https://www.uniprot.org/)

* **Purpose** : Comprehensive resource for protein sequence and functional annotation.
* **Key Components** :
* **SwissProt** : Manually reviewed, high-quality protein sequences with functional annotations.
* **TrEMBL** : Automatically annotated protein sequences, updated frequently.
* **Features** :
* Protein function, domains, post-translational modifications, and interaction data.
* Supports BLAST and sequence alignment searches.

### **1.2 SWISSPROT**

 **URL** : [https://www.uniprot.org](https://www.uniprot.org/) (part of UniProt)

* Subset of UniProt containing reviewed protein sequences.
* Prioritized for high-quality, experimentally validated annotations.

### **1.3 PDB (Protein Data Bank)**

 **URL** : [https://www.rcsb.org](https://www.rcsb.org/)

* **Purpose** : Repository of 3D structural data for biological macromolecules.
* **Key Features** :
* Structures determined using X-ray crystallography, NMR, and cryo-electron microscopy (cryo-EM).
* Formats: `.pdb`, `.cif`, and `.mtz` files.
* **Applications** :
* Structure-based drug design, protein-ligand interaction analysis, and homology modeling.

### **1.4 SCOP (Structural Classification of Proteins)**

 **URL** : [http://scop.mrc-lmb.cam.ac.uk](http://scop.mrc-lmb.cam.ac.uk/)

* **Purpose** : Classifies proteins hierarchically based on structural and evolutionary relationships.
* **Hierarchy Levels** :
* **Class** : Overall secondary structure composition.
* **Fold** : Core structural arrangement.
* **Superfamily** : Evolutionarily related families.
* **Family** : Closely related proteins with significant sequence similarity.

### **1.5 CATH (Class, Architecture, Topology, Homologous Superfamily)**

 **URL** : [https://www.cathdb.info](https://www.cathdb.info/)

* **Purpose** : Protein structure classification database.
* **Key Attributes** :
* Uses domain-based classification for protein folds.
* Facilitates comparisons of protein architectures and homologous relationships.

### **1.6 NCBI (National Center for Biotechnology Information)**

 **URL** : [https://www.ncbi.nlm.nih.gov](https://www.ncbi.nlm.nih.gov/)

* **Key Resources** :
* **GenBank** : Repository of nucleotide sequences.
* **BLAST (Basic Local Alignment Search Tool)** : For sequence similarity searches ([BLAST tool](https://blast.ncbi.nlm.nih.gov/)).
* **PubMed** : Literature resource for biomedical research articles ([PubMed](https://pubmed.ncbi.nlm.nih.gov/)).

### **1.7 KEGG (Kyoto Encyclopedia of Genes and Genomes)**

 **URL** : [https://www.genome.jp/kegg](https://www.genome.jp/kegg)

* **Purpose** : Resource for linking genomes to biological functions.
* **Key Databases** :
* **KEGG PATHWAY** : Molecular interaction and pathway maps.
* **KEGG GENES** : Annotated genes from various organisms.
* **KEGG ENZYME** : Data on enzymatic functions and metabolic roles.

### **1.8 YEASTbook**

 **URL** : [https://www.yeastgenome.org](https://www.yeastgenome.org/)

* **Purpose** : Resource for research on *Saccharomyces cerevisiae* (baker’s yeast).
* **Features** :
* Genome annotation and genetic regulatory network data.
* Detailed information on yeast genes and their functional roles in cellular processes.

### **1.9 BRENDA (The Comprehensive Enzyme Database)**

 **URL** : [https://www.brenda-enzymes.org](https://www.brenda-enzymes.org/)

* **Purpose** : Enzyme-specific database with data on enzymatic reactions.
* **Key Features** :
* Information on substrates, cofactors, inhibitors, and reaction kinetics.
* Pathway data integration to support metabolic engineering and systems biology.

---

## **2. Deep Learning Neural Networks (NN)**

**Neural Networks (NNs)** :

* Deep learning architectures for biological sequence and structure analysis.
* Typical layers:
  * **Input Layer** : Takes biological sequence data (DNA/protein sequences).
  * **Hidden Layers** : Perform computations using activation functions (ReLU, Sigmoid).
  * **Output Layer** : Predicts properties (e.g., structure, binding sites).
* **Example Applications** :
* **AlphaFold** : Predicts protein structures from sequences.
* **DeepSEA** : Predicts regulatory effects of genomic variants.
* **Libraries** :
  * PyTorch ([https://pytorch.org](https://pytorch.org/))

---

## **3. Sequence/Structure Alignment Algorithms**

### **3.1 Smith-Waterman Algorithm**

 **Purpose** : Performs local sequence alignment.

* **Characteristics** :
* Uses dynamic programming to find the best local alignment.
* Works with substitution matrices (e.g., BLOSUM, PAM) to score matches.
* Particularly useful for detecting conserved motifs within large sequences.

 **References** :

* Smith-Waterman (original publication): [DOI link](https://doi.org/10.1016/0022-2836(81)90087-5)

### **3.2 STAMP (Structural Alignment of Multiple Proteins)**

 **URL** : [https://www.compbio.dundee.ac.uk/manuals/stamp](https://www.compbio.dundee.ac.uk/manuals/stamp)

* **Purpose** : Aligns protein structures based on 3D conformation.
* **Applications** :
* Identifies structural similarities and evolutionary conservation.
* Provides superposition files for visualization.

---

## **4. Visualization Tools**

### **4.1 VMD (Visual Molecular Dynamics)**

 **URL** : [https://www.ks.uiuc.edu/Research/vmd](https://www.ks.uiuc.edu/Research/vmd)

* **Purpose** : A molecular visualization program used for viewing molecular dynamics simulations.
* **Key Features** :
* Reads `.pdb`, `.gro`, and simulation trajectory files.
* Can display molecular surfaces, secondary structures, and molecular bonds.
* **Uses** :
* Visualization of protein-ligand interactions.
* Rendering of molecular movies for presentations.

### **4.2 MultiSeq (VMD Extension)**

* **Purpose** : An extension for VMD that enables sequence and structure alignments.
* **Features** :
* Generates conservation maps from aligned structures.
* Helps visualize evolutionary patterns and functional sites.

---

## **5. Biopython (Python Library for Bioinformatics)**

 **URL** : [https://biopython.org](https://biopython.org/)

* **Purpose** : Provides tools for handling biological data in Python.
* **Key Functionalities** :
* **Sequence Parsing** : Read/write sequence files (.fasta, .genbank).
* **PDB Parser** : Extract atomic coordinates from PDB files for downstream analysis.
* **Alignment** : Perform pairwise and multiple sequence alignments programmatically.

 **Code Example** :

```python
from Bio import SeqIO

# Reading a FASTA file
for seq_record in SeqIO.parse("example.fasta", "fasta"):
    print(f"ID: {seq_record.id}")
    print(f"Sequence: {seq_record.seq}")
```

---

## **Conclusion**

These web resources, databases, and algorithms form the foundation for computational analysis of protein and nucleotide sequences, structural modeling, and biological pathway analysis. Visualization tools like VMD enhance understanding of macromolecular structures, while programming libraries like Biopython enable reproducible, automated workflows.
