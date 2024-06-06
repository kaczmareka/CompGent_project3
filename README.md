# CompGent_project3


exec &>output/log.txt
cnvpytor -root file.pytor -rd SRR_final_sorted.bam -chrom chr1 chr2 chr3 chr4 chr5 chr6 chr7 chr8 chr9 chr10 chr11 chr12 chr13 chr14 chr15 chr16 chr17 chr18 chr19 chr20 chr21 chr22 chrX chrY -T GRCh38_full_analysis_set_plus_decoy_hla.fa > output/temp_calls_1.txt
cnvpytor -root file.pytor -his 1000 > output/temp_calls2.txt
cnvpytor -root file.pytor -partition 1000 > output/temp_calls3.txt
cnvpytor -root file.pytor -call 1000 > output/temp_calls4.txt
cnvpytor -root file.pytor -view 1000 > output/temp_calls5.txt
