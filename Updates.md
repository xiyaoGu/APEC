**updates on 2020-03-25**

    APEC on pypi updated to 1.2.2.

**updates on 2020-03-25**

    APEC on pypi updated to 1.2.0.

**updates on 2019-11-18**

    APEC on pypi updated to 1.1.0.11, debugged algorithm for generate.differential_feature().

**updates on 2019-11-08**

    APEC on pypi updated to 1.1.0.10.
    APEC uses p-value to filter potential super enhancers.

**updates on 2019-11-03**

    APEC on pypi updated to 1.1.0.9.
    APEC doesn't filter accessons before clustering.

**Updates on 2019-07-17**

    APEC on pypi updated to 1.1.0.8, optimized algorithm for cell-cell corrlation heatmap.

**Updates on 2019-07-02**

    APEC on pypi updated to 1.1.0.7, optimized algorithm for trajectory construction and differential gene search.

**Updates on 2019-06-23**

    APEC on pypi updated to 1.1.0.6, debugged algorithm for clustering.cluster_comparison().

**Updates on 2019-06-19**

    APEC on pypi updated to 1.1.0.5, debugged algorithm for plot.correlation().

**Updates on 2019-06-17**

    Fixed several bugs, APEC on pypi updated to 1.1.0.4.

**Updates on 2019-06-16**

    Fixed several bugs, APEC on pypi updated to 1.1.0.3.

**Updates on 2019-06-14**

    APEC update to v1.1.0: all important parts (cell clustering, trajectory construction, feature analysis, etc.) are packaged and uploaded to Pypi. Users can install APEC by "pip install APEC". If users already have the fragment count matrix (for example, the CellRanger result of 10X data), please use APEC functions in Ipython, Jupyter-notebook or python script directly. If users want to get fragment count matrix from raw fastq data files, please run "bash APEC_prepare_steps.sh" with proper parameters.

**Updates on 2019-06-12**

    Using new algorithm to estimate gene score form relevant accessons.

**Updates on 2019-06-09**

    Cluster_byAccesson.py reuses KNN graph to build accesson matrix, due to the memory requirement for large datesets.

**Updates on 2019-05-30**

    APEC was updated to version 1.0.6:
        The fragment count matrix is stored in mtx format file, instead of csv format file.
        When building accesson matrix, cluster_byAccesson.py won't use KNN graph anymore, which make clustering result more stable.
        README.md file was updated.

**Updates on 2019-05-28**

    Fit the problem that cluster_byMotif.py cannot be used on the count matrix of mtx format (i.e. filtered_reads.mtx).
    Also, in cluster_byMotif.py we adopted MulticoreTSNE instead of sklearn.manifold.TSNE

**Updates on 2019-05-11**

    Update generate_differential_markers.py:
        If '--motif' set to 'no', 'projec/result/deviation_chromVAR.csv' is not required.

**Updates on 2019-04-27**

    We corrected the error on line 388 of subroutines.py

**Updates on 2019-04-25**

    We corrected the error on line 123 of cluster_byAccesson.py.

**Updates on 2019-04-21**

    There is a problem with the TSNE package in scikit-learn when analyzing a large number of cells.
    Now We use mulitcore-tsne in cluster_byAccesson.py to analyze datasets containing more than 10,000 cells.
