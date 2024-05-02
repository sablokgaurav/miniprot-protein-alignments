# miniprot-protein-alignments
a miniprot alignments to get the alignment ranges for the protein alignments that were done to generate the hints and also to generate the tabulated table for the length preparation. Run the miniprot as the following. The function below ill map the length so that you can map the aligned length to the plotter. 

```
./miniprot --gff test/DPP3-hs.gen.fa.gz test/DPP3-mm.pep.fa.gz > aln.gff 
miniprotalignment("/home/gaurav/Desktop/aln.gff", splicetype="mRNA")
mRNA = miniprotalignment("/home/gaurav/Desktop/aln.gff", splicetype="mRNA")
length = [i[1]int(i[1][1]) - int(i[1][0]) for i in mRNA]
sns.plot(length) 
```
Gaurav \
Academic Staff Member \
Bioinformatics \
Institute for Biochemistry and Biology \
University of Potsdam \
Potsdam,Germany

