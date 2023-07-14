# LMANStat

## Introduction
This package contains the dataset named named "Large-scale Multi-layer Academic Networks (LMANStat)" and the code in Gao, Zhang, Pan, and Wang's paper titled "Large-scale Multi-layer Academic Networks Derived from Statistical Publications".

We highly welcome you to utilize our data and code for your research work. If you use our data and code, please ensure to cite our paper accurately as follows:

@article{gao2023large,
  title={Large-scale Multi-layer Academic Networks Derived from Statistical Publications},
  author={Gao, Tianchen and Zhang, Yan and Pan, Rui and Wang, Hansheng},
  journal={Scientific Data},
  year={2023},
  publisher={Nature Publishing Group},
  doi={10.xxxxx/xxxxx}
}

## LMANStat Dataset Source
The dataset comprises two Excel files that contain the author and paper information (including author unique id, paper unique id, and the corresponding attributes) and eight CSV files that depict the edge list. Specifically, The record of the papers can be found in the file {\it Paper_information.xlsx}, which contains the basic information of the papers. 

Each row of the table represents a unique academic paper and is identified by the unique field {\it Paper_unique_id}. The file {it Author_information.xlsx} contains the attributes of each unique author, including the name, institution, country, and research interest and the authors can be uniquely identified by the field {\it Author_unique_id}. The eight CSV files with the name {\it Edgelist\_X.csv} (X is the name of each network) correspond to the edge lists of the seven networks described above. The fields {\it (Target and Source)} in each row of the edge data files represent an edge in the corresponding network, with the field {\it Year} indicating the time in which the edge is formed. The specific meaning of each edge is detailed in Table \ref{tab:intro_network}. By filtering according to the {\it Year} field, one can easily construct the academic network dynamically. 

The nodes in files Edgelist_citation.csv, {\it Edgelist_co_citation.csv}, {\it Edgelist\_collaboration.csv}, {\it Edgelist\_author\_citation.csv}, and {\it Edgelist\_author\_paper.csv} are {\it Paper\_unique\_id} or {\it Author\_unique\_id} while the nodes in files {\it Edgelist\_journal\_citation.csv}, {\it Edgelist\_co\_institution.csv}, and {\it Edgelist\_keyword\_co\_occurrence.csv} are the journal names, institution names, and keywords, respectively.
