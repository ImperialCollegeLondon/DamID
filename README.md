# DamID
Annotation of DamID sequencing results

This script adds annotation to a GFF file produced through DamID. It makes use of the ensembl API to identify genes in C.elegans close to the loci present in the GFF file. Should the locus be within a gene, the name and description of
this will be added to the GFF annotation field. If the locus is not within a gene, genes within 10kb upstream or downstream will be annotated.

The script is dependent upon the ensembl API, which is tied to specific versions of the ensembl database. This may therefore need to be updated prior to running the script -the version of the ensembl database and genome build in use are reported by the script. These should be compared with the versions on www.ensembl.org to determine if an upgrade is required.

Analysis of different organisms will require the sscript to be modified to change all occurrences of the species name (caenorhabditis_elegans).
