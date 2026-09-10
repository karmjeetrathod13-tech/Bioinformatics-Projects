# Experiment 2: PSI-BLAST Analysis of Lysozyme C

## Aim

To utilize Position-Specific Iterative BLAST (PSI-BLAST) to identify homologous protein sequences of a given query protein sequence and analyze their similarity through multiple iterations.

---

## Objectives

- To understand the working principle of PSI-BLAST.
- To retrieve a protein sequence from UniProt.
- To perform a PSI-BLAST search using NCBI.
- To analyze homologous protein sequences obtained during different iterations.
- To compare E-value, percentage identity, and query coverage of the obtained sequences.
- To observe how iterative searching identifies related protein sequences.

---

## Introduction

PSI-BLAST stands for **Position-Specific Iterated BLAST**. It is a sequence similarity searching method used to identify homologous proteins.

Standard BLAST mainly compares a query sequence with database sequences using a general scoring system. PSI-BLAST improves this process by creating a **Position-Specific Scoring Matrix (PSSM)** from the significant matches obtained in the initial search.

The PSSM contains information about which amino acids are conserved at different positions in the protein sequence. This profile is then used in subsequent iterations to identify additional related sequences.

In this experiment, **human Lysozyme C** was used as the query protein for PSI-BLAST analysis.

---

## Query Protein

The query protein was retrieved from the **UniProt Knowledgebase**.

| Parameter | Details |
|---|---|
| Protein | Lysozyme C |
| Gene | LYZ |
| Organism | Homo sapiens (Human) |
| UniProt Accession | P61626 |
| UniProt ID | LYSC_HUMAN |
| Protein Length | 148 amino acids |
| Protein Existence | Evidence at protein level |
| Status | UniProtKB reviewed (Swiss-Prot) |

---

## Query Protein Sequence

The FASTA sequence of human Lysozyme C was obtained from UniProt and used as the query sequence for PSI-BLAST.

The protein sequence contains **148 amino acids**.

### UniProt Protein Record

![UniProt Search](screenshots/01-UniProt-search.png)

### UniProt FASTA Sequence

![UniProt FASTA](screenshots/02-UniProt-FASTA.png)

---

## Principle of PSI-BLAST

PSI-BLAST works through an iterative sequence-searching process.

1. The query protein sequence is searched against a protein database.
2. Significant sequence matches are identified in the first iteration.
3. The significant matches are used to construct a **Position-Specific Scoring Matrix (PSSM)**.
4. The PSSM is used for the next iteration of the search.
5. Additional homologous sequences can be identified in subsequent iterations.
6. The process can be repeated until the search reaches convergence or no substantial new sequences are detected.

Important parameters used to evaluate the results include:

- **E-value:** Indicates the statistical significance of a sequence match. Lower values indicate more significant matches.
- **Percentage Identity:** Indicates the percentage of identical amino acids between the query and the matching sequence.
- **Query Coverage:** Indicates how much of the query sequence is included in the alignment.
- **Score:** Represents the quality of the sequence alignment.

---

## Tools and Database Used

### Tools

- UniProt
- NCBI BLAST
- PSI-BLAST

### Database

- **ClusteredNR (clustered_nr)**

### Input

- Protein FASTA sequence of human Lysozyme C

---

## PSI-BLAST Parameters

The following settings were used in the PSI-BLAST search:

| Parameter | Value |
|---|---|
| Program | PSI-BLAST |
| Query Protein | Lysozyme C |
| Accession | P61626 |
| Organism | Homo sapiens |
| Database | ClusteredNR (clustered_nr) |
| Search Type | Protein-protein BLAST |
| Iterations | 3 |
| Number of Sequences | 500 |

---

## Procedure

### Step 1: Retrieve the Query Protein

The protein **Lysozyme C** was searched in the UniProt database.

The selected UniProt entry was:

**P61626 – LYSC_HUMAN**

The record showed that the protein is Lysozyme C from *Homo sapiens* and contains 148 amino acids.

The FASTA sequence was obtained from the UniProt record.

---

### Step 2: Obtain the FASTA Sequence

The FASTA sequence of Lysozyme C was copied from the UniProt entry.

The sequence was used as the input query for the PSI-BLAST search.

---

### Step 3: Enter the Query Sequence in NCBI BLAST

