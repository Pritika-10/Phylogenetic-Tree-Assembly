# Phylogenetic Tree Assembly and Updation Workflow

In this research, I propose two novel alignment-free, pairwise distance calculation methods based on k-mers and locality-sensitive hashing. Additionally, I have introduced a machine learning-based mechanism for phylogenetic tree construction. These innovative approaches aim to enhance the efficiency and accuracy of genetic distance calculations.

The proposed tree construction method utilizes a modified version of k-medoids, which demonstrates significantly improved performance compared to traditional phylogenetic tree construction techniques. As the final aspect of this research, I developed a numerical neural network to efficiently update the phylogenetic tree.

In summary, this work presents  methodologies for genetic distance calculation, phylogenetic tree construction, and dynamic tree updating, collectively advancing the field of computational phylogenetics.


## Introduction

The phylogenetic tree, also known as an evolutionary tree, is a branching diagram that illustrates the evolutionary relationships among various organisms. It organizes species based on genetic similarities and calculates their genetic distances to define these relationships. Phylogenetic trees serve as a foundational component in many areas of bioinformatics research, providing critical insights into evolutionary biology, comparative genomics, and molecular phylogenetics.

![Phylogenetic-Tree-Construction](https://raw.githubusercontent.com/ngimhana/Phylogenetic_tree_construction/master/Diagram/phylogenetic-tree.png)


## **Methodology**  

### **1. Novel Alignment-Free Pairwise Distance Calculation**
- **K-mers-Based Approach**:  
  K-mers, which are fixed-length substrings of genetic sequences, are used to represent DNA sequences in a compressed form. This method avoids the computational burden of traditional sequence alignment by comparing k-mer frequencies or patterns directly.  
- **Locality-Sensitive Hashing (LSH)**:  
  LSH is employed to hash similar sequences into the same bucket with high probability. This drastically reduces the computational overhead by focusing only on relevant sequence comparisons, making the process faster and scalable for large datasets.  

### **2. Machine Learning-Based Phylogenetic Tree Construction**
- **Modified K-Medoids Clustering**:  
  The genetic distances derived from the alignment-free methods are used as input for clustering. A modified version of the k-medoids algorithm is applied to group sequences based on their similarities, ensuring better performance and more accurate tree construction than traditional clustering methods.  
- **Tree Assembly**:  
  The clustering results are used to construct the phylogenetic tree, with each cluster forming a branch of the tree.  

### **3. Numerical Neural Network for Tree Updation**
- A numerical neural network is implemented to update the phylogenetic tree dynamically as new data becomes available. This ensures the tree remains accurate and reflective of the latest sequence data.  

![Phylogenetic Tree Construction Methodology](https://raw.githubusercontent.com/ngimhana/Phylogenetic_tree_construction/master/Diagram/mehodology.png)  
