# Object-based Neuro Fuzzy Clustering (ONFC)
![Tensorflow](https://img.shields.io/badge/Implemented%20in-Tensorflow-green.svg) <br>

- Object clustering framework using latent variables of trained fully convolutional neural networks.
- The framework categorizes objects from pictures in an unsupervised. 
- Objects and latent features are extracted via image processing functions from OpenCV given the results from segmentation.
- Extract information are processed and evaluated by fuzzy inference for similarity analysis.
- Similarity results serve as basis for clustering.

| ![sample](https://raw.githubusercontent.com/cjuliani/tf-object-neuro-fuzzy-clustering/main/sample.PNG) |
|:--:|
| *Example of an RGB micro-photograph of mineral grains with corresponding annotations (A) (morphological erosion applied; background in white) and pixel predictions (P). Scanning-Electron-Microscope Backscatter images indicated three different minerals in this sample: grains marked by black squares are mostly apatite grains, yellow dots are monazites, and unmarked grains are zircons.*

| ![similarity results](https://raw.githubusercontent.com/cjuliani/tf-object-neuro-fuzzy-clustering/main/similarity.PNG) |
|:--:|
| *Examples of probabilistic similarity measures of mineral grains identified by U-Net; average values are indicated above each object frame and presented in decreasing order.*

| ![clusters](https://raw.githubusercontent.com/cjuliani/tf-object-neuro-fuzzy-clustering/main/clusters.PNG) |
|:--:|
| *Examples of clusters (up to 10 objects shown per row only) obtained from ONFC (a), and several of uncategorized grains (b). Opaque minerals tend to reflect more light.*
