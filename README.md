# rust-fastp

- rustic version of fastp each fastp subcommand in a separate multithreaded application
- this part implements the read sync for the fastp. 
- making each part multihreaded using rayon. 

```
cargo build
```
- to check the order
```
./target/debug/rust-fastp ./sample-files/ordered-files/samp2_L001_R1_001.fastq 
./sample-files/ordered-files/samp2_L001_R2_001.fastq
```
- on unordered files 
```
./target/debug/rust-fastp ./sample-files/ordered-files/unamp2_L001_R1_001.fastq 
./sample-files/unordered-files/samp2_L001_R2_001.fastq
```
Gaurav Sablok
