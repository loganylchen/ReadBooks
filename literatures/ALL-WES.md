---
title: The genomic landscape of pediatric and young adult T-lineage acute lymphoblastic leukemia
tags: ALL,nature
notebook: 文献阅读记录
---


## Abstract ##

**T-ALL的hallmarks**:*activate NOTCH  signaling* and *T cell transcription factors*, coupled with *inactivation of the INK4/ARF  tumor suppressors*

1. 264 T-ALL samples genomic analysis
2. New driver genes(CCND3, CTCF, MYB, SMARCA4,  ZFP36L2 and MYCN)

>We describe new mechanisms of coding and noncoding alteration and identify ten recurrently altered  pathways, with associations between mutated genes and pathways, and stage or subtype of T-ALL. For example, NRAS/FLT3  mutations were associated with immature T-ALL, JAK3/STAT5B mutations in HOXA1 deregulated ALL, PTPN2 mutations in TLX1  deregulated T-ALL, and PIK3R1/PTEN mutations in TAL1 deregulated ALL, which suggests that different signaling pathways have  distinct roles according to maturational stage.

## Results ##

### Molecular classification of T-ALL ###

1. 利用的数据为 **whole-exome sequencing** 和 **RNA-seq** 
2. 利用RNA-seq数据将样本费城了8个亚类
 1. TAL1 (n = 87)
 2. TAL2 (n = 8)
 3. TLX1 (n = 26)
 4. TLX3 (n = 46)
 5. HOXA (n = 33)
 6. LMO1/LMO2 (n = 10)
 7. LMO2/LYL1 (n = 18)
 8. NKX2-1 (n = 14) 
3. 针对一些之前没有报道过的突变，和一些较为复杂的突变，还做了基于扩增的测序（相当于做了一个验证）。
4. 利用免疫数据，把样本分成了4组。而且免疫的分类和转录组的分类有一些共同的类别（就是部分样本在免疫的一个类别中，而且也同时在转录组的一个类别里）
<en-media type="image/png" hash="d69267b56f62c5c4c0698326cc6ca95e"/>

**图中展示的也很明显，也就是转录组的表达数据与免疫的数据具有一定的一致性**


### Sequence mutations in pediatric（小儿科的） T-ALL ### 

转录组数据+全外数据，最终检测到的突变
>mean of 15.8 mutations (range: 2–50)


`重点软件：`
**MutSigCV**
**MuSiC**

**ProteinPaint画图软件**<en-media type="text/html" hash="41d773fb25de071da944c2d023ec83cb"/>

>We observed subclonal mutations (defined as those with a mutant allele fraction (MAF) of <0.3) frequently in many driver genes

由这个就得到了一个结论，说亚克隆进化就是一个T-ALL的一个hallmark。这个结论有点意思，可以用到全外的其他项目中。
<en-media type="image/png" hash="31a151f1a0dc1fbd09b5f9f64aae5034"/>

**图中的一个亮点就是，他区分了之前报道中出现的基因，和之前报道中没有出现的基因，整个的实验方法和分析流程其实不算新，但是对于分析做的很细致。这点需要学习**

>For example, NOTCH1 was the most frequently mutated gene, with 264 sequence mutations identified in 196 cases, and most mutations in the heterodimerization domain (62.9%; 166/264) or PEST domain (31.4%; 83/264).

*这个突变的位置都分析到了*

> many cases harbored multiple subclonal mutations in the same gene,indicating that these mutations are secondary events in leukemogenesis but exert driver functions in individual subclones.

**重点，没有理解到的：**   *觉得这个逻辑没有特别理解*
>To determine whether germline sequence mutations may influ- ence a person’s risk of developing T-ALL, we analyzed 89 genes (Supplementary Table 10), including 60 associated with autosomal dominant cancer predisposition syndromes55 and the 35 most fre- quent targets of somatic mutation in this study. We identified only four potentially deleterious germline mutations, in BRAF, BRCA1, BRCA2 and RUNX1 (Supplementary Note 1).

### Gene rearrangements in pediatric T-ALL ###

利用转录组数据检测基因重排，重排的结果：
<en-media type="image/png" hash="9f12be20372cee092c22fc0370c9feab"/>
<en-media type="image/png" hash="442a3eb8c48fe54290b7202e7b26c6ac"/>

> showed that transcriptome sequencing does not identify all rearrangements, notably cases with TLX3 deregulation 

**在25cases中利用全基因组的数据检测到转录组没有检测到的5个重排**

### Recurrently targeted pathways in pediatric T-ALL ###

将检测到的变异进行通路注释，然后进行整理
<en-media type="image/png" hash="b86b2090b32f36e2416cfb5baae150c2"/>

而且做了一个我们常作的基因共同突变及互斥关系，但是和我们常使用的OR及P值不太一样，他们使用相关系数。不过计算方法不太明了，因为正常来说突变和不突变的表示都为1，0表示方法，**难道是用VAF进行计算？这是个不错的方法，可以试一试。**

>Significant association was defined as absolute correlation coefficient greater than 0.1 and p- value less than 0.05 from Spearman correlation analysis.
<en-media type="image/png" hash="19c958749cb49abedb8c60cbe6275b83"/>

而且根据样本的分组，将该组中显著出现的基因进行了网络展示，以通路为主体，哪个通路的基因在哪个组中显著出现，在计算基因与该类样本的关系，得出关系，而之前获得的基因与基因间的关系也可以展示在途中。这是一个很有意思的图。
<en-media type="image/png" hash="3867f10f4b19ef23e79194b4e8c946e2"/>

### Somatic alterations targeting transcriptional regulators ###

针对于转录因子基因（TF）
主要说到一个MYCN基因的P44L位点
<en-media type="image/png" hash="8d045222dbae4cbdf5025d6812b7cc7d"/>

### Signaling pathway mutations in T-ALL ###

待补充

### Patterns of epigenetic mutation in T-ALL ###

待补充

### Mutational spectra of ETP and non-ETP T-ALL ###

待补充

## DISCUSSION ##

待补充

## 收获 ##

1. 有一篇讲germline突变与疾病的关系的文章需要研读一下，刚好是这篇的参考文献。<en-media type="text/html" hash="7a1783ec6adae4ac401c7ffc5eb501b9"/>
2. 知道了一个有关于话基因突变位置在基因上展示的软件，web-server。
3. 








