# rust-fastp

- rustic version of fastp each fastp subcommand in a separate multithreaded application
- this part implements the read sync for the fastp.
- please see the last commit message and if it says compiled binary then it is completed or else still in development version.

```
cargo build
```
```
╭─gauravsablok@fedora ~/Downloads/rust-fastp-sync-main  
╰─➤  ./rust-fastp -h
Usage: rust-fastp <READS_1_ARG> <READS_2_ARG>

Arguments:
  <READS_1_ARG>  please provide the reads R1 file path
  <READS_2_ARG>  please provide the reads R2 file path

Options:
  -h, --help     Print help
  -V, --version  Print version
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
