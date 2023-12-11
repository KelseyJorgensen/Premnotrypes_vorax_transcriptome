# Premnotrypes_vorax_transcriptome

RNASeq reads from P. vorax (NCBI SRA SRR8266148 and SRR8266149) were trimmed with fastp using the options “--qualified_quality_phred 30 --average_qual 30 --trim_front1 10 --trim_front2 10 –trim_tail1 5 --trim_tail2 5 --trim_poly_x –length_required 50” and then assembled with SOAPdenovo-Trans v1.03 with K=49. The transcriptome consisted of 20,231 transcripts >1 kb summing to 40 Mb. Duplicated transcripts and non-beetle contaminant sequences were removed using methods as described above for the genome assemblies. Transcripts were then clustered with usearch v11.0.667_i86linux32 and options “-id 0.95 -centroids”. Open reading frames for each cluster were predicted with TransDecoder v5.5.0 with a minimum length of 100. 

