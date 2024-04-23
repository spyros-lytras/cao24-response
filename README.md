# Cao *et al.* reanalysis

This repository contains code and results for the reanalysis of the data presented in: [The human microbiota is a beneficial reservoir for SARS-CoV-2 mutations](https://journals.asm.org/doi/10.1128/mbio.03187-23) by Cao *et al.* (2024).

Briefly, the authors find that a substantial number of viral mutation fragments (VMF), 
defined as mutated amino acids within SARS-CoV-2 proteins and six flanking amino acids,
have identical matches in bacterial protein sequences. They then conclude that the 
host microbiota is a reservoir for recombination with SARS-CoV-2.

Ultimately, the integration of “VMFs” by the SARS-CoV-2 RdRP from external sources is dependent on the RNA transcript, 
not the protein sequence.

In the [VMFhit_reanalysis.ipynb](VMFhit_reanalysis.ipynb) notebook presented here we download 
the coding sequences of the VMF containing protein hits from Cao *et al.*'s [Table S3](tableS3_spike)
corresponding to 7 amino acid long Spike VMF (the largest category analysed in the paper). By comparing
the nucleotide sequences underlying the VMF hits to the Spike gene nucleotide sequence of different 
SARS-CoV-2 Variants of Concern (VOC) we show that only a single nucleotide motif matches between the hits and the
SARS-CoV-2 sequences. This motif is found in 8 out of the 1,678 protein hits analysed here, representing a mere 0.4%.

File [spikemut_7aahit_CDS.csv](spikemut_7aahit_CDS.csv) contains the nucleotide motifs underlying each VMF protein hit.

File [spikemut_SC2var_CDS.csv](spikemut_SC2var_CDS.csv) contains the SARS-CoV-2 VOC Spike nucleotide motifs underlying each VMF.

*Note that fasta file [sc2_spikes.fas](sc2_spikes.fas) only contains GISAID accessions and the Spike coding sequences need to be redownloaded to rerun the analysis due to GISAID data sharing restrictions.*

