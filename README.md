# Object-based Neuro Fuzzy Clustering (ONFC)
![Tensorflow](https://img.shields.io/badge/Implemented%20in-Tensorflow-green.svg) ![Python 3.6](https://img.shields.io/badge/python-3.6-blue.svg?style=plastic) <br>

### TLDR:
- Object clustering framework using latent variables of trained fully convolutional neural networks.
- The framework categorizes objects in an unsupervised manner for pattern discovery.

### Description:
ONFC is an algorithm processing the latent characteristics of fully convolutional networks (FCNs) to group objects with analogous properties. We demonstrate its application to microscopic grains whose predominant attributes (e.g. composition and intergranular structures) are difficult to categorize. Clustering is carried out in 3 steps: (1) extract feature patterns per object from a trained FCN, (2) find the most similar patterns by fuzzy inference, and (3) decide on surrogate classes of the corresponding patterns given the similarity relations. The last step links the similarity analysis with clustering, which is refined by a weighting scheme involving the relevance of latent variables in classification.

*Keywords: clustering, similarity, fuzzy inference, convolutional neural networks, segmentation*

| <img src="https://raw.githubusercontent.com/cjuliani/tf-object-neuro-fuzzy-clustering/main/sample.PNG" width="65%"> |
|:--:|
| Example of an RGB micro-photograph of mineral grains with corresponding annotations (A) (morphological erosion applied; background in white) and pixel predictions (P). Scanning-Electron-Microscope Backscatter images indicated three different minerals in this sample: grains marked by black squares are mostly apatite grains, yellow dots are monazites, and unmarked grains are zircons.

| <img src="https://raw.githubusercontent.com/cjuliani/tf-object-neuro-fuzzy-clustering/main/similarity.PNG" width="85%"> |
|:--:|
| Examples of probabilistic similarity measures of mineral grains identified by U-Net; average values are indicated above each object frame and presented in decreasing order.

| <img src="https://raw.githubusercontent.com/cjuliani/tf-object-neuro-fuzzy-clustering/main/boots.PNG" width="85%"> |
|:--:|
| <img src="https://raw.githubusercontent.com/cjuliani/tf-object-neuro-fuzzy-clustering/main/boots2.PNG" width="85%"> |
|:--:|
| Another examples of probabilistic similarity measures for boots.

| <img src="https://raw.githubusercontent.com/cjuliani/tf-object-neuro-fuzzy-clustering/main/clusters.PNG" width="85%"> |
|:--:|
| Examples of clusters (up to 10 objects shown per row only) obtained from ONFC (a), and several of uncategorized grains (b). Opaque minerals tend to reflect more light.

| <img src="https://raw.githubusercontent.com/cjuliani/tf-object-neuro-fuzzy-clustering/main/feature-centroids-plot.png" width="50%"> |
|:--:|
| Examples of mean activations calculated per object and projected in 3D feature spaces (39 clusters displayed). Features are indicated per axis.

| <img src="https://raw.githubusercontent.com/cjuliani/tf-object-neuro-fuzzy-clustering/main/birds.png" width="70%"> |
|:--:|
| Testing of ONFC on Caltech-UCSD Birds-200-2011 dataset (https://www.vision.caltech.edu/datasets/cub_200_2011/).

