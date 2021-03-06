

```
Usage    :
    ./build_trio_kmers.sh [OPTION]

Build trio-binning-kmers based on paternal and maternal NGS reads by jellyfish.

Options  :
        --paternal    paternal NGS reads file in FASTA/FASTQ format.
                      file in gzip format can be accepted, but filename must end by ".gz".
        --maternal    maternal NGS reads file in FASTA/FASTQ format.
                      file in gzip format can be accepted, but filename must end by ".gz".
        --thread      thread number.
                      [ optional, default 8 threads. ]
        --size        initial hash table by jellyfish.
                      [ optional, default 10GB. ]
        --mer         mer-size
                      [ optional, default 21. ]
        --m-lower     maternal kmer frequency table will ignore kmers with count < m-lower.
                      [ optional, default 9. ]
        --m-upper     maternal kmer frequency table will ignore kmers with count > m-upper.
                      [ optional, default 33. ]
        --p-lower     paternal kmer frequency table will ignore kmers with count < p-lower.
                      [ optional, default 9. ]
        --p-upper     paternal kmer frequency table will ignore kmers with count > p-upper.
                      [ optional, default 33. ]
        --auto_bounds automatically calcuate lower and upper bounds based on kmer analysis.
                      [ optional, default not trigger; no parameter. ]
                      ( note : if auto_bounds is on, it will overwrite --*-lower and --*-upper  ]
                      ( !!! WARN : default bounds is seted for 30X WGS reads , if your data is not close to 30X, please use your own bounds or simply open auto_bound
s !!! )
```


