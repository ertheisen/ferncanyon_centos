# appalachian.hg19v1 container for early NGS pipeline applications
How to run pipeline:

 singularity run --app [appname] --bind [directory_info] container_name.simg

Path to genome in container needs to be:
 '/genomes/test/Sequence/Bowtie2Index/genome'
-or-
 '/genomes/spike/dm6/Sequence/Bowtie2Index/genome'
-or-
 '/genomes/spike/sacCer3/Sequence/Bowtie2Index/genome'
-or-
 '/genomes/STAR/[STAR index files]'
-or-
 '/genomes/anno/[gtf or gff annotation file]'

For Baker Cluster Users:
 directory to mount for fly spike-in is: /gpfs0/home/gdlessnicklab/share/trails/genomes/Drosophila_melanogaster/UCSC
 directory to mount for yeast spike-in is: /gpfs0/home/gdlessnicklab/share/trails/genomes/Saccharomyces_cerevisiae/UCSC
 directory to mount for hg19 is: /reference/homo_sapiens/hg19/ucsc_assembly/illumina_download/

To run interactive terminal in container

 singularity shell --bind [directory_info] appalachian_hg19.simg

 ##Be sure to bind your data, your genome, and any script files you may want to run


