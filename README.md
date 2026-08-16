# Assignment 02: Genome Exploration

### Species Info
* **Species:** *Felis catus* (Domestic Cat)
* **Accession Number:** GCF_018350175.1
  
### Objective
To evaluate the assembly quality and contiguity of the Felis catus reference genome across length-filtering thresholds, and to characterize Open Reading Frames (ORFs) on an unlocalized genomic scaffold.

### Tools and Parameters Used
1. **Fasta Statistics:** Default settings to compute total length, sequence count, N50, and GC content.
2. **Filter Sequences by Length:** Minimum length cutoff set to 10000 bp (10 kb).
3. **Split Fasta:**Split multi-FASTA file by record to extract target scaffold `chrA2_random_Un_scaffold_64` for manageable ORF processing.
4. **getorf:** Standard genetic code, protein translation output, default minimum size threshold.
5. **Sort Dataset:** Sorted on Column 2 in descending numerical order to rank ORFs by size.

### Genome Interpretation
Analysis of the *Felis catus* assembly metrics reveals a highly contiguous, chromosome-level genome rather than a fragmented one. The N50 value of 148,491,486 bp combined with a maximum scaffold length of 239,367,248 bp indicates that the vast majority of the 2.43 Gb assembly is dominated by massive, near-complete chromosomal sequences. Furthermore, filtering short sequences at the 10 kb threshold resulted in zero removed scaffolds and left the total length entirely unchanged, proving that short, fragmented contigs (<10 kb) are completely absent and contribute nothing to the overall genome size. The assembly exhibits a characteristic mammalian GC content of 41.81%, reflecting balanced base composition across coding and non-coding regions. Finally, the open reading frame (ORF) search identified 155 potential coding regions within a selected scaffold, with the longest spanning 624 amino acids (1,872 bp). While this exercise successfully demonstrated how bioinformatics tools locate translationally uninterrupted stretches between start and stop codons, it also highlighted a critical limitation: an ORF is merely a sequence capability and does not automatically equal a functional gene without supporting transcriptomic or homology data.

### Shared Galaxy History Link
[Paste your shared Galaxy URL here]
