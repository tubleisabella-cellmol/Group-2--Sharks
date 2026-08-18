# Assignment 02: Genome Exploration II

Species: *Rhincodon typus* (whale shark)

Assembly Accession: GCA_021869965.2

Objective: Evaluate the assembly quality, contiguity, sequence-length structure, and open reading frames (ORFs) composition of a whole genome using Galaxy bioinformatic tools.

# Tools & Parameters Used
FASTA Statistics: Summarizes overall genome assembly metrics, such as total sequence length, base count, GC content, and N50/L50 contiguity values. 

Compute Sequence Length: Measures and lists the precise length (in base pairs) for each individual sequence or contig in a FASTA file. 

Filter Sequences By Length: Filters the FASTA file to include only sequences within specified minimum or maximum length bounds. 

EMBOSS getorf: Extracts open reading frames (ORFs) from nucleotide sequences to identify potential protein-coding regions.

Minimum size: 213 bp

What to output: Translation of regions between START and STOP codons.

# Biological Interpretation

The *Rhincodon typus* genome assembly appears relatively well assembled and contiguous, as shown by its large scaffold N50 of about 65.4 Mb and L50 of 16. The largest scaffold is approximately 185 Mb, indicating that some genomic regions are contained in very large sequences. Although the assembly contains thousands of scaffolds, removing sequences shorter than 10 kb removed 291 scaffolds but only about 1.1 Mb of sequence, showing that the short scaffolds contribute little to the overall genome size. The genome has a GC content of approximately 42.96%, meaning that G and C bases make up about 43% of the DNA. The ORF analysis demonstrated that genomic DNA can contain sequences with the potential to encode proteins; the selected region contained a 333-bp ORF. However, finding an ORF alone does not confirm that it is a functional gene, so additional evidence such as gene annotation, transcript data, or protein similarity would be needed.

# Tables

# Table 1. *Genome Identity.*
<img width="778" height="248" alt="image" src="https://github.com/user-attachments/assets/f9056078-a51d-4644-9eff-ab1603868c4a" />

# Table 2. *Containing the main statistical values.*
<img width="773" height="335" alt="image" src="https://github.com/user-attachments/assets/60d742b2-56d5-4e6a-9103-808c19824c4e" />

# Table 3. *Ranking the longest sequence length using the tool compute the sequence length.*
<img width="778" height="250" alt="image" src="https://github.com/user-attachments/assets/ed9e0215-6b8c-4d77-ba8c-55f4a6f9b51c" />

# Table 4. *After applying the tool Filter sequences by length and Fasta statistic if there will be changes in its length after using these tools.*
<img width="780" height="247" alt="image" src="https://github.com/user-attachments/assets/a1ee870c-4e5a-48f6-81c2-dfdc162bb2c5" />

# Screenshots

<img width="780" height="375" alt="image" src="https://github.com/user-attachments/assets/16bd1572-716a-4630-98da-ea34d611f744" />

# Figure 1. *Galaxy interface showing a preview of the imported raw genome FASTA dataset (Rhincodon_typus_Genome_Sequences.fasta) containing nucleotide sequences for the whale shark assembly.*

<img width="782" height="398" alt="image" src="https://github.com/user-attachments/assets/a7eaa667-61b6-442a-901c-c27ebb654029" />

# Figure 2. *Galaxy output interface displaying the assembly summary statistics for the original Rhincodon typus genome, detailing metrics such as scaffold N50, total length, sequence count, and GC content.*

# Galaxy Reproducibility and Workflow

Workflow Link: https://usegalaxy.org/u/ann-marielle-dael54/w/rhincodon-typus-genome-sequences 

Platform: UseGalaxy.org

Description: This workflow shows all the automated steps executed in Galaxy for the *Rhincodon typus* genome assembly exploration, length filtering, and ORFs analysis.
