## Assignment 02: Genome Exploration II ##

Species: *Ginglymostoma cirratum* (nurse shark)
Assembly Accession: GCA_024137785.1
Objective: Evaluate the assembly quality, contiguity, sequence-length structure, and open reading frames (ORFs) composition of a whole genome using Galaxy bioinformatic tools.

## Tools & Parameters Used ##

**FASTA Statistics**:Summarizes overall genome assembly metrics, such as total sequence length, base count, GC content, and N50/L50 contiguity values.
**Compute Sequence Length**:Measures and lists the precise length (in base pairs) for each individual sequence or contig in a FASTA file.
**Filter Sequences By Length**:Filters the FASTA file to include only sequences within specified minimum or maximum length bounds.
**EMBOSS getorf**:Extracts open reading frames (ORFs) from nucleotide sequences to identify potential protein-coding regions.
> Minimum size: 300 bp (100 amino acids)
> What to output: Translation of regions between START and STOP codons.

## Biological Interpretation ##

The *Ginglymostoma cirratum* (nurse shark) genome assembly represents a large, complex eukaryotic genome displaying exceptionally high macro-contiguity at the scaffold level, despite underlying contig fragmentation. With a total scaffold length of 4.36 Gb (2.47 Gb ungapped) and only 289 scaffolds, the assembly achieves a high Scaffold N50 of 40.37 Mb and an L50 of 38, demonstrating that half of the total sequence spans just 38 massive scaffolds. Furthermore, the maximum sequence length of 96.6 Mb indicates that the largest scaffolds likely represent near-complete chromosome arms or intact chromosomes. Applying a ≥10 kb length filter removed zero sequences, proving that short contigs do not contribute to the scaffold-level layout, as the smallest scaffold starts at over 100 kb. The biological GC content of 41.63% falls within the normal baseline range for vertebrates, indicating unbiased base composition. Finally, the ORF exploration on a 100 kb slice revealed 127 candidate open reading frames, with the longest reaching 1,473 bp. While this highlights potential coding potential, it also illustrates a key limitation: an ORF only represents a stop-codon-free translation window and cannot be classified as a functional gene without orthogonal evidence such as RNA-seq transcripts, protein homology, or experimental validation.

## Tables ##

<img width="680" height="158" alt="image" src="https://github.com/user-attachments/assets/2a19c811-b3a3-4137-8f36-7d1ecf622ab4" />

*Table 1.* Genome Identity

<img width="702" height="295" alt="image" src="https://github.com/user-attachments/assets/78129205-6c5d-4f40-84a7-b104081b38f4" />

*Table 2.* Containing the main statistical values

<img width="682" height="390" alt="image" src="https://github.com/user-attachments/assets/6be3f96a-49ee-4764-90a5-91191735c1ec" />

*Table 3.* Ranking the longest sequence length using the tool compute the sequence length

<img width="677" height="154" alt="image" src="https://github.com/user-attachments/assets/16295278-b4d8-47a3-b9f9-319128af0153" />

*Table 4.* After applying the tool Filter sequences by length and Fasta statistic if there will be changes in its length after using these tools.

## Screenshots ##

<img width="1362" height="612" alt="image" src="https://github.com/user-attachments/assets/ec47b330-2f39-4f13-8630-6421b51be39c" />

*Figure 1.* Galaxy interface showing the preview of the imported genome FASTA dataset containing nucleotide sequences for the nurse shark assembly

<img width="1366" height="607" alt="image" src="https://github.com/user-attachments/assets/db04f8c2-1bd1-4866-9ff3-cdca7e740f31" />

*Figure 2.* Galaxy interface showing the statistical data using the  tool Fasta Statistics

<img width="608" height="424" alt="image" src="https://github.com/user-attachments/assets/ca598845-fc61-4185-abd7-53cb577c8f85" />

*Figure 3.* Genome Assembly Sequence Length Distribution

## Galaxy Reproducibility and Workflow ##

Workflow Link: https://usegalaxy.org/published/workflow?id=0dc4c974bfa79974

Platform:UseGalaxy.org

Description:Thia workflow shows all the automated steps executed in Galaxy for the *Ginglymostoma cirratum* genome assembly exploration, length filtering, and ORFs analysis.



