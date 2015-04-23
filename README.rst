Banzai
======

The Banzai Microbial Genomics Pipeline is currently in closed beta. Please 
`star`_ or `follow`_ this repository to receive updates when it's 
publicly available.

.. _`star`: https://github.com/mscook/Banzai-MicrobialGenomics-Pipeline/star

.. _`follow`: https://github.com/mscook/Banzai-MicrobialGenomics-Pipeline/watchers


Installation
------------

See Install.rst_

.. _Install.rst: https://github.com/mscook/Banzai-MicrobialGenomics-Pipeline/blob/master/Install.rst


About
-----

Banzai is a Microbial Genomics Next Generation Sequencing (NGS) Pipeline Tool 
developed within `Dr Scott Beatson's Group`_ at the University of Queensland.

.. _`Dr Scott Beatson's Group`: http://smms-steel.biosci.uq.edu.au

Banzai inherits it's name from the `Banzai 'Pipeline' surf break`_.

.. _`Banzai 'Pipeline' surf break`: http://en.wikipedia.org/wiki/Banzai_Pipeline

Banzai aims to simplify the analysis of large NGS datasets. It has been 
specifically designed to distribute the workload over internal and external 
High Performance Computing (HPC) resources as well as locally available 
workstations.


Core Features
-------------

Banzai allows for:
    * data validation/quality control of NGS reads,
    * de novo assembly of NGS reads,
    * mapping of NGS reads to reference genomes,
    * ordering of the contigs or scaffolds from draft assemblies against 
      reference genomes,
    * phylogenomics tasks (whole genome alignment, SNP based, recombination 
      detection)
    * annotating draft assemblies,
    * enrichment of the annotation of draft assemblies,
    * performing common utility tasks like the creation of BLAST databases, 
      file format conversion and more.

Banzai supports the NGS platforms that are perdominantly used in Microbial 
Genomics projects.

The platforms include:
    * `Illumina`_ (single end (SE), paired end (PE) and mate paired (MP)
      reads),
    * `454`_ (SE and PE reads),
    * `ABI SOLiD`_ colorspace reads and
    * `Pacific Biosciences`_ reads (under development)

.. _`Illumina`: http://www.illumina.com/technology/sequencing_technology.ilmn
.. _`454`: http://www.454.com/
.. _`ABI SOLiD`: http://www.appliedbiosystems.com.au/
.. _`Pacific Biosciences`: http://www.pacificbiosciences.com/

**Banzai is by default geared towards 100 bp Illumina Paired End reads.**


Philosophy
----------

Banzai (in most cases) does not provide new NGS algorithms, it harnesses the 
power of published and tested NGS tools. Simply, Banzai simplifies, automates 
and distributes computational workloads which is the typical bottleneck in 
analysis of large NGS datasets.


Developers
----------

The following have contributed significantly to Banzai:
    * Mitchell Stanton-Cook (lead developer)
    * Elizabeth Skippington (development of phylogenomics section)
    * Nico Petty (design & testing)
    * Nouri Ben Zakour (design and testing)
    * Scott Beatson (design)
