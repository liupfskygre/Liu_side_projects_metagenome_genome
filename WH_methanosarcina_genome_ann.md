#this is a markdown file for the annotation of Methanocarcina mazei zm-15 genomes from Wang and LU@PKU

#Methanocarcina mazei zm-15 is a genome isolated from xx, closely related to Methanosarcina mazei Go1

**EGGnog annotation**

```
cd 
#1. prodigal ORF calling
prodigal -p meta -q -i wh.assembly.fasta -a wh.assembly_prodigal.faa -d wh.assembly_prodigal.fna
# 3714 ORF from prodigal

#2, upload both fna and faa to eggnog mapper for annotation

#3, use rfam to search 16S rRNA
cmsearch  --tblout wh.assembly_prodigal.tbl --cpu 3 --default ~/Rfam_cm_model/Rfam_ba_ar_ssu.cm wh.assembly_prodigal.fna
#no 16S in annotated fna

```
**16S**
```
#//Users/pengfeiliu/Cooperations_Other_Labs_projects/Wang_Hui_Lu_genome/wh.assembly.fasta

barrnap -o wh.assembly_rrna.fa <wh.assembly.fasta> wh.assembly_rrna.gff

```

**dfast annotation**
```
https://dfast.nig.ac.jp/analysis/annotation/dffecb4f-21a7-4184-94f5-5bfa43ed2268

```


**default annotation from company**
```

```
