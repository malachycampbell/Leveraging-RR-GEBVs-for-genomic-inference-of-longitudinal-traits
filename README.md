<h1 align="center">
  <img alt=" Leveraging breeding values obtained from random regression models for genetic inference of longitudinal traits" width = "1711.846" height = "200" src = Title.svg>
</h1>

[Malachy Campbell](https://malachycampbell.github.io/), [Harkamal Walia](http://cropstressgenomics.org/), [Gota Morota](http://morotalab.org/)

## Abstract
Understanding the genetic basis of dynamic plant phenotypes has largely been limited due to lack of space and labor resources needed to record dynamic traits, often destructively, for a large number of genotypes. However, recent advent of image-based phenotyping platforms has provided the plant science researchers with an effective means to non-destructively evaluate morphological, developmental, and physiological processes at regular, frequent intervals for a large number of plants throughout development. The statistical frameworks typically used for genetic analyses (e.g. genome-wide association mapping, linkage mapping, and genomic prediction) in plant breeding and genetics are not particularly amenable for repeated measurements. Random regression (RR) models are routinely used in animal breeding for the genetic analysis of longitudinal traits, and provide a robust framework for  modeling traits trajectories and performing genetic analysis simultaneously. We recently used a RR approach for genomic prediction of shoot growth trajectories in rice. Here, we have extended this approach for genetic inference by leveraging genomic breeding values derived from RR models for rice shoot growth during early vegetative development. This approach provides considerable improvement for discovering loci associated with shoot growth trajectories over a conventional single time point analyses. This RR approach uncovers persistent, as well as time-specific, transient quantitative trait loci. This methodology can be widely applied to understand the genetic architecture of other complex polygeneic traits with repeated measurements.

## Background
This repo contains all the code and data used for the manuscript: "Leveraging breeding values obtained from random regression models for genetic inference of longitudinal traits". It builds off the approach used for our 2018 Plant Direct paper where we used RR for genomic prediction of shoot growth trajectories. Breifly, this approach estimates marker effects from breeding values obtained using a random regression model, and estaimtes the marker variance and corresponding *p*-values. The pipeline uses both [ASREML](https://www.vsni.co.uk/downloads/asreml/) and R. To predict the breeding values, users should have [ASREML](https://www.vsni.co.uk/downloads/asreml/) installed. Alternativly, you can just use the ".sln" files that are provided. All the code is presented in Rmarkdown, and the '.as' files used for ASREML are included as snippets in the .Rmd files. The contents are layed out according to the order presented in the methods section of the paper. All input and output is provided in [DataandCode.zip](DataandCode.zip). Refer to the README for a brief description of the contents.  

The phenotypic and genotypic data used is the same that was used in our Plant Direct manuscript. So if you are interested in seeing how we cleaned up the raw data, head on over to the [RR genomic prediction page](https://github.com/malachycampbell/Utilizing-random-regression-models-for-genomic-prediction-of-a-longitudinal-trait-derived-from-HTP) and check out the first two sections.

## Table of Contents 
* **1. Preparation of Genotypic Data**
  - [html output](https://rawgit.com/malachycampbell/Leveraging-RR-GEBVs-for-genomic-inference-of-longitudinal-traits/master/HTMLoutput/1.GenotypicData.html)
  - [.Rmd File](https://rawgit.com/malachycampbell/Leveraging-RR-GEBVs-for-genomic-inference-of-longitudinal-traits/master/HTMLoutput/1.GenotypicData.Rmd)
  
* **2. Predicting GEBVs with random regression models**
  - [html output](https://rawgit.com/malachycampbell/Leveraging-RR-GEBVs-for-genomic-inference-of-longitudinal-traits/master/HTMLoutput/2.GEBVs_RR.html)
  - [.Rmd File](https://rawgit.com/malachycampbell/Leveraging-RR-GEBVs-for-genomic-inference-of-longitudinal-traits/master/HTMLoutput/2.GEBVs_RR.Rmd)
  
* **3. Predicting GEBVs with single time point gBLUP models**
  - [html output](https://rawgit.com/malachycampbell/Leveraging-RR-GEBVs-for-genomic-inference-of-longitudinal-traits/master/HTMLoutput/3.GEBVs_TP.html)
  - [.Rmd File](https://rawgit.com/malachycampbell/Leveraging-RR-GEBVs-for-genomic-inference-of-longitudinal-traits/master/HTMLoutput/3.GEBVs_TP.Rmd)
  
* **4. Estimating marker effects from GEBVs**
  - [html output](https://rawgit.com/malachycampbell/Leveraging-RR-GEBVs-for-genomic-inference-of-longitudinal-traits/master/HTMLoutput/4.BetasFromGEBVs.html)
  - [.Rmd File](https://rawgit.com/malachycampbell/Leveraging-RR-GEBVs-for-genomic-inference-of-longitudinal-traits/master/HTMLoutput/4.BetasFromGEBVs.Rmd)
 
* **5. Calculating *p*-values for RR and TP GWAS**
  - [html output](https://rawgit.com/malachycampbell/Leveraging-RR-GEBVs-for-genomic-inference-of-longitudinal-traits/master/HTMLoutput/5.CalculatingPvaluesForGWAS.html)
  - [.Rmd File](https://rawgit.com/malachycampbell/Leveraging-RR-GEBVs-for-genomic-inference-of-longitudinal-traits/master/HTMLoutput/5.CalculatingPvaluesForGWAS.Rmd)
  
* **6. Summarising GWAS results**
  - [html output](https://rawgit.com/malachycampbell/Leveraging-RR-GEBVs-for-genomic-inference-of-longitudinal-traits/master/HTMLoutput/6.SummariseGWASResults.html)
  - [.Rmd File](https://rawgit.com/malachycampbell/Leveraging-RR-GEBVs-for-genomic-inference-of-longitudinal-traits/master/HTMLoutput/6.SummariseGWASResults.Rmd)
  
* **6. Classification of QTL from the RR approach**
  - [html output](https://rawgit.com/malachycampbell/Leveraging-RR-GEBVs-for-genomic-inference-of-longitudinal-traits/master/HTMLoutput/7.ClassificationOfQTL.html)
  - [.Rmd File](https://rawgit.com/malachycampbell/Leveraging-RR-GEBVs-for-genomic-inference-of-longitudinal-traits/master/HTMLoutput/7.ClassificationOfQTL.Rmd)
  
 ## Funding
*Funding for this project was provided by the National Science Foundation through the Plant Genome Reasearch Program grant [(#1238125)](https://www.nsf.gov/awardsearch/showAward?AWD_ID=1238125) awarded to HW and a Research Infrastructure Improvement (RII) Track-2 Focused EPSCoR grant [(#1736192)](https://www.nsf.gov/awardsearch/showAward?AWD_ID=1736192) awarded to HW and GM.*

---

<img align = "left" alt="WRCHR" src = WRCHR.png width = "200" height = "65.43491">
<img align = "left" alt="NSF" src = nsf_logo.png width = "65.43491" height = "65.43491"/>
