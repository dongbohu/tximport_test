# tximport_test

This repo includes a test case of tximport. Input files are generated based on:
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

The expected output files are located in `expected_output` directory.
- txi_out.RDS: RDS of tximport output
- gene_lengthScaledTPM.tsv: length-scaled TPM (transcripts per million) file
