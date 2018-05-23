# tximport_test

This repo includes a test case of **tximport**. Input files are generated based on:
https://github.com/jaclyn-taroni/ref-txome/

They include `quant.sf` of 6 samples in `PRJNA408323` directory:
- SRR6080007/quant.sf
- SRR6080008/quant.sf
- SRR6080009/quant.sf
- SRR6080012/quant.sf
- SRR6080013/quant.sf
- SRR6080014/quant.sf

and genes-to-transcript mapping file:
- np_gene2txmap.txt (genes-to-transcript mapping file)

To run the test, type:
```
Rscript tximport.R --exp_dir PRJNA408323 --gene2txmap np_gene2txmap.txt
```
which will generate two output files in `PRJNA408323` directory:
- **txi_out.RDS**: RDS of tximport output
- **gene_lengthScaledTPM.tsv**: length-scaled TPM (Transcripts Per Million) file

You can compare them with the two in `expected_output` directory.

More details of the R package `tximport` are available at:
https://bioconductor.org/packages/devel/bioc/vignettes/tximport/inst/doc/tximport.html
