# VirusDiscoveryProject
Software, architecture, and data index design for the 2018/2019 Virus Discovery Project

## Here we present a compromise pipeline for extracting virological information from publicly available metagenomic datasets, in order to present a usable index to the virological research community.  

# Look at the cool new sh*& NCBI built for us!

## NCBI Blast Docker:

### https://github.com/ncbi/docker/blob/blast2.8.1/blast/README.md

##### Theres also a nice cookbook here, with thanks to @christiam!

### GS Blast dbs

#### BLAST Databases currently being updated to the NIH STRDES GCP bucket (gs://blast-db/)

##### nr, nt, etc.  

##### Virus specific ones!

1. ref_viruses_rep_genomes_v5 
  * Reference Viral sequences
  * Entrez query - “latest_refseq[Prop] AND viruses[Organism]”	

2. ref_viroids_rep_genomes_v5	
  * Reference Viroid Sequences 
  * Entrez Query - “latest_refseq[Prop] AND viroids[Organism]”	

3. NCBI_VIV_protein_sequences_v5	
  * Proteins from coding-complete, genomic viral sequences
  * Equivalent to nr Entrez Query - Viruses[Organism] NOT cellular organisms[ORGN] NOT wgs[PROP] NOT gbdiv syn[prop] AND (srcdb_refseq[PROP] OR nuccore genome samespecies[Filter]) 

4. NCBI_VIV_nucleotide_sequences_v5	
  * Coding-complete, genomic viral sequences
  * Equivalent to nt Entrez Query -	Viruses[Organism] NOT cellular organisms[ORGN] NOT wgs[PROP] NOT gbdiv syn[prop] AND (srcdb_refseq[PROP] OR nuccore genome samespecies[Filter]) 

#### CONTIGS!

##### XXXnumber are available from <>

##### Accessible using SRA toolkit
