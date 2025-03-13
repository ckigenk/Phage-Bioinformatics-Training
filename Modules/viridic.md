# VIRIDIC
VIRIDIC (Virus Intergenomic Distance Calculator) computes pairwise intergenomic distances/similarities amongst viral genomes. 
![image](https://github.com/user-attachments/assets/a5197f9b-55b2-4e37-a019-e4ce5db072ba)

### Step 1: Create directory and cd into it
```
mkdir viridic_analysis
cd viridic_analysis
```
### Step 2: Download Viridic software
```
wget https://rhea.icbm.uni-oldenburg.de/shiny/VIRIDIC02/session/d811cf1c5c8b10d972ec8ef6555c6fe0/download/Down_standAlone?w=
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
### Step 7: Create project directory
We are analyzing Enterococcus phages
```
mkdir Enterococcus_phages
```
### Step 8: Combined the fasta files and save in project directory
```
cat test_data/*.fasta > Enterococcus_phages/combined_enterococcus_phages.fasta
```
### Step 9: Give permissions to viridic.bash
```
chmod 777 viridic.bash
```
### Step 10: Run Viridic 
```
./viridic.bash projdir=Enterococcus_phages in=Enterococcus_phages/combined_enterococcus_phages.fasta ncor=16
```


