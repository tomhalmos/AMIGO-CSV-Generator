# AMIGO-CSV-Generator

The code will generate the CSV file for DNA-BOT taking any number of genes and a desired output ratio. Unless specified, the backbone, promoter and UTRs will have default settings.

INPUT: GenBank IDs (from the NUCLEOTIDE database), 3 letter code for each gene, gene output ratio
OUTPUT: BASIC sequences for synthesis + CSV file for DNA BOT

The code is now fully up and running, please have a go and let me know any errors/problems. 
Pulling out the nucleotide sequence from the FASTA file you get from the server request was an absolute faff (any improvement appreciated). Thinking that GenBank isn't the best database to use, but the SynBioHub API didn't work so...

The way I pick out RBSs also feels a bit odd. I've taken the relative output of each RBSs and scaled them up to run between 1 and 100. So input the ratio you want with the highest number as close to, but lower than, 100. i.e for a ratio of 1:5:10, input 10:50:100. Keeping everything as integers just made the code a bit easier as working with an output of 1 rather than 0.01. 


