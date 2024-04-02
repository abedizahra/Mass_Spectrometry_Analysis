**Biomarker discovery using machine learning techniques for mass spectrometry data**


## Installation
```r{}
# Loading/installing packages
packages <- read.table("packages.txt", header = F)
suppressMessages({
if (!requireNamespace("BiocManager", quietly = TRUE)) {
install.packages("BiocManager")
}
for (package in packages$V1) {
if (!requireNamespace(package, quietly = TRUE)) {
BiocManager::install(package)
require(package, character.only = TRUE)
} else {
require(package, character.only = TRUE)
}
}
})
```
