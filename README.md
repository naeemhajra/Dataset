# Datasets

### SmartThings - Corpus 1
We have collected these SmartApps from: https://github.com/SmartThingsCommunity/SmartThingsPublic. To prepare this dataset Celik et al. [[1]](#1) have collected SmartApps from marketplace, community, SmartThings forum and IoTBench.

### Mutated_SmartApps - Corpus 2
The dataset was prepared by Parveen and Alalfi [[2]](#2). To prepare this dataset they injected mutations in the SmartApps of SmartThings - Corpus 1 dataset. They mainly altered the order of statements in benign SmartApps to introduce vulnerabilities that leak sensitive information. Mutations created by them mainly focus on generating tainted flows vulnerabilities by changing the order of statements in the sequential code flow.

## Research Papers published Using these Datasets

<p align="justify">1- Hajra Naeem, and Manar H. Alalfi. "Predicting sensitive information leakage in IoT applications using flows-aware machine learning approach." Empirical Software Engineering 27, no. 6 (2022): 137.
https://link.springer.com/article/10.1007/s10664-022-10157-y 

Preprint of this research paper can be downloaded from: https://arxiv.org/abs/2201.02677

2- Hajra Naeem, and Manar H. Alalfi. "Identifying vulnerable IoT applications using deep learning." In 2020 IEEE 27th International Conference on Software Analysis, Evolution and Reengineering (SANER), pp. 582-586. IEEE, 2020.
https://ieeexplore.ieee.org/abstract/document/9054817

### FlowsMiner 
<p align="justify">The FlowsMiner tool is implemented in Python 3 and uses text mining techniques to identify tainted flows from Corpus1 and Corpus2. The tool processes the source code of a SmartApp to put the source code in a so called standard format before tokenizing the source code. This reduces the number of cases to be handled at each step while identifying the tainted flows. The tool starts by identifying the sources of a SmartApp. Once the sources set is identified, the sinks are read from a locally deployed file named as Sinks.txt. This tool uses a fixed set of sinks provided in the Sinks.txt file. However, the tool provides flexibility to update the sinks and is capable of working with any set of sinks. The set of sources and sinks are used to identify tainted flows. The tool tokenizes the source code to check if it contains a sink. If the source code contains a sink, it proceeds further to identify tainted flows. <!--The usage of FlowsMiner is fairly straightforward, copy and paste the source code of a SmartApp.--> The tool analyzes the selected source code to display the tainted flows.</p>

<!-- I'm commenting/hiding the following link because FlowsMiner is not available at this link anymore-->
<!-- Link: https://141.117.231.79:6852/ -->



## References
<a id="1">[1]</a> 
Celik, Z. Berkay, Leonardo Babun, Amit Kumar Sikder, Hidayet Aksu, Gang Tan, Patrick McDaniel, and A. Selcuk Uluagac. "Sensitive information tracking in commodity IoT." In 27th {USENIX} Security Symposium ({USENIX} Security 18), pp. 1687-1704. 2018.

<a id="2">[2]</a> 
Sajeda Parveen, Manar H. Alalfi (2020). 
A Mutation Framework for Evaluating Security Analysis Tools in IoT Applications. 
27th {IEEE} International Conference on Software Analysis, Evolution and Reengineering, {SANER} 2020, London, ON, Canada, February 18-21, 2020.


