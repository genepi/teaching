# NGS QC Commands

## FastQC Commands

    cd /home/[your_user]/
    mkdir fastqc_report
    ls –lh 
    /opt/tools/FastQC/fastqc /opt/bma-data/fastq/*.fastq.gz --outdir=/home/[your_user]/fastqc_report/
    ls /home/[your_user]/fastqc_report/
    
## FastQC Commands Advanced

    zcat /opt/bma-data/fastq/4*R1*.fastq.gz > merged_R1.fastq
    zcat /opt/bma-data/fastq/4*R2*.fastq.gz > merged_R2.fastq
    mkdir fastqc_report/merged
    /opt/tools/FastQC/fastqc merged_R1.fastq --outdir=./fastqc_report/merged
    /opt/tools/FastQC/fastqc merged_R2.fastq --outdir=./fastqc_report/merged
    
## MultiQC

    cd /home/[your_user]/fastqc_report/
    ls -lh
    multiqc /home/[your_user]/fastqc_report/
    cd ..
