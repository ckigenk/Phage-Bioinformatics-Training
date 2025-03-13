# VIRIDIC
VIRIDIC (Virus Intergenomic Distance Calculator) computes pairwise intergenomic distances/similarities amongst viral genomes. 
### Step 1: Create directory and cd into it
```
mkdir viridic_analysis
cd viridic_analysis
```
### Step 2: Download Viridic software
```
wget https://rhea.icbm.uni-oldenburg.de/shiny/VIRIDIC05/session/c7426903cb5ae1c37ef52f5133e217a8/download/Down_standAlone?w=
```
### Step 3: Extract the file
```
tar -xvzf viridic_singularity_v1.1.tar.gz
```
### Step 4: Navigate to the viridic software folder
```
cd  viridic_v1.1
```
### Step 5: Download test dataset
```
wget https://github.com/ckigenk/Phage-Bioinformatics-Training/raw/refs/heads/main/viridic/test_data.tar
```
### Step 6: Extract the file
```
tar -xvf test_data.tar
```
### Step 8: Create project directory
We are analyzing Enterococcus phages
```
mkdir Enterococcus_phages
```
### Step 9: Combined the fasta files and save in project directory
```
cat test_dir/*.fasta Enterococcus_phages/combined_enterococcus_phages.fasta
```
### Step 7: Run Viridic 
```
./viridic.bash projdir=Enterococcus_phages in=test_data/combined.fasta ncor=10
```


