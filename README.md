# LMANStat

## Introduction
This package contains the dataset named named "Large-scale Multi-layer Academic Networks (LMANStat)" and the code in Gao, Zhang, Pan, and Wang's paper titled "Large-scale Multi-layer Academic Networks Derived from Statistical Publications".

We highly welcome you to utilize our data and code for your research work. If you use our data and code, please ensure to cite our paper accurately as follows:

Gao, T., Zhang, Y., Pan, R., & Wang, H. (2023). Large-scale Multi-layer Academic Networks Derived from Statistical Publications. Scientific Data. Submission.

## LMANStat Dataset

The dataset comprises two Excel files that contain the author and paper information (including author unique id, paper unique id, and the corresponding attributes) and eight CSV files that depict the edge list. Specifically, The record of the papers can be found in the file *Paper_information.xlsx*, which contains the basic information of the papers. Each row of the table represents a unique academic paper and is identified by the unique field **Paper_unique_id**. The file *Author_information.xlsx* contains the attributes of each unique author, including the name, institution, region, and research interest and the authors can be uniquely identified by the field **Author_unique_id**. 

The eight CSV files with the name *Edgelist_X.csv* (X is the name of each network) correspond to the edge lists of the seven networks described above. The fields **(Target and Source)** in each row of the edge data files represent an edge in the corresponding network, with the field **Year** indicating the time in which the edge is formed. The specific meaning of each edge is detailed in the paper. By filtering according to the **Year** field, one can easily construct the academic network dynamically. 

The nodes in files Edgelist_citation.csv, *Edgelist_co_citation.csv*, *Edgelist_collaboration.csv*, *it Edgelist_author_citation.csv*, and *Edgelist_author_paper.csv* are **Paper_unique_id** or **Author_unique_id** while the nodes in files *Edgelist_journal_citation.csv*, *Edgelist_co_institution.csv*, and *Edgelist_keyword_co_occurrence.csv* are the journal names, institution names, and keywords, respectively.

