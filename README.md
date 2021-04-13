# Works for Me! Cannot Reproduce -- A Large Scale Empirical Study of Non-reproducible Bugs

**Mohammad Masudur Rahman, Foutse Khomh, and Marco Castelluccio**

**Abstract** Software developers attempt to reproduce software bugs 
	to understand their erroneous behaviours and to fix them. 
	Unfortunately, they often fail to reproduce (or fix) them, which leads to 
	faulty, unreliable software systems. However, to date, only a little research has been done to better understand what makes the software bugs non-reproducible. In this article, we conduct a multimodal study to better understand the non-reproducibility of software bugs. First, we perform an empirical study using 576 non-reproducible bug reports from two popular software systems (Firefox, Eclipse) and identify 11 key factors that might lead a reported bug to non-reproducibility. Second, we conduct a user study involving 13 professional developers where we investigate how the developers cope with non-reproducible bugs. We found that they either close these bugs or solicit for further information, which involves long deliberations and counter-productive manual searches. Third, we offer several actionable insights on how to avoid non-reproducibility (e.g., false-positive bug report detector) and improve reproducibility of the reported bugs (e.g., sandbox for bug reproduction) by combining our analyses from multiple studies (e.g., empirical study, developer study). 
	Fourth, we explain the differences between reproducible and non-reproducible bug reports by systematically interpreting multiple machine learning models that classify these reports with high accuracy. We found that links to existing bug reports might help improve the reproducibility of a reported bug.
	Fifth, we further demonstrate how 93 prior bugs connected to 71 non-reproducible bugs from our dataset can offer complementary information (e.g., attachments, screenshots, program flows).


Subject Systems
---------------------------
**WORKSFORME**
- Mozilla Firefox Core (250)
- Eclipse JDT (326)

**FIXED**
- Mozilla Firefox Core (250)
- Eclipse JDT (283)


**Total: 1,109**

Materials Included
-----------------------------
- **```Grounded Theory```** contains all the artifacts generated during our empiricial study
  - **Firefox Core**: Open Coding, Axial Coding 
  - **Eclipse JDT**: Open Coding, Axial Coding
  - **Combined:** Selective Coding
  - **Combined:** Key Factors
- **```Developer Study```** contains all the artifacts generated during our developer study
  - Raw responses from the developers
  - Agreed + Disagreed responses
- **```Machine Learning Model```** contains all the artifacts related to machine learning-based classification & model interpretation
  - **Dataset**: Contains the 17 attibutes (12 structural + 2 textual + 3 sentiment) for 1,109 bug reports.
  - **SelectedBugs**: Bug IDs of 1109 bugs from Firefox Core and Eclipse JDT
  - **XGBoost**: Implemented classifier & configuration
  - **Model Interpretation**: Jupyter notebook containing the code to generate all the interpretation diagram using **SHAP** framework
  - *Model Configurations*: Naive Bayes, Logistic Regression, J48, and RandomForest used the default configurations from Weka 3.9.4
- **```Manual Analysis```** contains all artifacts generated during manual analysis
  - *Eclipse-Firefox-Manual-Analysis* : Shows whether the connected bug reports contain stack traces, fixes, attachments, and other items
  - *Manual-Analysis-Workbook* : Raw data from the manual analysis.
- README
- LICENSE


Accepted Paper at ICSME 2020
-----------------------------
**TCSE Distinguished Paper Award 2020**
```
Why are Some Bugs Non-Reproducible? An Empirical Investigation using Data Fusion

Mohammad Masudur Rahman, Foutse Khomh, and Marco Castelluccio
```
![Distinguished Paper Award Nomination](https://web.cs.dal.ca/~masud/nlp2api/img/dpa-150.png) 

**Download this paper:**  [<img src="https://web.cs.dal.ca/~masud/img/pdf.png"
     alt="PDF" heigh="16px" width="16px" />](https://web.cs.dal.ca/~masud/papers/masud-ICSME2020-pp.pdf)


Please contact **Masud Rahman (masud.rahman@dal.ca)** for details.



