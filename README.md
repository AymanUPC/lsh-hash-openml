# lsh-hash-openml
The OpenML ground-truth for testing the Locality Sensitive Hashing (LSH) algorithm. It includes a sample of matching attributes from 203 datasets which were detected using schema matching.

## Locality Sensitive Hashing (LSH) for blocking attributes
This page is dedicated for the LSH blocking of attributes project by the [DTIM Research Group](http://www.essi.upc.edu/dtim) of the ESSI department, UPC. We provide here the main benchmark gold standards and sources for experimental evaluation of LSH effectiveness over a sample of 203 datasets from [OpenML](https://www.openml.org) data.

## Description
* **OpenML_Sample_Nominal_Attributes.csv:** Stores the information about the nominal attributes from the 203 datasets sample we retrieved from OpenML and their data profile. The columns are described in our paper.
* **OpenML_Sample_Numeric_Attributes.csv:** Stores the information about the numeric attributes from the 203 datasets sample we retrieved from OpenML and their data profile. The columns are described in our paper.
* **OpenML_Sample_Nominal_Attributes_Gold_Standard.csv:** Stores the gold-standard of matching nominal attributes with a similarity score generated by schema matching, where the minimum threshold is 50%.
* **OpenML_Sample_Numeric_Attributes_Gold_Standard.csv.tar.gz:** Stores the gold-standard of matching numeric attributes with a similarity score generated by schema matching, where the minimum threshold is 50%. We compress the CSV file due to its large size.

To retrieve the original datasets from OpenML using the APIs provided by them and the dataset IDs from our CSV files, please refer to the [OpenML API guide](https://openml.github.io/OpenML/Java-guide/).

## Built With

* [Java V8](https://openjdk.java.net/projects/jdk8/)
* [Java OpenML API](https://openml.github.io/OpenML/Java-guide/)
* [Postgres DB](https://www.postgresql.org/)
