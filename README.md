# CIDGOH training materials

This repository collects the CIDGOH training materials about genomics data analysis.

## Index of the Material

- Genomics data analysis (@azmigueldario)
  - [raw sequencing reads processing](genomics_data_analysis/raw_reads_processing.ipynb)
  - [Genome assembly and quality control of assembly](genomics_data_analysis/genome_assembly.ipynb)
  - [Annotation of genomes](genomics_data_analysis/annotation_genomes.ipynb)
- cg-MLST analysis (@jimmyliu1326)

## Genomics data analysis tutorials

Jupyter notebooks with tutorials for bioinformatics training in the Center for Infectious Diseases Genomics and One Health. Each notebook is executable in the institution cluster and reproduces common steps in most bacterial genomic analysis pipelines. It includes links to further references and training material.

Common processes in the group for microbial genomics isolate analysis include:

1. Quality control and filtering of raw reads
    - Appraisal of quality in sequencing results
    - Filtering of low quality regions
    - Trimming adapter sessions
    - Visualization of quality control
2. Assembly of draft genome
    - De-novo assembly (polishing of final fasta files)
    - Appraisal of quality in the resulting assembly
3. Genome annotation and downstream analysis
    - Annotation of genomic features using comprehensive databases
    - Define a matrix of genomic distances (SNP)
    - Produce a phylogenetic tree

### Set up for tutorials

They can be executed directly by accessing the web interface of the seagull cluster at <https://seagull.cidgoh.ca/>.

Open up a terminal inside Jupyter and run the following command to copy all the necessary files into your home directory. Everything else, including tools and data, should be easily accessible once you start to execute the tutorial notebooks.

```sh

```

### Troubleshooting - common issues

If by any chance, you cannot find a bash kernel (interpreter for shell command line in jupyter), you can quickly create one for your own use.

First, open a terminal inside **Seagull** and run the following commands to create a virtual environment and install the bash_kernel inside

```sh
conda create -n bash_kernel
conda activate bash_kernel
pip3 install -m bash_kernel
python3 -m bash_kernel.install
conda deactivate
```

Then, in the Jupyter notebook interface, you should be able to choose **bash** as your kernel and run your notebook tutorial.
