# Companion Animals are Spillover Hosts of the Multidrug-Resistant Human Extraintestinal *Escherichia coli* Pandemic Clones ST131 and ST1193
This repository provides *de novo* assemblies of paired-end short-read sequencing data for our phylogenomic study of *E. coli* sequence type (ST)131 in an accessible format. If you use this data in your publications please cite:

```
Kidsley AK^, White RT, Beatson SA, Saputra S, Schembri MA, Gordon D, Johnson JR, O'Dea M, 
Mollinger JL, Abraham S*,Trott DJ*. Companion animals are spillover hosts of the 
multidrug-resistant human extraintestinal Escherichia coli pandemic clones ST131 and ST1193.
Frontiers in Microbiology, (in press).

^CORRESPONDING AUTHORS *AUTHORS CONTRIBUTED EQUALLY

AKK performed experiments, data analysis, drafted & prepared the manuscript. RTW performed 
whole genome sequencing & built/analysed the phylogenetic tree. 
```

The Illumina sequence read data have been submitted to the National Center for Biotechnology Information (NCBI) Sequence Read Archive (SRA) under BioProject [PRJNA627752](https://dataview.ncbi.nlm.nih.gov/object/PRJNA627752?reviewer=81pm20s9n7mj2kku719fs34ein) (20 paired reads).

## Manifest
Contains:
- Assemblies/ - the assembled contigs from Velvet that have been ordered against *E. coli* ST131 strain EC958 (GenBank: [HG941718.1](https://www.ncbi.nlm.nih.gov/nuccore/HG941718.1)) described by [Forde *et al.* (2014)](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4134206/).
  - Contigs from the draft assemblies were ordered against the complete chromosome of EC958 using [Mauve](http://darlinglab.org/mauve/mauve.html) by [Darling, *et al*. (2004)](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC442156/).
- The assembly statistics are provided.

## Matching the SRA accession to strain identifier

The following table facilitates this:

| Strain | Alternate ID | SRA Accession | BioSample accession |
| :---         |          ---: |          ---: |          ---: |
| MS10667 | Q13/1/80 | SRR11608173 | SAMN14686254 |
| MS10669 | W13/1/13 | SRR11608172 | SAMN14686255 |
| MS10670 | N13/1/75 | SRR11608161 | SAMN14686256 |
| MS10671 | N13/1/109 | SRR11608160 | SAMN14686257 |
| MS10672 | N13/4/38 | SRR11608159 | SAMN14686258 |
| MS10673 | N13/1/351 | SRR11608158 | SAMN14686259 |
| MS10674 | S13/1/53 | SRR11608157 | SAMN14686260 |
| MS10675 | N13/4/125 | SRR11608156 | SAMN14686261 |
| MS10677 | N13/4/101 | SRR11608155 | SAMN14686262 |
| MS10678 | N13/1/272 | SRR11608154 | SAMN14686263 |
| MS10893 | 2338849 | SRR11608171 | SAMN14686264 |
| MS10895 | 4209016 | SRR11608170 | SAMN14686265 |
| MS10898 | 2306405 | SRR11608169 | SAMN14686266 |
| MS10899 | 2400728-Feline | SRR11608168 | SAMN14686267 |
| MS10900 | 4180360 | SRR11608167 | SAMN14686268 |
| MS10901 | B08/0924 | SRR11608166 | SAMN14686269 |
| MS10902 | MU1 | SRR11608165 | SAMN14686270 |
| MS10903 | MU4 | SRR11608164 | SAMN14686271 |
| MS10908 | 2435694 | SRR11608163 | SAMN14686272 |
| Q13/1/261 | Q13/1/261 | SRR11608162 | SAMN14686315 |

## Getting the data
Note: The data is ~102.4 MB

**Option 1) Download the current release as an archive:**
```
$ wget https://github.com/RhysWhite/ST131_19_Pets/archive/master.zip -O ST131_19_Pets_v1.tar.gz
$ unzip ST131_19_Pets_v1.tar.gz
```

**Option 2) Clone the current master branch in this repository:**

Please ensure you have git installed. git can be really useful for scientists. See [here](http://blogs.biomedcentral.com/bmcblog/2013/02/28/version-control-for-scientific-research/) for some discussion.

With git:

```
$ git clone --recursive https://github.com/RhysWhite/ST131_19_Pets.git 
# The --recursive option is used to pull down all the smaller repositories
```

