# This is the data and code repository for manuscripts (Coding-PTMs) submitted to ASE 2024. If you have any questions, please contact the first author of the published version.

## Datasets
We first give the datasets under the Sample+split/MYVDCWEDATA folder shown above, these datasets were processed well by previous researchers. See the next **Acknowledgment**.

## Code Pre-trained Models
The code pre-trained models used in this paper are all come from HuggingFace, we do not give the models since it is too large and easy to obtain.

## Instructions
1. The RQ1 folder shows the results of RQ1 in the paper. You can directly run the jupyter notebook to obtain the RQ1 results in the paper. About the performance values, you can download the code zip file in the RQ1 folder, then unzip it under the environment and run the setcode file to collect the performance values.

2. The RQ2 folder shows the results of code embeddings, i.e., corresponding to the RQ2 in the paper. You can directly run the jupyter notebook to obtain the figure.

3. The RQ3 folder includes the following content. First, the process of building the new code embedding dataset is shown, including extracting code embedding metrics (run the features notebook) and making tags (run the tag notebook). Then the performance of the recommendation model is trained and tested on the constructed dataset (run the tag1-auc notebook). Finally, it is evaluated in a real-world scenario (run the scene notebook). In addition, running the feature-importance notebook can get the feature importance analysis of the code metrics of the established recommendation model.

4. The Sample+split folder is where we sample the original dataset to obtain more differently distributed vulnerability datasets to proceed with our research. Download all the files and run the notebook can obtain the same datasets as our paper, and then move the dataset into the dataset folder of the unzip code file, finally, you can move step 1 to run the code.


## Environment
transformers 4.42.4

torch 1.8.0+cu111

Python 3.9.13 

## Acknowledgment 

Thank the following works for providing the original repository to facilitate the collection of the data sets required for this paper. At the same time, we gave the address of the raw datasets depository.

Datasets Devign for code vulnerability detection Devign: https://github.com/microsoft/CodeXGLUE/tree/main/Code-Code/Defect-detection and the raw dataset comes from the paper Devign: Effective Vulnerability Identification by Learning Comprehensive Program Semantics via Graph Neural Networks. 

Datasets Reveal for code vulnerability detection Reveal: https://github.com/VulDetProject/ReVeal, which comes from the paper Deep Learning Based Vulnerability Detection: Are We There Yet? 

Datasets CWE119 and CWE399: https://github.com/CGCL-codes/VulDeePecker and these two datasets come from the paper Vuldeepecker: A deep learning-based system for vulnerability detection.