The Lysozyme C FASTA sequence was entered into the NCBI BLAST protein search interface.

The **PSI-BLAST (Position-Specific Iterated BLAST)** algorithm was selected.

The database displayed in the search interface was **ClusteredNR (clustered_nr)**.

![PSI-BLAST Input](screenshots/03-PSI-BLAST-input.png)

---

# PSI-BLAST Results

## Iteration 1

The first PSI-BLAST iteration produced significant sequence matches to human Lysozyme C.

Several highly similar lysozyme sequences were identified from different organisms.

Some representative results observed were:

| Protein | Organism | Query Coverage | E-value | Percentage Identity |
|---|---|---:|---:|---:|
| Lysozyme C precursor | *Gorilla gorilla gorilla* | 100% | 3e-103 | 99.32% |
| Lysozyme C precursor | *Macaca mulatta* | 100% | 2e-94 | 88.51% |
| Mdc-hly hybrid protein, partial | Synthetic construct | 88% | 1e-91 | 100.00% |
| Predicted Lysozyme C | *Chrysochloris asiatica* | 100% | 1e-91 | 86.49% |
| Lysozyme C | *Taphozous melanopogon* | 100% | 3e-91 | 83.78% |
| Chain A, LYSOZYME | *Homo sapiens* | 88% | 1e-90 | 99.23% |
| c-type lysozyme | *Leptonycteris yerbabuenae* | 100% | 2e-90 | 86.49% |
| Lysozyme C | *Piliocolobus tephrosceles* | 100% | 4e-90 | 82.43% |

The results showed high sequence similarity and strong statistical significance among the major hits.

### Iteration 1 Screenshot

![PSI-BLAST Iteration 1](screenshots/04-PSI-BLAST-iteration%201.png)

---

## Iteration 2

In the second iteration, the PSSM generated from the PSI-BLAST analysis was used to identify related sequences.

The results continued to show highly significant matches with high query coverage and high sequence identity.

Representative results included:

| Protein | Organism | Query Coverage | E-value | Percentage Identity |
|---|---|---:|---:|---:|
| Lysozyme C | *Taphozous melanopogon* | 100% | 2e-116 | 83.78% |
| c-type lysozyme | *Leptonycteris yerbabuenae* | 100% | 2e-116 | 86.49% |
| Predicted Lysozyme C | *Chrysochloris asiatica* | 100% | 8e-115 | 86.49% |
| Lysozyme C precursor | *Macaca mulatta* | 100% | 3e-114 | 88.51% |
| Lysozyme C | *Rhinopoma microphyllum* | 100% | 5e-113 | 80.41% |
| Lysozyme C | *Talpa occidentalis* | 100% | 7e-113 | 81.08% |
| Lysozyme C precursor | *Gorilla gorilla gorilla* | 100% | 1e-112 | 99.32% |
| Predicted Lysozyme C | *Elephantulus edwardii* | 100% | 5e-112 | 78.38% |

The second iteration continued to identify highly conserved Lysozyme C-related sequences.

### Iteration 2 Screenshot

![PSI-BLAST Iteration 2](screenshots/05-PSI-BLAST-iteration%202.png)

---

## Iteration 3

The third PSI-BLAST iteration displayed clustered sequence results representing several organisms.

The results included sequences from groups such as primates, bats, insectivores, rodents, and other mammals.

Representative results observed were:

| Cluster Representative Sequence | Query Coverage | E-value | Percentage Identity |
|---|---:|---:|---:|
| Lysozyme C – *Taphozous melanopogon* | 100% | 6e-115 | 83.78% |
| c-type lysozyme – *Leptonycteris yerbabuenae* | 100% | 2e-114 | 86.49% |
| Predicted Lysozyme C – *Chrysochloris asiatica* | 100% | 1e-112 | 86.49% |
| Lysozyme C precursor – *Macaca mulatta* | 100% | 1e-111 | 88.51% |
| Lysozyme C – *Rhinopoma microphyllum* | 100% | 3e-111 | 80.41% |
| Lysozyme C – *Talpa occidentalis* | 100% | 9e-111 | 81.08% |
| Predicted Lysozyme C – *Elephantulus edwardii* | 100% | 2e-110 | 78.38% |
| Lysozyme C-1 – *Cricetulus griseus* | 100% | 5e-110 | 75.00% |
| Lysozyme C precursor – *Gorilla gorilla gorilla* | 100% | 9e-110 | 99.32% |
| Lysozyme C – *Octodon degus* | 100% | 1e-109 | 83.11% |

