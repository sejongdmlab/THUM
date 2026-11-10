# THUM

This article provides executables of software and datasets used in our research for Incremental Top-k High Utility Pattern Mining with Modification.

The executables include the software of THUM, PULM+K, ITHUI+M, PreTK+M, and PIHUP-MOD+K and the datasets of Retail, Mushroom, Chess, Chainstore, OnlineRetail, E-Shop, and T10I4D200K—T10I4D1000K.

All executables were compiled to run on 64-bit architectures.

Please refer to the following guide:

1. Note that the names of the executables match their corresponding approach names.

2. The parameters of the executables are as follows:

 for THUM, PULM+K, ITHUI+M, PreTK+M, and PIHUP-MOD+K
```bash
[0]          [1]       [2]                 [3]                     [4]                  [5]
[Executable] [K-value] [Utility Data Path] [Transaction Data Path] [Modification Ratio] [Division Number]
```


3. Next, the file name and the parameters of each dataset are as follows:

| Dataset     | Number of Transactions | Number of Items | \|T\|.avg |
| ----------- | ---------------------- | --------------- | --------- |
| Retail      | 88,162                 | 16,469          | 10.3      |
| Mushroom    | 8,124                  | 119             | 23.0      |
| Chess       | 3,196                  | 75              | 37.0      |
| Chainstore  | 1,112,949              | 46,086          | 7.23      |
| OnlineRetail| 530,104                | 7,918           | 6.75      |
| E-Shop      | 165,474                | 24,564          | 13.0      |
| T10I4DxK    | 200,000-1,000,000      | 100             | 10        |

4. For example
```bash
THUM 200 ..\Data\utilRetail.txt ..\Data\Retail.txt 2.0 4
```
will run THUM on Retail, with k set to 200, a modification ratio of 2.0%, and 4 data increments.

5. The output directory "/out" is required for writing result patterns for all algorithms.