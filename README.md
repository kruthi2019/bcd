# bcd
Breast Cancer Detection
MOTIVATION:
To evaluate movtivational factors for pqarticipation in a breast cancer screening program and concurrently examine beliefs regarding carcinoma of the breast held by those women, we took records and datasets from wisconsin diagnostic dataset.
OBJECTIVE:
Breast cancer has been characterised as a heterogeneous disease consisting of many different subtypes. The early diagnosis and prognisiness of a cancer type have become a necessity in cancer research as it can facilitate the subsequent clinical management of patients.
PROBLEM STATEMENT:
Detection of breast cancer in women in early stages that help them to sucessfully overcome it.
REQUIREMENT ANALYSIS:
PLATFORM USED:machine learning
DATASET USED :Wisconsin dataset
LANGUAGE:Python 
IDE:Anaconda

ALGORITHMS:
SVM algorithm
Support Vector Machine” (SVM) is a supervised machine learning algorithm which can be used for both classification or regression challenges. However,  it is mostly used in classification problems. In this algorithm, we plot each data item as a point in n-dimensional space with the value of each feature being the value of a particular coordinate. Then, we perform classification by finding the hyper-plane that differentiate the two classes very well.In Python, scikit-learn is a widely used library for implementing machine learning algorithms, SVM is also available in scikit-learn library and follow the same structure

ID3 algorithm
'Decision tree learning is a method for approximating discrete-valued target functions, in which the learned function is represented by a decision tree. Decision tree learning is one of the most widely used and practical methods for inductive inference'.Decision trees classify instances by traverse from root node to leaf node. We start from root node of decision tree, testing the attribute specified by this node, then moving down the tree branch according to the attribute value in the given set. This process is the repeated at the subtree level.

ID3 ( Learning Sets S, Attributes Sets A, Attributesvalues V) Return Decision Tree.

Begin

Load learning sets first, create decision tree root node 'rootNode', add learning set S into root node as its subset.

For rootNode, we compute Entropy(rootNode.subset) first

If Entropy(rootNode.subset)==0, then rootNode.subset consists of records all with the same value for the categorical attribute, return a leaf node with decision attribute:attribute value;

If Entropy(rootNode.subset)!=0, then compute information gain for each attribute left(have not been used in splitting), find attribute A with Maximum(Gain(S,A)). Create child nodes of this rootNode and add to rootNode in the decision tree.

For each child of the rootNode, apply ID3(S,A,V) recursively until reach node that has entropy=0 or reach leaf node.

End ID3.

