# imKmeans

Improved k-means method, developed by Toyoda and Ikehara(2011), uses mahalanobis distance as similarity between variables. And by using this method, we can determine the number of clusters with AIC and BIC.

## Install

You need `devtools` to install `imKmeans` from GitHub.

```
install.packages("devtools")
```

After install these packages, excute the following in R:

```
library(devtools)
install_github("kosugitti/imKmeans")
```
## Example
```
imKmeans(iris[1:4],4)
```

## Reference
Toyoda H. and Ikehara K. 2011 An improved method using k-means to determine the optimal number of clusters, considering the relations between several variables. The Japanese Journal of Psychology,Vol.82, No.1, pp.32-40.


## Note

AIC and BIC yielded by this function are differ from the result of Toyoda et al.(2011). because of counting the number of free parameters...