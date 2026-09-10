# Experiment 1: Exploring Biological Databases

## Aim

To familiarize students with the exploration and utilization of various biological databases for information retrieval relevant to bioinformatics research.

---

## Objectives

- To understand the purpose and applications of biological databases.
- To explore different biological databases used in bioinformatics.
- To retrieve nucleotide, protein, pathway, and structural information.
- To understand how biological information is organized and accessed.
- To record relevant accession numbers, sequences, and annotations.

---

## Introduction

Biological databases are organized collections of biological information that can be accessed and analyzed using computational tools.

They contain different types of biological data such as:

- DNA and RNA sequences
- Protein sequences
- Protein structures
- Metabolic pathways
- Gene annotations
- Functional information

In this experiment, four important biological databases were explored:

1. NCBI GenBank
2. UniProt
3. KEGG
4. Protein Data Bank (PDB)

Each database has a different purpose and provides different types of biological information.

---

# Databases Explored

## 1. NCBI GenBank

**Database:** NCBI Nucleotide / GenBank

NCBI GenBank is a nucleotide sequence database that provides DNA and RNA sequence information along with biological annotations.

### Search Performed

**Gene/Protein:** Lysozyme C (LYZ)  
**Organism:** Homo sapiens

### Observations

| Parameter | Observation |
|---|---|
| Database | NCBI GenBank |
| Gene | LYZ |
| Organism | Homo sapiens |
| Accession Number | M19045.1 |
| Molecule Type | mRNA |
| Sequence Length | 1,483 bp |

The GenBank record provided information about the human lysozyme C mRNA sequence, including its accession number, organism, sequence length, and annotations.

### Screenshots

#### NCBI Search

![NCBI Search](./screenshots/01-NCBI-search.png)

#### NCBI Record

![NCBI Record](./screenshots/02-NCBI-record.png)

#### NCBI FASTA Record

![NCBI FASTA Record](./screenshots/03-NCBI-FASTA-record.png)

---

# 2. UniProt

**Database:** UniProt

UniProt is a protein sequence and functional information database. It provides protein sequences along with information about protein function, genes, organisms, and other annotations.

### Search Performed

**Protein:** Lysozyme C  
**Gene:** LYZ  
**Organism:** Homo sapiens

### Observations

| Parameter | Observation |
|---|---|
| Database | UniProt |
| Protein | Lysozyme C |
| Gene | LYZ |
| Organism | Homo sapiens |
| UniProt Accession | P61626 |
| Entry Name | LYSC_HUMAN |
| Sequence Length | 148 aa |
| Entry Status | Reviewed (Swiss-Prot) |
| Protein Evidence | Protein-level evidence |

The UniProt record provided the protein sequence and functional information for human Lysozyme C.

### Screenshots

#### UniProt Search

![UniProt Search](./screenshots/04-UniProt-search.png)

#### UniProt Record

![UniProt Record](./screenshots/05-UniProt-record.png)

#### UniProt FASTA

![UniProt FASTA](./screenshots/06-UniProt-FASTA.png)

---

# 3. KEGG

**Database:** Kyoto Encyclopedia of Genes and Genomes (KEGG)

KEGG is a biological database that provides information about metabolic pathways, molecular functions, genes, proteins, and biological processes.

### Search Performed

**Pathway:** Glycolysis / Gluconeogenesis

### Observations

| Parameter | Observation |
|---|---|
| Database | KEGG |
| Pathway | Glycolysis / Gluconeogenesis |
| Pathway ID | map00010 |
| Category | Metabolism |
| Subcategory | Carbohydrate Metabolism |

The KEGG pathway map was explored to understand how different enzymes and metabolites are connected in the glycolysis and gluconeogenesis pathways.

### Screenshots

#### KEGG Search

![KEGG Search](./screenshots/07-KEGG-search.png)

#### KEGG Record

![KEGG Record](./screenshots/08-KEGG-record.png)

#### KEGG Result

![KEGG Result](./screenshots/09-KEGG-result.png)

---

# 4. Protein Data Bank (PDB)

**Database:** Protein Data Bank (PDB)

The Protein Data Bank contains experimentally determined three-dimensional structures of proteins, nucleic acids, and other biological macromolecules.

### Search Performed

**Structure:** Lysozyme-related protein structure

### Observations

| Parameter | Observation |
|---|---|
| Database | Protein Data Bank |
| PDB ID | 168L |
| Protein | T4 Lysozyme |
| Organism | Tequatrovirus T4 |
| Experimental Method | X-ray Diffraction |
| Resolution | 2.90 Å |

**Note:** The retrieved PDB entry 168L is a structure of T4 lysozyme from *Tequatrovirus T4*. It is recorded here as the structural database observation from the search and is not the structure of human Lysozyme C (LYZ).

### Screenshots

#### PDB Search

![PDB Search](./screenshots/10-PDB-search.png)

#### PDB Record

![PDB Record](./screenshots/11-PDB-Record.png)

#### PDB Structure

![PDB Structure](./screenshots/12-PDB-Structure.png)

---

# Comparison of Biological Databases

| Database | Main Information | Example from Experiment |
|---|---|---|
| NCBI GenBank | Nucleotide sequences | Human LYZ mRNA |
| UniProt | Protein sequences and annotations | Human Lysozyme C |
| KEGG | Biological and metabolic pathways | Glycolysis/Gluconeogenesis |
| PDB | 3D structures of biomolecules | T4 Lysozyme structure |

---

# Result

Different biological databases were successfully explored and used to retrieve biological information.

The following information was obtained:

- Human **LYZ mRNA** sequence from NCBI GenBank.
- Human **Lysozyme C protein** information from UniProt.
- **Glycolysis/Gluconeogenesis pathway** information from KEGG.
- A **T4 lysozyme three-dimensional structure** from PDB.

The experiment demonstrated that different biological databases provide specialized types of biological information useful for bioinformatics research.

---

# Conclusion

The experiment provided practical knowledge about accessing and exploring biological databases.

NCBI GenBank was useful for retrieving nucleotide sequence information, UniProt provided protein sequence and functional information, KEGG provided pathway information, and PDB provided three-dimensional structural information.

These databases are important resources for sequence analysis, functional annotation, structural studies, and other bioinformatics applications.

---

# Tools and Databases Used

- NCBI GenBank
- UniProt
- KEGG
- Protein Data Bank (PDB)

---

# Repository Structure

```text
01-Biological-Databases/
│
├── README.md
│
└── screenshots/
    ├── 01-NCBI-search.png
    ├── 02-NCBI-record.png
    ├── 03-NCBI-FASTA-record.png
    ├── 04-UniProt-search.png
    ├── 05-UniProt-record.png
    ├── 06-UniProt-FASTA.png
    ├── 07-KEGG-search.png
    ├── 08-KEGG-record.png
    ├── 09-KEGG-result.png
    ├── 10-PDB-search.png
    ├── 11-PDB-Record.png
    └── 12-PDB-Structure.png
