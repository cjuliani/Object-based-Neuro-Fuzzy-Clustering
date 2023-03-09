# Object-based Neuro Fuzzy Clustering (ONFC)
![Tensorflow](https://img.shields.io/badge/Implemented%20in-Tensorflow-green.svg) <br>

- Object clustering framework using latent variables of trained fully convolutional neural networks.
- The framework categorizes objects in an unsupervised manner for pattern discovery.

| <img src="https://raw.githubusercontent.com/cjuliani/tf-object-neuro-fuzzy-clustering/main/sample.PNG" width="65%"> |
|:--:|
| *Example of an RGB micro-photograph of mineral grains with corresponding annotations (A) (morphological erosion applied; background in white) and pixel predictions (P). Scanning-Electron-Microscope Backscatter images indicated three different minerals in this sample: grains marked by black squares are mostly apatite grains, yellow dots are monazites, and unmarked grains are zircons.*

| <img src="https://raw.githubusercontent.com/cjuliani/tf-object-neuro-fuzzy-clustering/main/similarity.PNG" width="85%"> |
|:--:|
| *Examples of probabilistic similarity measures of mineral grains identified by U-Net; average values are indicated above each object frame and presented in decreasing order.*

| <img src="https://raw.githubusercontent.com/cjuliani/tf-object-neuro-fuzzy-clustering/main/clusters.PNG" width="85%"> |
|:--:|
| *Examples of clusters (up to 10 objects shown per row only) obtained from ONFC (a), and several of uncategorized grains (b). Opaque minerals tend to reflect more light.*

| <img src="https://raw.githubusercontent.com/cjuliani/tf-object-neuro-fuzzy-clustering/main/feature-centroids-plot.png" width="50%"> |
|:--:|
| *Examples of mean activations calculated per object and projected in 3D feature spaces (39 clusters displayed). Features are indicated per axis.*
