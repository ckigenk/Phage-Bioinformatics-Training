## PhageTerm
### Download test datasets
```
wget test_data.tar https://github.com/ckigenk/Phage-Bioinformatics-Training/raw/refs/heads/main/PhageTerm/test_data.tar
```
### Extract the file
```
tar -xcvf test_data.tar
```
### Activate phageterm
```
conda activate phageterm
```
### Run phageterm
```
ptv-py3_release_1_light/PhageTerm.py -f test_data/COS-3.fastq -r test_data/COS-3.fasta --report_title cohesive -c 20
```
