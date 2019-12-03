1. Explain BAM FLAG value： 143
143=128+15
   =128+8+7
   =128+8+4+3
   =128+8+4+2+1
解释：在paired reads中，该read是与参考序列比对的第二条，与该read成对的matepair read没有比对到参考序列上，该read没比对到参考序列上，paired reads中每个都正确比对到参考序列上，该read是成对的paired reads中的一个。

2.Explain BAM FLAG value： 99
99=64+35
  =64+32+3
  =64+32+2+1
解释：在paired reads中，该read是与参考序列比对的第一条，与该read成对的matepair read其反向互补序列能够比对到参考序列，paired reads中每个都正确比对到参考序列上，该read是成对的paired reads中的一个。

3. Explain BAM FLAG value：516
516=512+4
解释：该read没有通过质量控制，该read没比对到参考序列上

4. Explain BAM FLAG value： 2064
2064=2048+16
解释：补充匹配的read，该read其反向互补序列能够比对到参考序列

5.Explain BAM FLAG value： 147
147=128+19
   =128+16+3
   =128+16+2+1
解释：在paired reads中，该read是与参考序列比对的第二条，该read其反向互补序列能够比对到参考序列，paired reads中每个都正确比对到参考序列上，该read是成对的paired reads中的一个。

6. Explain BAM CIGAR：14M2D31M
解释：这条序列与参考基因相比，有14个碱基完全匹配，有2个碱基删除，然后31个碱基的完全匹配

7. Explain BAM CIGAR：3S6M1D5M
解释：这条序列与参考基因相比，有三个碱基虽然比对不上参考基因组，但是在reads上还是存在，然后6个碱基完全匹配，1个碱基删除，然后5个碱基匹配。

8. Explain BAM CIGAR: 6M14N5M
解释：这条序列与参考基因相比，有六个碱基完全匹配，接着跳过第三列的 RNAME 序列上 14 bp，然后5个碱基完全匹配

9.Explain BAM CIGAR: 7M5D8M2I14M  (小写：7m5d8m2i14m）
解释：有7个碱基完全匹配，然后5个碱基删除，然后8个碱基完全匹配，然后2个碱基插入，然后14个碱基完全匹配。

10.how long is the read with alignment CIGAR of 7M5D8M2I14M?
答：7+8+2+14=31 该read长31bp


