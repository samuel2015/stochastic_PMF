Poisson matrix factorization and automatic music tagging
======

Source code for the following paper:
[Codebook-based Scalable Music Tagging with Poisson Matrix Factorization](http://www.ee.columbia.edu/~dliang/publications/LiangPE2014-codebook.pdf) by Dawen Liang, John Paisley and Dan Ellis. 

### What's included:

There are four ipython notebook files, which will help reproduce the experiments in the aforementioned paper:

* **buildVQ_MSD.ipynb**: Build the VQ Codebook for the Million Song Dataset and vector-quantize the MSD and save to disk.

* **processLastfmTags.ipynb**: Process the tagging data from Last.fm and build the vocabulary and bag-of-tags representation and save to disk.

* **tagging_ooc.ipynb**: After building the VQ-histogram and bag-of-tags, this one will reproduce the results from the data saved on the disk.

* **tagging_in_memory.ipynb**: If you have enough memory, you can also save the data from **tagging_ooc.ipynb** and directly fit to the PMF with this notebook.

### Dependencies:
* numpy 
* scipy
* scikit-learn (for evaluation metrics)
* nltk (for tag stemming)
