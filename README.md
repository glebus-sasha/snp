# SNP Pipeline

SNP Pipeline is a Nextflow-based pipeline for Single Nucleotide Polymorphism (SNP) calling from genome sequencing data. This pipeline provides streamlined processing from sequencing to annotation, assisting researchers in analyzing genetic variations with minimal effort.

## Features

- Alignment using BWA mem for accurate mapping of sequences to the reference genome.
- Quality control using fastp to remove adapters and low-quality reads.
- Variant calling using mpileup for SNP and indel detection.
- Variant annotation using Variant Effect Predictor (VEP) to identify functional consequences of variations.
- Support for containerization using Singularity, ensuring ease of deployment and management of the execution environment.

## DAG (Directed Acyclic Graph)

![image](https://github.com/glebus-sasha/SNP/assets/28355746/1cfe6c23-228c-4191-92b8-3b8d20e11105)

## Requirements

- Installed Nextflow (https://www.nextflow.io/docs/latest/getstarted.html)
- Installed Singularity (https://docs.sylabs.io/guides/3.0/user-guide/installation.html)
- Resources for analysis: computational power, access to sequencing data.
- Singularity for containerization. Make sure Singularity is installed and accessible in your environment.

## Installation and Execution

1. Install Nextflow by following the instructions on the official website. (https://www.nextflow.io/docs/latest/getstarted.html)

2. Clone the SNP Pipeline repository to your local machine.
```
git clone https://github.com/glebus-sasha/SNP.git
```
3. Navigate to the directory containing the pipeline and execute it using the command `nextflow run SNP.nf`.


## Usage Example

Example command to run the pipeline:

```
nextflow run SNP.nf
```

## Contributors

- Oxana Kolpakova ([@OxanaKolpakova](https://github.com/OxanaKolpakova))
- Glebus Aleksandr ([@glebus-sasha](https://github.com/glebus-sasha/))

## License

SNP Pipeline is distributed under the MIT license. See the LICENSE file for details.
