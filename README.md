## Research Papers published Using these Satasets
Naeem, Hajra, and Manar H. Alalfi. "Predicting sensitive information leakage in IoT applications using flows-aware machine learning approach." Empirical Software Engineering 27.6 (2022): 137.

### FlowsMiner 
The FlowsMiner tool is implemented in Python 3 and uses text mining techniques to identify tainted flows. The tool processes the source code of a SmartApp to put the source code in a so called standard format before tokenizing the source code. This reduces the number of cases to be handled at each step while identifying the tainted flows. The tool starts by identifying the sources of a SmartApp. Once the sources set is identified, the sinks are read from a locally deployed file named as Sinks.txt. This tool uses a fixed set of sinks provided in the Sinks.txt file. However, the tool provides flexibility to update the sinks and is capable of working with any set of sinks. The set of sources and sinks are used to identify tainted flows. The tool tokenizes the source code to check if it contains a sink. If the source code contains a sink, it proceeds further to identify tainted flows. The usage of FlowsMiner is fairly straightforward, copy and paste the source code of a SmartApp. The tool analyzes the selected source code to display the tainted flows.

Link: https://141.117.231.79:6852/

### SmartThings - Corpus 1
This folder contains a set of SmartApps from SmartThings. We collected these applications from: https://github.com/SmartThingsCommunity/SmartThingsPublic

### Mutated_SmartApps - Corpus 2
This dataset is prepared by Parveen and Alalfi [[1]](#1). To prepare this dataset they injected mutations in the SmartApps of SmartThings dataset.


## References
<a id="1">[1]</a> 
Sajeda Parveen, Manar H. Alalfi (2020). 
A Mutation Framework for Evaluating Security Analysis Tools in IoT Applications. 
27th {IEEE} International Conference on Software Analysis, Evolution and Reengineering, {SANER} 2020, London, ON, Canada, February 18-21, 2020.
