# Tissue_Nonvariable_450K_CpGs
Scripts and lists of CpGs which are seen as non-variable in GEO data on the 450K.

# Download CpG List into R
library(RCurl)
x <- getURL("https://raw.githubusercontent.com/redgar598/Tissue_Invariable_450K_CpGs/master/Invariant_Buccal_CpGs.csv")
y <- read.csv(text = x)
nonvariable_buccal<-y$CpG

## Validation
In a study of 25 blood samples @lmcewen ~108,000/114,000 blood invariable CpGs were non-variable. 

In PAWS @redgar598 (buccals) 99.5% of the buccal non-variable CpGs are also invariable in PAWS
