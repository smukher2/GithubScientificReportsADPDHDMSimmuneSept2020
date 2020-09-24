# GithubScientificReports2020

## This github repository is made open access in hope that it will enable researchers replicate and/or adapt it for their work. So if you use or adapt the results, inferences and computational pipelines presented here, I will be grateful if you please help by citing it as follows. 

# Please help by citing this article and methods as follows (one citation): 
### Mukherjee, S. Immune signature genes are enriched in shared gene networks associated with neurological disorders: Multiple Sclerosis (MS), Alzheimer’s disease (AD), Parkinson’s disease (PD) and Huntington’s disease (HD). Scientific Reports (2020 submitted). (put doi link here)



# Author Information
Shradha Mukherjee*#
Address correspondence to: Shradha Mukherjee, PhD; Alias Goldy; Garland Avenue, Downtown Los Angeles, Los Angeles, CA 90017, U.S. Email: smukher2@gmail.com
* First author and # Corresponding author

Shradha Mukherjee, PhD in Biochemistry,                                                                                                                                       
MS in Chemistry, MAS in Health Informatics 

CV/Resume Link https://github.com/smukher2/Shradha_Mukherjee_Resume                                                                                      
Researchgate Link https://www.researchgate.net/profile/Shradha_Mukherjee                                                         
Github Link https://github.com/smukher2                                                                                                                                       
Pubmed Link https://www.ncbi.nlm.nih.gov/pubmed/?term=Shradha+Mukherjee   
Youtube Channel Link https://www.youtube.com/user/smukher2/playlists


# Protocol: Organization of folders containing subfolders, files and codes. 
 
**Step1 DEG_NoCuff_CellTypeBrainImmune(notStemCells)/ 

Contains the codes, input files and results for entire analysis of a select cell types vs other cell types differential gene expression analysis with 3 methods (Limma, edgeR and simple comparison of means) starting from htseq count files. The htseq count files were obtained in Step1 above.
The minimum files, folders and .Rmd codes required to reproduce the results are provided. After downloading these if the user runs the .Rmd codes in RStudio using command 'knit to html' or 'Run all' it should reproduce same results. 
  
**Step2 HuAgeDis_MSNDsplitArray(recoded)_7.71/ 

Contains the codes, input files and results for WGCNA analysis of gene expression array files. Also contains code for characterization of modules with enrichR such as GO analysis;  
The minimum files, folders and .Rmd codes required to reproduce the results are provided. After downloading these if the user runs the .Rmd codes in RStudio using command 'knit to html' or 'Run all' it should reproduce same results. 

**Step3 HuAgeDis_MSNDsplitRnaseq(recoded)_v7.71_minMod100/ 

Contains the codes, input files and results for WGCNA analysis of htseq files obtained in Step1 above. Also contains code for characterization of modules with enrichR such as GO analysis;
The minimum files, folders and .Rmd codes required to reproduce the results are provided. After downloading these if the user runs the .Rmd codes in RStudio using command 'knit to html' or 'Run all' it should reproduce same results. 

**Step4 HuAgeDis_MSNDsplit_Array_Rnaseq_Preservation_minMod100(bw)/ 

Contains the codes, input files and results for comparison of gene expression array WGCNA analysis and RNA-seq WGCNA analysis outputs obtained in Step3 and Step4 above. Black and white figures are generated for preservation. 
The minimum files, folders and .Rmd codes required to reproduce the results are provided. After downloading these if the user runs the .Rmd codes in RStudio using command 'knit to html' or 'Run all' it should reproduce same results. 

**Step5 HuAgeDis_MSNDsplit_Array_Rnaseq_Preservation_minMod100(color)/ 

Contains the codes, input files and results for comparison of gene expression array WGCNA analysis and RNA-seq WGCNA analysis outputs obtained in Step3 and Step4 above. Color figures are generated for preservation. 
The minimum files, folders and .Rmd codes required to reproduce the results are provided. After downloading these if the user runs the .Rmd codes in RStudio using command 'knit to html' or 'Run all' it should reproduce same results. 

**Step6 HuAgeDis_MSNDsplit_Array_Rnaseq_Preservation_minMod100(red)/ 

Contains the codes, input files and results for comparison of gene expression array WGCNA analysis and RNA-seq WGCNA analysis outputs obtained in Step3 and Step4 above. Red figures are generated for preservation. 
The minimum files, folders and .Rmd codes required to reproduce the results are provided. After downloading these if the user runs the .Rmd codes in RStudio using command 'knit to html' or 'Run all' it should reproduce same results. 

**Footnote: Below are three different methods for installation of R packages. 
*Method 1 replace within "" the package name to be installed
library(BiocInstaller)
biocLite(c("name_of_package1","name_of_package2"))

*Method 2
install.packages(c("name_of_package1","name_of_package2"))

*Method 3
install.packages("BiocManager")
BiocManager::install(c("name_of_package1","name_of_package2"))
 

# Acknowledgements: 

1) SVA: Dr. Jeff Leek http://jtleek.com/genstats/inst/doc/02_13_batch-effects.html and https://www.bioconductor.org/packages/release/bioc/vignettes/sva/inst/doc/sva.pdf
2) WGCNA: Dr. Jeremy Miller https://horvath.genetics.ucla.edu/html/CoexpressionNetwork/JMiller/
3) WGCNA Preservation: Dr. Steve Horvath and Dr. Peter Langfelder https://horvath.genetics.ucla.edu/html/CoexpressionNetwork/ModulePreservation/Tutorials/MiniTutorial-MouseLiver.pdf
4) WGCNA Hub Genes: Dr. Steve Horvath and Dr. Peter Langfelder https://pdfs.semanticscholar.org/5e42/e2185c54874277794395e5825808e5f5709c.pdf
5) edgeR: https://github.com/smukher2/StemCells_RNAseq_Expression_edgeR_visualization_GO and https://web.stanford.edu/class/bios221/labs/rnaseq/lab_4_rnaseq.html
6) limma: https://kasperdanielhansen.github.io/genbioconductor/html/limma.html and https://ucdavis-bioinformatics-training.github.io/2018-June-RNA-Seq-Workshop/thursday/DE.html

Users new to SVA, MEGENA and Differential Gene Expression methods are encouraged to refer to the above mentioned turotials and pipelines. Other acknowledgements have been added to the best of our knowledge as #comment in the code/pipeline itself. 
