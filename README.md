@(文献阅读记录)[ecDNA][tumor]
# Extrachromosomal oncogene amplification drives tumor evolution and genetic heterogeneity #

[文献](https://www.nature.com/nature/journal/v543/n7643/full/nature21356.html)

**[ecDNA](https://en.wikipedia.org/wiki/Extrachromosomal_DNA)**: *extrachromosomal DNA* 
- 这个染色体外的DNA指的是线粒体质粒DNA？（通过文献阅读，感觉这个染色体外DNA指的是从染色体上脱离下来的DNA）
- 只有tumor中才会有这种脱离的DNA产生，他的很多序列和染色体上的一样。

**[Double minutes](https://en.wikipedia.org/wiki/Double_minute)**: are small fragments of extrachromosomal DNA.

####发现####
1.	文中猜想这种ecDNA的存在导致了异质性的存在，导致有的细胞的copy number变化可以被治好，但是有的细胞的copy number变化无法被治好。这使我猜想，copy number的变化或者ecDNA导致的copy number的变化会不会是由于一个**driver gene** mutation导致。这对以后研究中出现异质性的结果后有一个较好的解释（*推到ecDNA*身上）。
2.	目前还没有研究能够给出产生ecDNA的原因，这可能很关键。

#### 重点 ####
1. ecDNA在几乎一般的human cancers中都有发现，不同的tumor类型含量会有差异。**重来没有在normal cell中发现**。
2. ECdetect（image analysis）能够进行ecDNA detection和analysis。


#### 结论 ####
*使用* **one-sided Wilcoxon rank-sum test** *进行统计计算。*
1. normal cell中的ecDNA count数很少，几乎没有![Alt text](./1498632308072.png)
2.	不同癌肿之间的ecDNA count数也差异不大![Alt text](./1498632365247.png)

*使用* **beta-bin分布**进行proportion的估计（**这个真厉害** *因为每个细胞中的ecDNA含量不同，所以干脆以细胞为统计来进行proportion的估计*）
3.	通过计算的proportion也能得到与count相类似的结果![Alt text](./1498633548211.png)
4.	使用fish的探针针对一些基因进行检测，然后能够检测到某些基因不仅仅在染色体上发生了copy number的变异，还在ecDNA上有。**有趣** ![Alt text](./1498635107693.png)
5.	通过mRNA的表达也能看出，ecDNA的扩增确实会影响表达![Alt text](./1498635194606.png)
6.	从copy number来看，也是ecDNA的扩增能够决定DNA的copy number![Alt text](./1498635445407.png)


#### 判断copy number变化来自于（不太理解的部分，有待于进一步理解） ####
1. use discordant read-pair alignments and coverage information to iteratively visit and extend connected genomic regions with high copy numbers;
2. for each set of connected amplified regions, segment the regions based on depth of coverage using a mean-shift segmentation to detect copy-number changes and discordant read-pair clusters to identify genomic breaks; 
3. construct a breakpoint graph connecting segments using discordant read-pair clusters; 
4. compute a maximum-likelihood network to estimate copy counts of genomic segments; and 
5. report paths and cycles in the graph that identify the dominant linear and circular structures of the amplicon 


