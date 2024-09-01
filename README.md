# bioinformation

trimmomatic PE -threads 10 \
C1_R1.fq C1_R2.fq \
../clean_data/C1_paired_clean_R1.fq.gz ../clean_data/C1_unpair_clean_R1.fq.gz ../clean_data/C1_paired_clean_R2.fq.gz ../clean_data/C1_unpair_clean_R2.fq.gz \ 
ILLUMINACLIP:home/.conda/pkgs/trimmomatic-0.39-hdfd78af_2/share/trimmomatic-0.39-2/adapters/TruSeq3-PE-2.fa:2:30:10:1:true \
LEADING:3 TRAILING:3 \
SLIDINGWINDOW:4:20 MINLEN:36 TOPHRED33
