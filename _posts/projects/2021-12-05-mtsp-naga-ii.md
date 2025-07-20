---
layout: post
title: "MTSP-NAGA-II"
author: Zhicheng Zhang (leader), Chenyang Lei and Yuxiang Chen
date: 2021-12-05 09:33:56 +0800
tags: [Project]
excerpt_separator: <!--excerpt-->
comments: true
sticky: false
---

This is the code of course project in Advanced Artificial Intelligence. This project uses **NSGA-II** to solve the problem of **Multiple Traveling Salesmen Problem**.<!--excerpt--> The baseline code is [GA-for-mTSP](https://github.com/Anupal/GA-for-mTSP) and we finetuned its parameters to make it more suitable for our experiment. The population select algorithm of our code was mainly based on the [NSGA-II](https://github.com/haris989/NSGA-II) and the enhanced GA algorithm is mainly based on [the arifield's work](ttps://github.com/ariefield/MTSP-Genetic). For more information, please visit [the repository](https://github.com/ZZwarn1998/MTSP_NSGA_II).  

## Contribution

<table>
<tr>
    <th>NAME</th>
    <th>ID</th>
    <th>CONTRIBUTION</th>
</tr>
<tr>
    <td>Zhang Zhicheng (leader)</td>
    <td>12132375</td>
    <td>1/3</td>
</tr>
<tr>
    <td>Lei Chenyang</td>
    <td>12132336</td>
    <td>1/3</td>
</tr>
<tr>
    <td>Yuxiang Chen</td>
    <td>12132330</td>
    <td>1/3</td>
</tr>
</table>

## Instruction manual
### Repeate our experiment result
1. **Change** the dir to `baseline/code/`, and run the shell `repeat_test.sh`, and
 you will get the baseline result saved in the `baseline_run_data.json`<br/><br/>
2. **Change** the dir ro `mtsp_nsga_ii/code/`, and run the python file `repeat_test.py`, and
you will get the improved GA result saved in the `ours_run_data.json`<br/><br/>
3. **Move** the two `.json` file you get in the previous step to `summary_figure/` and run `polt_figure.py`and `summary.py` , and you will get the result figure and table of this two algorithm we represent in  our report.

> Note: It needs a lot of time to run the experiment, as we repeat 30 times in each dataset.

### Run the enhanced GA algorithm
**Change** the dir to `mtsp_nsga_ii/code/`
 ```
 >python main.py 
 usage main.py --problem [--traveller] [--population] [--generations] [--mutation]
 optional arguments:
         --problem      problem name
         --traveller    number of travellers,default 5
         --population   number of population,default 100
         --generations  number of generations, default 200
         --mutation     nutation rate, default 0.2
 ```
 
<!-- * If you just want to obtain the results of six data sets stored in **mtsp_nsga_ii/data**, you can run **mtsp_nsga_ii/code/repeat_test.py**.   
* If you add a new data set in **mtsp_nsga_ii/data**, please remember to add the the name of new data set to the parameter  **`problem_name_list`**, which can be found in **mtsp_nsga_ii/code/repeat_test.py**, and then run **mtsp_nsga_ii/code/repeat_test.py**.  
* If you want to modify **the number of traveling salesman**, **the number of populations**, **the number of trainings**, **mutation rate**, and **the number of program repetitions**, you can modify **`num_travellers`**, **`population_size`** , **`generations`**, **`mutation_rate`** and **`repeat_times`** separately. You can find them in **mtsp_nsga_ii/code/repeat_test.py**. -->

<!-- ## File manifest  
─MTSP_NSGA_II-master
    │  README.md
    │
    ├─.idea
    │  │  .gitignore
    │  │  deployment.xml
    │  │  misc.xml
    │  │  modules.xml
    │  │  MTSP_NSGA_II.iml
    │  │  other.xml
    │  │  vcs.xml
    │  │  workspace.xml
    │  │
    │  └─inspectionProfiles
    │          profiles_settings.xml
    │          Project_Default.xml
    │
    ├─baseline
    │  │  dustbin.py
    │  │  galogic.py
    │  │  globals.py
    │  │  main.py
    │  │  nodenum.py
    │  │  population.py
    │  │  README.md
    │  │  repeat_test.sh
    │  │  route.py
    │  │  routemanager.py
    │  │
    │  └─data
    │          mtsp100.txt
    │          mtsp150.txt
    │          mtsp51.txt
    │          pr152.txt
    │          pr226.txt
    │          pr76.txt
    │
    ├─code
    │  └─__pycache__
    │          chromosome.cpython-36.pyc
    │          GA.cpython-36.pyc
    │          globalManager.cpython-36.pyc
    │          Node.cpython-36.pyc
    │          nodeManager.cpython-36.pyc
    │          Population.cpython-36.pyc
    │          test.cpython-36.pyc
    │          test2.cpython-36.pyc
    │
    ├─mtsp_nsga_ii
    │  ├─code
    │  │      chromosome.py
    │  │      ga.py
    │  │      node.py
    │  │      nodemanager.py
    │  │      nsga_ii.py
    │  │      repeat_test.py
    │  │
    │  └─data
    │          mtsp100.txt
    │          mtsp150.txt
    │          mtsp51.txt
    │          pr152.txt
    │          pr226.txt
    │          pr76.txt
    │
    └─summary_figure
            baseline_run_data.json
            ours_run_data.json
            plot_figure.py
            summary.py
            unite.svg   -->
                 
                   
   
