# graybuck2019_scatacseq_pipeline

This single cell ATAC-seq pipeline includes a set of tools necessary for pre-processing ATAC-Seq libraries prepared as in (Graybuck et. al 2019). 

This pipeline adapted from following study: [Paper](https://www.sciencedirect.com/science/article/pii/S0896627321001598?via%3Dihub),  [Code](https://github.com/AllenInstitute/graybuck2019analysis/) and [Data](https://assets.nemoarchive.org/dat-7qjdj84)

##### Steps:
  1. Trim Galore tool is used to remove adapters from reads. 
  2. Trimmed and untrimmed reads are aligned to the reference using Bowtie
  3. Duplicates reads are deleted using Samtools. 
  4. MACS2 is used for calling peaks within ATAC-Seq reads.
  5. ChipSeeker package (R) is incorporated to annotate peaks. 

##### Pipeline Container:
  * Docker: amanukyan1385/graybuck2019\_scatacseq\_pipeline:latest
