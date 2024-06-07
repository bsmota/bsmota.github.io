## Required files and packages

## Two example high-coverage ancient genomes

**RISE1159 (4726-4830 ypb, Poland):** ancient genome (27.5x) from Schroeder et al., *PNAS* 2019 (https://doi.org/10.1073/pnas.1820210116) and Sousa da Mota et al., *Nat Comm* 2023 (https://doi.org/10.1038/s41467-023-39202-0)

**Yana (30950-32950 ybp, Siberia):** ancient genome (26.5x) from Sikora et al., Nature 2019  (https://doi.org/10.1038/s41586-019-1279-z)
```
# RISE1159
wget ftp://ftp.sra.ebi.ac.uk/vol1/run/ERR112/ERR11270548/RISE1159.bam
samtools index RISE1159.bam

#Extract chromosome 20 
samtools view RISE1159.bam 20 -b > RISE1159.chr20.bam
samtools index RISE1159.chr20.bam

# Yana
wget ftp://ftp.sra.ebi.ac.uk/vol1/run/ERR335/ERR3350997/Yana_old.sort.rmdup.realign.md.bam
samtools index Yana_old.sort.rmdup.realign.md.bam

#Extract chromosome 20 
samtools view Yana_old.sort.rmdup.realign.md.bam 20 -b > Yana.chr20.bam
samtools index Yana.chr20.bam

```
