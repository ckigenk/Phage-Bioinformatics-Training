# VIRIDIC
VIRIDIC (Virus Intergenomic Distance Calculator) computes pairwise intergenomic distances/similarities amongst viral genomes. 
### Step 1: Create directory and cd into it
```
mkdir viridic_analysis
cd viridic_analysis
```
### Step 2: Download Viridic software
```
wget https://rhea.icbm.uni-oldenburg.de/shiny/VIRIDIC04/session/15d99fa79893cc3fb1d5317303d06170/download/Down_standAlone?w=
```
### Step 3: Extract the file
```
tar -xvf viridic_singularity_v1.1.tar.gz
```
### Step 4: Navigate to the viridic software folder
```
cd viridic
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
### Step 7: Run Viridic 
```
./viridic.bash projdir=Enterococcus_phages in=test_data/combined.fasta ncor=10
```


