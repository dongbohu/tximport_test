# tximport_test

This repo includes a test case of **tximport**. Input files are generated based on:
https://github.com/jaclyn-taroni/ref-txome/

They include `quant.sf` of 6 samples in experiment `PRJNA408323`:
- PRJNA408323/SRR6080007/quant.sf:
- PRJNA408323/SRR6080008/quant.sf
- PRJNA408323/SRR6080009/quant.sf
- PRJNA408323/SRR6080012/quant.sf
- PRJNA408323/SRR6080013/quant.sf
- PRJNA408323/SRR6080014/quant.sf

and genes-to-transcript mapping file:
- np_gene2txmap.txt: genes-to-transcript mapping file

To run the test, type:
```
Rscript tximport.R --exp_dir PRJNA408323 --gene2txmap np_gene2txmap.txt
```
The two output files will be saved as:
- PRJNA408323/txi_out.RDS
- PRJNA408323/gene_lengthScaledTPM.tsv

You can compare them with the two in `expected_output` directory.
