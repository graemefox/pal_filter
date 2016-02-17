
pal_filter

Program to pick optimum loci from the output of pal_finder_v0.02.04

This program can be used to filter output from pal_finder and choose the
'optimum' loci.

For the paper referncing this workflow, see Griffiths et al.
(unpublished as of 15/02/2016) (sarah.griffiths-5@postgrad.manchester.ac.uk)


INSTALLATION INSTRUCTIONS

To run pal_filter.py you will need the following:

Python 2.7 (https://www.python.org/download/releases/2.7/)

Biopython (http://biopython.org/wiki/Download)

PANDAseq (https://github.com/neufeld/pandaseq)

Clone the pal_filter repo using from your terminal:

    git clone https://github.com/graemefox/pal_filter

Then move into the directory and allow execution of the script:

    cd pal_filter/

    chmod +x pal_filter.py

USAGE

You must supply pal_filter.py both your paired-end FastQ files (R1 and R2 files)
and the output from pal_finder (the -i, -j and -p flags respectively).

You can then turn on the pal_filter.py filters using any of the flags below
(we recommend turning using all flags for the best results in your PCR)

EXAMPLE USAGE

    ./pal_filter.py -i R1.fastq -j R2.fastq -p pal_finder_output.txt -primers -occurrences -rankmotifs -assembly
