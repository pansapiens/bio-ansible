# List of available tags

The best way to determine which tags are available for each playbook is to run:

```sh
ansible-playbook --list-tags common.yml
ansible-playbook --list-tags bio.yml
ansible-playbook --list-tags interactive.yml
```

Note that when running tasks via tag(s), role dependencies (in <role>meta/main.yml)
are ignored (unless the dependency also contains that tag).

### Need `sudo`

#### common.yml

- `apt`
- `email`
- `lmod`
- `pip`
- `pip3`
- `r_base`
- `r-extras`
- `r-data`
- `sw_guy`
- `timezone`

#### interactive.yml

- `nginx`
- `rstudio`
- `rstudio_pro`
- `shiny`

### Don't need `sudo`

#### bio.yml

- `java` - the `java_flavour` variable determines Java installation method: 
           *oracle_tarball* (no sudo), *distro* (sudo), *oracle_ppa* (sudo)

- `dirs`

- `bds`
- `bwa`
- `bedtools`
- `cutadapt`
- `fastqc`
- `freebayes`
- `gatk`
- `htslib`
- `igv`
- `mimodd`
- `multiqc`
- `picard`
- `qualimap`
- `rnasik`
- `raxml`
- `samtools`
- `seqtk`
- `sratoolkit`
- `star`
- `snpeff`
- `spades`
- `subread`
- `stdenv`
- `vcflib`
- `vsearch`

- `maven`
- `nodejs`
- `stack`
