
# To get top 10 biggest contigs in a fasta file:

`faSize contigs.fasta -detailed | sort -k2 -n -r | head`
faSize is a script from [UCSC Kent-utils](https://github.com/ucscGenomeBrowser/kent)

