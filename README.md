# GRaSP Project Repository
Materials, code, datasets, etc., for the GRaSP project

The contents of this repository are for this paper:

Lam, W. Y., Andrews, B., & Ramsey, J.. (2022). Greedy Relaxations of the Sparsest Permutation Algorithm. Uncertainty in Artificial Intelligence, Accepted.

On arXiv: https://arxiv.org/abs/2206.05421

# Python Translation

A scalable Python translation of GRaSP-2 for the linear, Gaussian case is available here:

https://github.com/bja43/GRaSP

# Simulation Datasets

All of the simulation dataset used in our paper are available on Box here:

https://cmu.box.com/s/h2e6ab9a62u2yu7kytg5ejsbyijsoc1u

This includes all dataset in tabular form plus all true graphical models for the dataset
to compare results to. We include tabular data (instead of covaraince matrices) because we 
realize some tools require it.

# Simulation Results

All simulation results reported in the figures in our paper may be downloaded from this 
GitHub site; please download this file:

https://github.com/cmu-phil/grasp/blob/main/files/grasp_results.zip

This includes all specific algorithms results for all runs in our paper, plus the summaries
of these results in the Comparison.txt files, comparing to the true DAG. We also include
summaries comparing to the true CPDAG, here:

https://github.com/cmu-phil/grasp/blob/main/files/grasp_results_comparing_to_true_CPDAG.zip

The latter information is what is plotted in our simulation Figures.

All of these results were generated using the algcomparison facility in Tetrad--

Ramsey, J. D., Malinsky, D., & Bui, K. V. (2020). algcomparison: comparing the performance of 
graphical structure learning algorithms with TETRAD. Journal of Machine Learning Research, 21(238), 1-6.

# Ground truth Independence Models (IMs)

The 4-node ground truth models may be downloaded from their source as referenced in our paper.
The 5-node path-canceling models in Appendix F may be downloaded from this repository
in this file:

https://github.com/cmu-phil/grasp/blob/main/files/udags5.zip

# Real Datasets Repository

A number of real datasets have been formatted with ground truth for easy analysis using 
causal discovery algorithms in this GitHub repository

https://github.com/cmu-phil/example-causal-datasets

Users are encouraged to analyze these dataset using own algorithms.

# PC/FGES/GRaSP2/SP on a subset of these real datasets.

A slide presentation for these may be downloaded from this repository, here:

https://github.com/cmu-phil/grasp/blob/main/files/SomeRealDataExamplesForGrasp.pdf

GRaSP-0 and GRaSP-1 results will be added to these slides.

# Code

All Java code for our paper is included in the granch 'grasp-pub' of the GitHub 
repository for the Tetrad project,

https://github.com/cmu-phil/tetrad

The specific code used to generate the examples for our paper is in this branch:

https://github.com/cmu-phil/tetrad/tree/grasp-pub

The GRaSP class in the granch 'grasp-pub' is here:

https://github.com/cmu-phil/tetrad/blob/grasp-pub/tetrad-lib/src/main/java/edu/cmu/tetrad/search/Grasp.java

The underlying scoring class in the branch 'grasp-pub' is here:

https://github.com/cmu-phil/tetrad/blob/grasp-pub/tetrad-lib/src/main/java/edu/cmu/tetrad/search/TeyssierScorer.java

Some other classes in this branch are also used, as referenced in the import statements of the above classes.

Tetrad uses Maven to build the project, which is easily set up in the IntelliJ app, nere:

https://www.jetbrains.com/idea/

Instructions for setting up the project in IntelliJ may be found in the Wiki for the Tetrad project, here:

https://github.com/cmu-phil/tetrad/wiki/Setting-up-Tetrad-in-IntelliJ-IDEA

# Tetrad Jar

The Tetrad app build used to generate the examples above is in the Maven Cental Repository and may be downloaded using this link:

https://s01.oss.sonatype.org/content/repositories/releases/io/github/cmu-phil/tetrad-gui/7.1.0/tetrad-gui-7.1.0-launch.jar

To launch the Tetrad app, install a Java JDK (default version 1.8), then type in a terminal window:

java -Xmx[#gigbates-ram]g -jar [path-to-the-above-jar-file].jar

This should work on all platforms; if not, let us know.

