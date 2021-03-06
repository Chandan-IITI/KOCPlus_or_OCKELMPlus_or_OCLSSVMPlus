# KOC+ or OCKELM+
One-class KRR or One-class KELM with Privileged Information

If you are using this code then kindly cite the folowing **paper**: 

### C. Gautam, A. Tiwari, and M. Tanveer, KOC+: Kernel ridge regression based one-class classification using privileged information, Information Sciences, vol. 504, pp. 324-333, 2019 (ELSEVIER).

                  https://www.sciencedirect.com/science/article/pii/S0950705118305823


**KOC+ can also be treated as the variant of Kernel Extreme learning Machine or Least Squares SVM with zero bias, therefore, paper and method can also be named as follows:**

OCKELM+: Kernel Extreme Learning Machine based One-class Classification using Privileged Information 

or 

LSSVM+: Least Square SVM with zero bias based One-class Classification using Privileged Information


## For reproducing the results of Heart datasets:

--  Open KOC+_Heart_Experiments.ipynb in Python notebook and run all cells. It will save all results in .pkl files. Results on optimal   parameters along with optimal parameters values will be saved in a excel file.   

--  Be dfault these codes produce results for group attribute 'Age'. For other two group attributes (Sex and Electrocardiographic): change the value in cell number 3 and 4 as follows:

**For group attribute = Sex:**

Uncomment this line in cell 3:  
 privileged_space = privileged_space_tot.ix[:]['p1']

Uncomment this line in cell 4:
 feature_space = feature_space.drop('a2', axis=1)
 privfeat = 'Sex'

**For group attribute = Electrocardiographic:**

Uncomment this line in cell 3:  
 privileged_space = privileged_space_tot.ix[:]['p3']

Uncomment this line in cell 4:
 feature_space = feature_space.drop('a7', axis=1)
 privfeat = 'Elect'


**For any query, you can reach me at chandangautam31@gmail.com , phd1501101001@iiti.ac.in**
