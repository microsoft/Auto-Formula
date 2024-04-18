
# Auto-Formula: Recommend Formulas in Spreadsheets using Contrastive Learning for Table Representations 
 

## Benchmark overview

This benchmark dataset contains real Excel spreadsheets from 4 enterprise domains (3 of which are cralwed from the public web): 
- Cisco (cisco.com)
- PGE (pge.com)
- TI (ti.com)
- Enron (we reuse the publicly available Enron spreadsheet dataset, obtained from https://github.com/SheetJS/enron_xls)

In our study  [1] below to predict formulas that users want to author in a target spreadsheet cell (using the actual formula in the target cell as the ground-truth), we test different algorithms using real formulas extracted from the spreadsheets of the 4 enterprise domains above, to test algorithms to accurately predict formulas that users would type in a spreadsheet cell.

Statistics of this spreadsheet benchmark can be found in the table below. 
![image](https://github.com/microsoft/Auto-Formula/assets/37452189/a796660f-3e2a-4eb2-8105-70c1d552abec)

We hope the release of this spreadsheet dataset can facilitate futureu research in this and other related directions.


## Data link

Data can be downloaded from [this link](https://1drv.ms/f/s!AkvY8ho1gepOiptfygjBTFLp_V3rtg). 


## Folder structure

The benchmark has 4 folders, each corresponds to an enterprise domain (Cisco, PGE, TI, Enron). 

Furthermore, in our experiments we tested two ways of sampling test spreadsheets: 
- (1) Random: randomly sample 10% from spreadsheets in the same enterprise domain as test cases;
- (2) Timestamp: order all spreadsheets by timestamps (last modified time), and use the most recently modified 10% spreadsheets as test cases.

These two test settings correspond to the two sub-folders named "random" and "timestamp: under Cisco/PGE/TI/Enron, respectively.

```
benchmark
└───Cisco
│   └───random
│   └───timestamp
│   │   test_formulas.json
└───PGE
│   └───random
│   └───timestamp
│   │   test_formulas.json
└───TI
│   └───random
│   └───timestamp
│   │   test_formulas.json
└───Enron
│   └───random
│   └───timestamp
│   │   test_formulas.json
```

Each folder contains two sub-folders for reference workbooks and test workbooks. There is also a "test_formulas.json" file, which contains formulas sampled as test cases, where the format is "spreadsheet-file-name"---"sheet-name"---"row-id"---"col-id" (e.g., ```"244228682981234450530384331754331956360-mls-mqc-qos-converter-v1.xlsx---MQCtoMLSQOS---19---15"```).


## License

This data set is released under the [MICROSOFT RESEARCH LICENSE](https://github.com/microsoft/Auto-Formula/blob/main/Research%20License%20(Nov%202023)%20.docx). 

 

## Reference

[1] Auto-Formula: Recommend Formulas in Spreadsheets using Contrastive Learning for Table Representations. [TOFILL](TOFILL).

