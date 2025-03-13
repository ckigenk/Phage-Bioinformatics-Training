# VIRIDIC
VIRIDIC (Virus Intergenomic Distance Calculator) computes pairwise intergenomic distances/similarities amongst viral genomes. 
### Create directory
```
mkdir viridic_analysis
cd viridic_analysis
```
### Download Viridic software
```
wget https://rhea.icbm.uni-oldenburg.de/shiny/VIRIDIC04/session/15d99fa79893cc3fb1d5317303d06170/download/Down_standAlone?w=
```
### Extract
```
tar -xvf viridic_singularity_v1.1.tar.gz
```
### Navigate to the viridic software folder
```
cd viridic
```
### Download test dataset
```
wget https://github.com/ckigenk/Phage-Bioinformatics-Training/raw/refs/heads/main/viridic/test_data.tar
```
### Extract the file
```
tar -xvf test_data.tar
```
### Run Viridic 
```
viridic.bash viriddi
