**Shark Phylogenetic Analysis**

**Course**: Cell and Molecular Biology Laboratory 

**Group Number**: 2

**Members**:

Abrasaldo, Gaze Everly
Dael, Ann Marielle
Romano, Dave Lister
Tuble, Isabella
Villegas, Angela 

**Taxonomic Group**: Shark

**Gene Used**: COI

This repository contains the documentation of our phylogenetic analysis conducted using NCBI and Galaxy.

# Project   Overview 

This project investigated the evolutionary relationships among selected shark species using mitochondrial cytochrome c oxidase subunit I (COI) gene sequences obtained from the NCBI database. The sequences were analyzed through the Galaxy bioinformatics platform using multiple sequence alignment (MAFFT) and phylogenetic tree construction (FastTree). An oceanic manta ray (**Mobula birostris*) was included as the outgroup to root the phylogenetic tree. The study aimed to demonstrate how molecular sequence data can be used to infer evolutionary relationships and compare the resulting phylogeny with previously published studies.

# Taxonomic group
**Kingdom**:	Animalia
**Phylum**:	Chordata
**Class**:	Chondrichthyes (Cartilaginous fishes)
**Subclass**:	Elasmobranchii
**Orders Included**:	Carcharhiniformes, Lamniformes, Orectolobiformes
**Families Included**:	Carcharhinidae, Sphyrnidae, Lamnidae, Alopiidae, Ginglymostomatidae, Rhincodontidae
**Genera Included**:	Sphyrna, Negaprion, Ginglymostoma, Galeocerdo, Prionace, Rhincodon, Carcharodon, Alopias
**Species Included**:	**Sphyrna lewini, Negaprion acutidens, Ginglymostoma cirratum, Galeocerdo cuvier, Prionace glauca, Rhincodon typus, Carcharodon carcharias, Alopias pelagicus*
**Outgroup**:	**Mobula birostris* (Kingdom: Animalia; Phylum: Chordata; Class: Chondrichthyes; Order: Myliobatiformes; Family: Mobulidae)

# Methods

**Reconstructing Evolutionary Relationships Using Mitochondrial COX1**

The evolutionary relationships among the selected shark species were reconstructed using mitochondrial cytochrome c oxidase subunit I (COI/COX1) gene sequences. The COI gene was selected because it is a widely used molecular marker for studying evolutionary relationships and species identification due to its relatively slow mutation rate and high level of conservation among animals. By comparing the COI sequences of the selected shark species, their genetic similarities and differences were analyzed to infer their evolutionary history.

**Sequence Retrieval from NCBI**

The mitochondrial COI sequences of eight shark species and one outgroup (**Mobula birostris*) were obtained from the National Center for Biotechnology Information (NCBI) Nucleotide database. Each sequence was downloaded in FASTA format and renamed according to the corresponding organism to facilitate identification during subsequent analyses. These sequences served as the primary dataset for phylogenetic reconstruction.

**Data Preparation in Galaxy**

The downloaded FASTA files were uploaded into the Galaxy bioinformatics platform using the upload tool. After all sequences were imported, they were combined into a single multiFASTA dataset, which is the required input format for multiple sequence alignment and phylogenetic tree construction. This step ensured that all sequences could be analyzed simultaneously using the Galaxy workflow.

**Multiple Sequence Alignment**

Multiple sequence alignment was performed using the MAFFT alignment tool available in Galaxy. The multiFASTA dataset containing all selected sequences was aligned to identify conserved and variable nucleotide positions across the shark species. The resulting alignment was visualized using the Multiple Sequence Alignment and Sequence Logo tools, allowing similarities and sequence variations to be examined before phylogenetic analysis.

**Consensus Sequence Generation**

A consensus sequence was generated from the aligned COI sequences to summarize the conserved and variable nucleotide sites among the selected species. Conserved positions represented nucleotides shared across most sequences, whereas variable positions highlighted genetic differences among species. These variable sites provided important information for distinguishing species and contributed to the inference of their evolutionary relationships.

**Phylogenetic Tree Construction**

The aligned COI sequences were used to construct a phylogenetic tree with the FastTree tool in Galaxy using the maximum-likelihood method. The resulting tree was rooted using **Mobula birostris* as the outgroup to determine the evolutionary relationships among the selected shark species. The generated phylogenetic tree was then visualized in Galaxy, where the branching patterns and branch lengths were examined to interpret genetic divergence and evolutionary relatedness among the taxa.

<img width="720" height="693" alt="057d5f5e-8f68-43d2-b662-f0ee0f9b7792" src="https://github.com/user-attachments/assets/007188e8-5688-4439-a326-fc936069728d" />


**Figure 1.** Galaxy workflow

<img width="550" height="232" alt="762205337_1397514722323714_8332615800813876030_n (1)" src="https://github.com/user-attachments/assets/6d11f02b-e8b5-436f-8f76-6fc18262e9d9" />


**Figure 2.** Consensus sequence

<img width="384" height="360" alt="758706656_1368704648025839_7724202154654968420_n" src="https://github.com/user-attachments/assets/f2460e3b-48e8-4541-a64b-800f15a1960d" />


**Figure 3.** Phylogenetic tree

**Discussion**

The COI gene sequences were highly conserved across the selected shark species, indicating that mitochondrial COI is a stable genetic marker suitable for DNA barcoding and species identification. However, several variable nucleotide positions were detected, providing sufficient genetic variation to distinguish species and construct a phylogenetic tree.

The phylogenetic analysis recovered several closely related groups. **Ginglymostoma cirratum* (nurse shark) and **Rhincodon typus* (whale shark) formed one sister group, while **Carcharodon carcharias* (great white shark) and **Alopias pelagicus* (thresher shark) formed another. Although **Mobula birostris* was designated as the outgroup, it clustered closer to some shark lineages than expected. This unexpected placement may have resulted from the use of only a single mitochondrial gene, limited taxon sampling, sequence quality, or methodological limitations. Therefore, the generated tree should be interpreted as an estimate of evolutionary relationships rather than a definitive species phylogeny.

Comparison with previous studies showed that the overall clustering of several shark species was generally consistent with molecular phylogenetic analyses reported by Naylor et al. (2012). Likewise, the use of the COI gene aligns with Ward et al. (2005), who demonstrated its effectiveness for DNA barcoding of fishes. Nevertheless, both the published literature and this study recognize that analyses based on a single mitochondrial gene may not fully resolve deeper evolutionary relationships. Incorporating additional nuclear or mitochondrial genes, or whole-genome data, would improve phylogenetic accuracy and provide a more comprehensive understanding of shark evolution.

**References**

Naylor, G. J. P., Caira, J. N., Jensen, K., Rosana, K. A. M., White, W. T., & Last, P. R. (2012). A DNA sequence-based approach to the identification of shark and ray species and its implications for global elasmobranch diversity and parasitology. Bulletin of the American Museum of Natural History, 367, 1–262. https://doi.org/10.1206/754.1 

Ward, R. D., Zemlak, T. S., Innes, B. H., Last, P. R., & Hebert, P. D. N. (2005). DNA barcoding Australia's fish species. Philosophical Transactions of the Royal Society B: Biological Sciences, 360(1462), 1847–1857. https://doi.org/10.1098/rstb.2005.1716
