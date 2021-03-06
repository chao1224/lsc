# lsc
**Large-scale comparison of machine learning methods for drug target prediction on ChEMBL**
* [Link to Publication](https://pubs.rsc.org/en/content/articlelanding/2018/sc/c8sc00148k#!divAbstract)
* [Electronic Supplementary Information](http://www.rsc.org/suppdata/c8/sc/c8sc00148k/c8sc00148k1.pdf)

<br>
<br>

**Additional Information** on dataset creation and code: http://ml.jku.at/research/lsc/index.html

<br>
<br>

**Dataset Download**: http://ml.jku.at/research/lsc/mydata.html
* maybe most interesting to you (in case you are working in Python) is the section `dataPythonReduced` (reduced <span>&#8658;</span> because it is the data on which finally, the benchmark for Deep Learning was performed; everything that is unimportant to the Deep Learning code skipped)
* load `dataPythonReduced`-data (for the FNN case) into Python: https://github.com/ml-jku/lsc/blob/master/pythonCode/apred/loadData.py
* data download script: https://github.com/ml-jku/lsc/blob/master/download.sh (maybe you need only parts out of it, but maybe simpler to use than downloading by browser)
<br>
<br>

**Update Feb 2020:**
* Consider that the source codes are based on an older version of TF1.X and are not adapted to the eager execution mode of TF2.
* A technical appendix and a partial reanalysis is available [here](http://www.bioinf.jku.at/research/lsc/report.pdf). To obtain the results there, change "normalizeLocalDense" to "True" even for sparse features (since for simplicity reasons the matrix in the reference code is converted to a dense one).
<br>
<br>

**BibTeX:**

>@Article{bib:Mayr2018,\
>&nbsp;&nbsp;author="Mayr, Andreas and Klambauer, G{\\"u}nter and Unterthiner, Thomas and Steijaert, Marvin and Wegner, J{\\"o}rg K. and Ceulemans, Hugo and Clevert, Djork-Arn{\\'e} and Hochreiter, Sepp",\
>&nbsp;&nbsp;title={{Large-scale comparison of machine learning methods for drug target prediction on ChEMBL}},\
>&nbsp;&nbsp;journal="Chem. Sci.",\
>&nbsp;&nbsp;year="2018",\
>&nbsp;&nbsp;volume="9",\
>&nbsp;&nbsp;issue="24",\
>&nbsp;&nbsp;pages="5441-5451"\
>} 
