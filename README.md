===============

# Auto-Formula: Recommend Formulas in Spreadsheets using Contrastive Learning for Table Representations

 

## Overview

This benchmark dataset contains real Excel spreadsheets from 4 enterprise domains (3 of which are cralwed from the public web): 
- Cisco (cisco.com)
- PGE (pge.com)
- TI (ti.com)
- Enron (we reuse the publicly available Enron spreadsheet dataset, obtained from https://github.com/SheetJS/enron_xls)

In our study  [1] below to predict formulas that users want to author in a target spreadsheet cell (using the actual formula in the target cell as the ground-truth), we test different algorithms using real formulas extracted from the spreadsheets of the 4 enterprise domains above, to test algorithms to accurately predict formulas that users would type in a spreadsheet cell.

We hope the release of this spreadsheet dataset can facilitate futureu research in this and other related directions.


## Data link

Data can be downloaded from [this link](https://1drv.ms/f/s!AkvY8ho1gepOiptfygjBTFLp_V3rtg). 


## Folder structure

```
benchmark
└───Enron
│   └───random
│   └───timestamp
│   │   formulas.json
└───Cisco
│   └───random
│   └───timestamp
│   │   formulas.json
└───PGE
│   └───random
│   └───timestamp
│   │   formulas.json
└───TI
│   └───random
│   └───timestamp
│   │   formulas.json
```
![image](https://github.com/microsoft/Auto-Formula/assets/37452189/a796660f-3e2a-4eb2-8105-70c1d552abec)


## License

This data set is released under the [MICROSOFT RESEARCH LICENSE](https://github.com/microsoft/Auto-Formula/blob/main/Research%20License%20(Nov%202023)%20.docx). 

 

## Reference

[1] Auto-Formula: Recommend Formulas in Spreadsheets using Contrastive Learning for Table Representations. [TOFILL](TOFILL).

===============
