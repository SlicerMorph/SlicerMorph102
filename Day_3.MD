## Day 3 topics

### Setting up the R environment
This step takes time and we will need these functionality to do the SlicerMorphR exercises. Best is to let them running while we are learning the DeCaL module. Open the Rstudio (click the R icon on the left bar) and type this command in the R terminal (lower left:

```R
install.packages(c("devtools", "geomorph")
devtools::install_github("SlicerMorph/SlicerMorphR")
```

Minimize your Rstudio window and let this continue. It takes anywhere from 5-10 minutes. 


### DeCA Extension: Dense Correspondence Analysis 
DeCA integrates biological insights in the form of homologous landmark points with dense surface registration to provide highly detailed shape analysis of smooth and complex structures that are typically challenging to analyze with sparse manual landmarks alone.

1. [Rolfe, S. M., Mao, D., & Maga, A. M. (2025). Streamlining Asymmetry Quantification in Fetal Mouse Imaging: A Semi-Automated Pipeline Supported by Expert Guidance. Developmental Dynamics. Early View](https://anatomypubs.onlinelibrary.wiley.com/doi/10.1002/dvdy.70028)
2. [Rolfe, S.M., Maga, A.M. (2023). DeCA: A Dense Correspondence Analysis Toolkit for Shape Analysis. In: Wachinger, C., Paniagua, B., Elhabian, S., Li, J., Egger, J. (eds) Shape in Medical Imaging. ShapeMI 2023. Lecture Notes in Computer Science, vol 14350. Springer, Cham. https://doi.org/10.1007/978-3-031-46914-5_21](https://www.researchgate.net/publication/375111739_DeCA_A_Dense_Correspondence_Analysis_Toolkit_for_Shape_Analysis)


  * [**DeCaL: DeCA semi-Landmarking tool**](https://github.com/SlicerMorph/Tutorials/blob/main/DeCAL/README.md)
  * Atlas building 
  * Editing the atlas for solidfiying
  * Using the Editor to subset the pseudoLMs from the model
### SlicerMorphR 
  * Various convenience functions to read/write mrk.json format into R as data matrix. 
  * Reading SlicerMorph output into R using SlicerMorphR::parser2 function
  * Creating SlicerMorph output from R using SlicerMorphR::geomorph2slicermorph2 function (so that you can slide your LMs and revisualize the results in SlicerMorph)
### ANTsPy Template building 
  * alternative to doing the atlas creation in DeCA


