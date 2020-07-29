ST131 Assembly Statistics of 20 Strains
========================================

Methodology
------------

1) Low-quality bases & read-pairs, together with Illumina adaptor sequences, were trimmed from the raw reads using Trimmomatic v0.36 `(Bolger et al., 2014) <https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4103590/>`_ (settings: LEADING:10 TRAILING:10 MINLEN:50 HEADCROP:10). 

2) The average sequence coverage depth was estimated from mapping reads to the complete chromosome of *E. coli* ST131 strain EC958 using SPANDx v3.2 `(Sarovich & Price, 2014) <https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4169827/>`_.

3) Quality-trimmed paired-end reads were *de novo* assembled using the `Microbial Genome Assembler Pipeline (MGAP) <https://github.com/dsarov/MGAP---Microbial-Genome-Assembler-Pipeline>`_.

MGAP implements:
  - Velvet v1.2.10 `(Zerbino & Birney, 2008) <https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2336801/>`_
  - VelvetOptimiser (https://github.com/tseemann/VelvetOptimiser)
  - GapFiller v1.10 `(Boetzer & Pirovano, 2012) <https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3446322/>`_
  - ABACAS v1.3.1 `(Assefa et al., 2009) <https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2712343/>`_ (scaffolds against the chromosome of EC958)
  - IMAGE v2.4 `(Tsai et al., 2010) <https://genomebiology.biomedcentral.com/articles/10.1186/gb-2010-11-4-r41>`_
  - SSPACE v2.0 `(Boetzer et al., 2011) <https://academic.oup.com/bioinformatics/article/27/4/578/197626>`_
  - Pilon v1.22 `(Walker et al., 2014) <https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0112963>`_
  - MIRA v4 `(Chevreux et al., 2004) <https://www.ncbi.nlm.nih.gov/pmc/articles/PMC419793/>`_
  
  4) QUAST v4.5 `(Gurevich et al., 2013) <https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3624806/>`_ assessed the assembly statistics generated from MGAP by comparing each isolate to EC958. 

------------

**Table. Quality control & assembly metrics for 20 Australian isolates:**

========  =========================== ===================  ================== ======= ========
Strain    Estimated coverage (-fold)  No. contigs ≥1kbp    Total length (bp)  GC (%)  N50
========  =========================== ===================  ================== ======= ========
MS10667   102.0                       116                  5,546,001          50.38   230,256
MS10669   180.9                       54                   5,221,408          50.75   235,715
MS10670   184.9                       26                   5,024,015          50.64   332,128
MS10671   189.4                       74                   5,151,974          50.76   247,208
MS10672   155.8                       82                   5,429,515          50.66   208,069
MS10673   130.9                       89                   5,412,603          50.71   226,639
MS10674   111.9                       38                   5,041,008          50.64   303,060
MS10675   108.2                       62                   5,050,511          50.74   192,455
MS10677   113.3                       104                  5,413,093          50.72   156,514
MS10678   98.8                        102                  5,041,402          50.68   191,083
MS10893   140.2                       51                   5,189,766          50.78   235,548
MS10895   178.8                       553                  6,386,927          50.32   52,076
MS10898   182.0                       56                   5,103,730          50.75   340,215
MS10899   132.0                       53                   5,036,376          50.77   245,963
MS10900   191.5                       53                   5,171,835          50.76   235,785
MS10901   160.8                       59                   5,086,896          50.92   229,597
MS10902   149.8                       74                   5,204,970          50.77   229,637
MS10903   184.1                       72                   5,189,747          50.78   370,428
MS10908   208.1                       72                   5,209,506          50.74   222,092
Q13/1/261 141.0                       66                   4,900,997          50.72   222,896
========  =========================== ===================  ================== ======= ========
