# Dimensionality Reduction

Dimensionality reduction is simply, the process of reducing the dimension of your feature set. Your feature set could be a dataset with a hundred columns (i.e features) or it could be an array of points that make up a large sphere in the three-dimensional space. Dimensionality reduction is bringing the number of columns down to say, twenty or converting the sphere to a circle in the two-dimensional space.

___The Curse of Dimensionality___

The curse of dimensionality refers to all the problems that arise when working with data in the higher dimensions, that did not exist in the lower dimensions.
As the number of features increase, the number of samples also increases proportionally. The more features we have, the more number of samples we will need to have all combinations of feature values well represented in our sample.

As the number of features increases, the model becomes more complex. The more the number of features, the more the chances of overfitting. A machine learning model that is trained on a large number of features, gets increasingly dependent on the data it was trained on and in turn overfitted, resulting in poor performance on real data, beating the purpose.

Avoiding overfitting is a major motivation for performing dimensionality reduction. The fewer features our training data has, the lesser assumptions our model makes and the simpler it will be. But that is not all and dimensionality reduction has a lot more advantages to offer, like:
* Less misleading data means model accuracy improves.
* Less dimensions mean less computing. Less data means that algorithms train faster.
* Less data means less storage space required.
* Less dimensions allow usage of algorithms unfit for a large number of dimensions
* Removes redundant features and noise.

![image](https://user-images.githubusercontent.com/54405639/83546855-f8cce180-a51e-11ea-8d11-b2b493bc6f81.png)

### ___Linear Dimensionality Reduction Methods___

The most common and well known dimensionality reduction methods are the ones that apply linear transformations, like:

1. ___PCA (Principal Component Analysis)___: Popularly used for dimensionality reduction in continuous data, PCA rotates and projects data along the direction of increasing variance. The features with the maximum variance are the principal components.

2. ___Factor Analysis___: A technique that is used to reduce a large number of variables into fewer numbers of factors. The values of observed data are expressed as functions of a number of possible causes in order to find which are the most important. The observations are assumed to be caused by a linear transformation of lower dimensional latent factors and added Gaussian noise.

3. ___LDA (Linear Discriminant Analysis)___: Projects data in a way that the class separability is maximised. Examples from same class are put closely together by the projection. Examples from different classes are placed far apart by the projection.

PCA orients data along the direction of the component with maximum variance whereas LDA projects the data to signify the class separability.

### ___Non-linear Dimensionality Reduction Methods___

Non-linear transformation methods or manifold learning methods are used when the data doesn’t lie on a linear subspace. It is based on the manifold hypothesis which says that in a high dimensional structure, most relevant information is concentrated in small number of low dimensional manifolds. If a linear subspace is a flat sheet of paper, then a rolled up sheet of paper is a simple example of a nonlinear manifold. Informally, this is called a Swiss roll, a canonical problem in the field of non-linear dimensionality reduction. Some popular manifold learning methods are:

1. ___Multi-dimensional scaling (MDS)___: A technique used for analyzing similarity or dissimilarity of data as distances in a geometric spaces. Projects data to a lower dimension such that data points that are close to each other (in terms if Euclidean distance) in the higher dimension are close in the lower dimension as well.

2. ___Isometric Feature Mapping (Isomap)___: Projects data to a lower dimension while preserving the geodesic distance (rather than Euclidean distance as in MDS). Geodesic distance is the shortest distance between two points on a curve.

3. ___t-distributed Stochastic Neighbor Embedding (t-SNE)___: Computes the probability that pairs of data points in the high-dimensional space are related and then chooses a low-dimensional embedding which produce a similar distribution.

_[Link](https://towardsdatascience.com/dimensionality-reduction-toolbox-in-python-9a18995927cd)_