The third iteration showed continued detection of strongly conserved Lysozyme C-related sequences.

### Iteration 3 Screenshot

![PSI-BLAST Iteration 3](screenshots/06-PSI-BLAST-iteration%203.png)

---

# Observations

The PSI-BLAST analysis produced significant matches in all three iterations.

### Major observations

- The query protein was **human Lysozyme C (P61626)**.
- The query sequence contained **148 amino acids**.
- The search was performed using **PSI-BLAST**.
- The selected database was **ClusteredNR (clustered_nr)**.
- Three PSI-BLAST iterations were performed.
- Major hits showed **high query coverage**, commonly 100%.
- Many sequences showed **more than 80% sequence identity**.
- Very low E-values were observed for the major hits.
- Lysozyme C-related sequences were identified from several different organisms.
- The results included organisms from groups such as primates, bats, rodents, insectivores, and other mammals.
- The presence of high sequence identity and very low E-values indicates strong similarity between the query protein and the identified sequences.

---

# Analysis of E-value, Identity and Query Coverage

### E-value

The observed E-values were extremely low, for example:

- `3e-103`
- `2e-94`
- `3e-91`
- `2e-116`
- `1e-112`
- `6e-115`

These low E-values indicate that the observed sequence similarities are statistically significant.

### Percentage Identity

The major hits showed high percentage identity.

For example:

- *Gorilla gorilla gorilla*: **99.32%**
- *Macaca mulatta*: **88.51%**
- *Chrysochloris asiatica*: **86.49%**
- *Taphozous melanopogon*: **83.78%**
- *Cricetulus griseus*: **75.00%**

This indicates that Lysozyme C is highly conserved among the analyzed organisms.

### Query Coverage

Most of the major hits showed **100% query coverage**, meaning that the complete 148-amino-acid query protein was covered by the alignment.

---

# Interpretation

The PSI-BLAST results demonstrate that human Lysozyme C has strong sequence similarity with Lysozyme C and related lysozyme proteins from multiple organisms.

The high percentage identities, high query coverage, and very low E-values indicate that these sequences are strongly related to the human Lysozyme C query.

The results obtained across three iterations also demonstrate how PSI-BLAST uses a position-specific profile to continue searching for related sequences.

The presence of conserved Lysozyme C sequences across different organisms suggests that important regions of this protein have been conserved during evolution.

---

# Conserved Domain Analysis

No separate conserved-domain result screenshot was included among the six screenshots provided for this experiment.

Therefore, no specific conserved-domain result is reported in this README.

If a conserved-domain result is obtained later, it can be added as an additional screenshot and observation.

---

# Conclusion

PSI-BLAST analysis was successfully performed using **human Lysozyme C (P61626)** as the query protein.

The three iterations identified numerous highly similar Lysozyme C-related sequences from different organisms. The major hits showed high query coverage, high percentage identity, and very low E-values.

The results demonstrate that Lysozyme C is a highly conserved protein among the organisms identified in the PSI-BLAST search.

This experiment also demonstrated the usefulness of PSI-BLAST for identifying homologous protein sequences through iterative profile-based sequence searching.

---

# Screenshots

The experiment is documented using the following screenshots:

1. **UniProt Protein Search**
   - `01-UniProt-search.png`

2. **UniProt FASTA Sequence**
   - `02-UniProt-FASTA.png`

3. **PSI-BLAST Input**
   - `03-PSI-BLAST-input.png`

4. **PSI-BLAST Iteration 1**
   - `04-PSI-BLAST-iteration 1.png`

5. **PSI-BLAST Iteration 2**
   - `05-PSI-BLAST-iteration 2.png`

6. **PSI-BLAST Iteration 3**
   - `06-PSI-BLAST-iteration 3.png`

---

# Project Structure

```text
02-PSI-BLAST/
│
├── README.md
│
└── screenshots/
    ├── 01-UniProt-search.png
    ├── 02-UniProt-FASTA.png
    ├── 03-PSI-BLAST-input.png
    ├── 04-PSI-BLAST-iteration 1.png
    ├── 05-PSI-BLAST-iteration 2.png
    └── 06-PSI-BLAST-iteration 3.png
