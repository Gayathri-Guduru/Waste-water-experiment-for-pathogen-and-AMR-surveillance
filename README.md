**The goal is to study pathogens of interest in real wastewater samples by spiking them with synthetic reads. 

***Our main focus is to predict the ST’s of Streptococcus pneumoniae. After some research and reading articles, seroBA, PneumoCaT, PneumoKITy, stringMLST, MetaMLST and PyMLST are the widely used tools. I selected SeroBA, stringMLST and MetaMLST as key tools for analysis:
_**SeroBA**_: The first 3 mentioned tools are specific to Streptococcus pneumoniae and there are several github pages that are promising as they claim that the tool works on low coverage levels ~10X and SeroBA can predict serotypes, by identifying the cps locus, directly from raw whole genome sequencing read data. This tool also has the reference databases from PneumoCaT. Therefore, I chose this tool. (seroBA, last updated 2020).
_**stringMLST**_: This is a fast and efficient tool for sequence typing bacterial species. It skips the need for full genome assembly by using a k-mer approach, which means it works directly on raw sequencing data. It’s accurate, works even with lower-quality data, and can handle multiple species. (stringMLST, last updated 2020).
_**MetaMLST**_: This is a tool designed for typing pathogens directly from metagenomic datasets, making it perfect for complex samples like wastewater, soil, or gut microbiomes. Unlike traditional MLST, it works well with mixed microbial communities, identifying specific pathogens and their sequence types (STs) without needing genome assembly. But it needs aligned files as inputs. We can also customize it for specific microbes or loci we’re interested in. (metamlst, last updated 2022).
***_Serocall_***: SeroCall can identify and quantitate the capsular serotypes in Illumina whole-genome sequencing samples of S. pneumoniae, calculating abundances of each serotype in mixed cultures. 

Different experiments were conducted on these tools and the details are mentioned in the powerpoint.

*** The next goal is to predict the emm types of _Streptococcus pyogenes_. The tools that were experimented were emm-typing, emmtyper.
