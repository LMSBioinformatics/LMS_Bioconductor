# Bioconductor


## The Course

This course introduces some of the fundamental concepts and tools available in Bioconductor.

Each section is presented as both HTML and Rpres markdown (to allow for intergration of the presentation in the RStudio enviroment itself).  Exercises and answer sheets are included after all subsections to practice techniques and provide future reference examples. 

  
All material is available to download under GPL v3 license. For  information on other courses run by our team see our [github IO page](http://bioinformatics.lms.mrc.ac.uk/LMStraining.html).


## The Team
This course was created and conducted by the MRC London Institute of Medical Sciences Bioinformatics Team at Imperial College London, Hammersmith Hospital.  
For more information on the team see our [github IO page](http://bioinformatics.lms.mrc.ac.uk/LMSpeople.html).

This course is free for MRC LMS and Imperial staff and students. 


## Setting up.


#### Install R.

R can be installed from the R-project website.  
R 3.6.0 or higher is required for this course.

http://www.r-project.org/

#### Install RStudio.

RStudio can be installed from the R-project website. 

http://www.rstudio.com/

#### Install required packages.

Having downloaded R and RStudio, some additional packages are required (rmarkdown and ggplot2).  

To install these,
* First launch RStudio
* Install the packages in the R console if R version > 3.5.0
<pre>
if (!requireNamespace("BiocManager", quietly = TRUE))
    install.packages("BiocManager")

BiocManager::install(c("GenomicRanges","limma","Rsamtools","GenomicAlignments",
"org.Hs.eg.db","TxDb.Mmusculus.UCSC.mm9.knownGene","GenomicFeatures","biomaRt"))
</pre>
* Install the packages in the R console if R version <= 3.5.0
<pre>
source("https://bioconductor.org/biocLite.R")
biocLite(c("GenomicRanges","limma","Rsamtools","GenomicAlignments",
"org.Hs.eg.db","TxDb.Mmusculus.UCSC.mm9.knownGene","GenomicFeatures","biomaRt"))
</pre>

<!--#### Download the material
The material can either be downloaded as a [zip](https://github.com/LMSBioinformatics/LMS_Bioconductor/archive/master.zip)
<pre>
wget https://github.com/LMSBioinformatics/LMS_Bioconductor/archive/master.zip ./
</pre>
or checked out from our Github repository
https://github.com/mrccsc/Bioconductor/ -->
