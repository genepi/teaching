## Mapping

     bwa index /opt/bma-data/reference/kiv2_6.fasta

     bwa mem /opt/data/reference/kiv2_6.fasta /opt/bma-data/fastq/4153_S13_L001_R1_001.fastq.gz > aligned-file.sam

     samtools sort aligned-file.sam > aligned-file.bam
     
## View BAM File

    samtools view /opt/bma-data/bam/aligned.bam
    samtools sort kiv2.bam > kiv2_sorted.bam
