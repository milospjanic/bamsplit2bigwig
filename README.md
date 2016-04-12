# bamsplit2bigwig

This script will take bam file **(mapped to human genome hg19)** and convert it to two bigwig files that could be uploaded to UCSC Genome Browser. It depends on bedtools bamtobed (aka bamToBed), and it will attempt to download and execute three UCSC scripts, bedItemOverlapCount, bedGraphToBigWig and fetchChromSizes, so make sure your connection is working.
Converting bam to bigwig and separating according to strand could be useful to visualize nucleosomal or protein binding 'footprints' in ChIP-Seq experiments as at the boundaries of protein-DNA interactions will be marked with reads mapping on different DNA strands. 

# Usage

<pre>
chmod 775 bamsplit2bigwig
./bamsplit2bigwig file.bam
</pre>

Note the bam file name is an example, add your file name.

# Example output

