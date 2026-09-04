---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
toc: true
toc_sticky: true
---

My research deals with developing and analyzing novel efficient algorithms for learning and inference, and applying these algorithms in challenging real-world domains. My research interests are mainly related to statistical machine learning and more specifically to the fields of graphical models and deep learning. Deep learning methods attempt to model high-level abstractions in data by using a deep graph with multiple processing layers, composed of multiple linear and non-linear transformations. As often pointed out, the same machine learning models and algorithms can be applied in many different research areas. In my research I concentrate on developing and analyzing those algorithms in the context of classical [machine learning tasks](/publications/#topic) (classification, regression, clustering, dimensionality reduction, etc.) and applying them to a large variety of [real-world applications](/publications/#topic) (computer vision, language processing, audio processing, medical imaging, etc.).

------------------------------------------------------------------------

### Selected Projects

- [Deep learning classification with noisy labels](#noisy)
- [Confidence calibration](#calib)
- [Domain adaptation](#adapt)
- [Deep clustering](#cluster)
- [Multi-document summarization](#mds)
- [Message-passing algorithms for MIMO wireless communication](#mimo)
- [Non-parametric differential entropy estimation  
  ](#npee)
- [LDPC serial scheduling](#ldpc)
- [Neighborhood Components Analysis (NCA)](#nca)
- [Mixture of Gaussians, distance and simplification](#mog)

<span id="noisy"></span>

------------------------------------------------------------------------

**Deep learning classification with noisy labels.** The availability of large data sets has enabled neural networks to achieve impressive recognition results. However, the presence of inaccurate or inconsistent class labels is known to deteriorate the performance of even the best classifiers in a broad range of classification problems. Noisy labels also tend to be more harmful than noisy features. In a line of projects, we defined neural network architectures and training procedures that can explicitly address training data with unreliable labels.

- [Learning probabilistic fusion of multilabel lesion contours.](https://www.eng.biu.ac.il/goldbej/files/2020/01/Gal_isbi_2020.pdf) ISBI, 2020.
- [A soft STAPLE algorithm combined with anatomical knowledge.](https://www.eng.biu.ac.il/goldbej/files/2019/07/miccai_2019.pdf) MICCAI, 2019.
- [Soft labeling by distilling anatomical knowledge for improved MS lesion segmentation.](https://www.eng.biu.ac.il/goldbej/files/2019/03/isbi_eytan_2019.pdf) ISBI, 2019.
- [Training neural networks based on unreliable human annotation of medical images](https://www.eng.biu.ac.il/goldbej/files/2018/01/ISBI_2018_Yair.pdf) ISBI, 2018.
- [Training deep neural-networks using a noise adaptation layer.](https://www.eng.biu.ac.il/goldbej/files/2012/05/ICLR2017.pdf) ICLR, 2017.
- [Multi-view probabilistic classification of breast microcalcifications.](https://www.eng.biu.ac.il/goldbej/files/2012/05/TMI_2016_alan.pdf) IEEE TMI, 2016.
- [A semisupervised approach for language identification based on ladder networks.](https://www.eng.biu.ac.il/goldbej/files/2012/05/Odyssey_2016_paper.pdf) *Odyssey, 2016.*
- [Training deep neural-networks based on unreliable labels.](https://www.eng.biu.ac.il/goldbej/files/2012/05/icassp_2016_Alan.pdf) ICASSP, 2016.
- [Combining soft decisions of several unreliable experts.](https://www.eng.biu.ac.il/goldbej/files/2012/05/ICASSP_2016_Jacob.pdf) ICASSP, 2016.

<span id="calib"></span>

**Confidence calibration.** Performance alone is not sufficient. Accurately assessing the confidence of a prediction is important in a wide range of applications, including medical diagnosis, weather forecasting and autonomous driving. Hence, there is a need to calibrate the confidence information reported by the network. We addressed this problem in the contexts of classification, regression and prediction sets.

- [Conformal nucleus sampling](https://www.eng.biu.ac.il/goldbej/files/2023/05/Shauli_ACL_2023.pdf) Findings of ACL, 2023.
- [Calibration of a regression network based on the predictive variance with applications to medical images](https://www.eng.biu.ac.il/goldbej/files/2023/04/LIor_ISBI_2023.pdf), (ISBI) 2023.
- [Network calibration by temperature scaling based on the predicted confidence,](https://www.eng.biu.ac.il/goldbej/files/2022/09/Eusipco_2022_Lior.pdf) EUSIPCO, 2022.
- [Calibration of medical imaging classification systems with weight scaling](https://www.eng.biu.ac.il/goldbej/files/2022/09/Lior_MICCAI_2022.pdf), MICCAI, 2022.
- [Network calibration by class-based temperature scaling](https://www.eng.biu.ac.il/goldbej/files/2022/01/Lior_Frenkel_Eusipco_2021.pdf), EUSIPCO, 2021.

<span id="adapt"></span>

**Domain adaptation.** The application of deep learning systems to real-world problems is hindered by the drop in performance when a network trained on data from one domain is applied to data from a different domain. The issue of domain shift is particularly critical in medical imaging where the accuracy of a model trained on data from one medical facility decreases when applied to data from a different site.

- [PLPP: A pseudo labeling post-processing strategy for unsupervised domain adaptation,](https://www.eng.biu.ac.il/goldbej/files/2023/07/ISBI_2023_Tomer.pdf)   *ISBI,* 2023.
- [PLST: A pseudo-labels with a smooth transition Strategy for medical site adaptation](https://www.eng.biu.ac.il/goldbej/files/2023/08/Tomer_MICCAI_2023_.pdf), DART, 2023.
- [Supervised domain adaptation using gradient transfer for improved medical image analysis,](https://www.eng.biu.ac.il/goldbej/files/2022/09/Shaya_dart_2022.pdf)  DART, 2022.
- [Unsupervised site adaptation by intra-site variability alignment](https://www.eng.biu.ac.il/goldbej/files/2022/09/Shaya_shira_dart_2022.pdf),  DART, 2022.
- [Adaptation of a multisite network to a new clinical site via batch-normalization similarity](https://www.eng.biu.ac.il/goldbej/files/2022/03/Shira_isbi_2022.pdf), I*SBI,* 2022.
- [Transfer learning with a layer-dependent regularization for medical image segmentation](https://www.eng.biu.ac.il/goldbej/files/2021/08/MLMI_Nimrod_2021.pdf), MLMI, 2021.
- [Transfer learning via parameter regularization for medical image segmentation,](https://www.eng.biu.ac.il/goldbej/files/2021/08/Nimrod_eusipco_2021.pdf) *EUSIPCO,* 2021.

<span id="cluster"></span>

**Deep clustering.** Clustering is one of the most fundamental techniques in unsupervised machine learning. Applying k-means methods to high-dimensional data is problematic. Deep learning methods are expected to automatically discover the most suitable non-linear representations for a specified task.

- [An entangled mixture of variational autoencoders approach to deep clustering](https://www.eng.biu.ac.il/goldbej/files/2023/02/Neuro_avi.pdf), Neurocomputing, 2023.
- [K-Autoencoders deep clustering.](https://www.eng.biu.ac.il/goldbej/files/2020/02/ICASSP_2020_Yaniv.pdf) ICASSP, 2020.
- [Deep clustering based on a mixture of autoencoders.](https://www.eng.biu.ac.il/goldbej/files/2019/08/MLSP_Shlomi.pdf) MLSP, 2019.
- [Clustering-driven deep embedding with pairwise constraints](https://www.eng.biu.ac.il/goldbej/files/2021/09/Hadar_2018.pdf). IEEE Computer Graphics and Applications, 2019.

** **

**<span id="mds"></span>**

**Multi-document summarization.** Common information needs are most often satisfied by multiple texts rather than by a single one. Accordingly, there is a rising interest in MultiDocument Summarization (MDS) — generating a summary for a set of topically-related documents. Inherently, MDS needs to address, either explicitly or implicitly, several subtasks embedded in this summarization setting. These include salience detection, redundancy removal, and text generation.

- <span class="fontstyle0">[Peek across: Improving multi-document modeling via cross-document question-answering](https://www.eng.biu.ac.il/goldbej/files/2023/05/Avi_ACL_2023.pdf), ACL 2023.</span>
- [A proposition-level clustering approach for multi-document summarization](https://www.eng.biu.ac.il/goldbej/files/2022/07/naccl_ori_2022.pdf), NAACL, 2022.
- [Summary-source proposition-level alignment: task, datasets and supervised baseline](https://www.eng.biu.ac.il/goldbej/files/2021/11/Ori_CoNLL_2021.pdf), CoNLL, 2021.

<span id="mimo"></span>  
**Message-Passing Algorithms for MIMO Wireless Communication.** The detection problem for MIMO communication systems is known to be NP-hard. The factor graph that corresponds to this problem is very loopy; in fact, it is a complete graph. Hence, a straightforward application of the Belief Propagation (BP) algorithm yields very poor results. We have developed several methods that either modify the cost function we want to optimize or modify the BP messages in such a way that the BP algorithm yields improved performance. One approach is based on an optimal tree approximation of the Gaussian density of the unconstrained linear system. The finite-set constraint is then applied to obtain a cycle-free discrete distribution. Another approach is based on two-dimensional Gaussian projections and a third method is based on imposing priors on the BP messages.

- [Improved MIMO detection based on successive tree approximations](https://www.eng.biu.ac.il/~goldbej/papers/ISIT_2013.pdf) . ISIT, 2013. [C code  
  ](https://www.eng.biu.ac.il/~goldbej/papers/MIMO_source_files.rar)
- [Iterative tomographic solution of integer least squares problems with applications to MIMO detection.](https://www.eng.biu.ac.il/~goldbej/papers/JSTSP_2011.pdf) IEEE Journal of Selected Topics in Signal Processing, 2011.
- [MIMO detection for high-order QAM based on a Gaussian tree approximation.](https://www.eng.biu.ac.il/~goldbej/papers/IEEE_IT_2011.pdf) IEEE Trans. Information Theory, 2011.
- [Pseudo prior belief propagation for densely connected discrete graphs.](https://www.eng.biu.ac.il/~goldbej/papers/ITW_2010.pdf) IEEE Information Theory Workshop (ITW), 2010.
- [A Gaussian tree approximation for integer least-squares.](https://www.eng.biu.ac.il/~goldbej/papers/NIPS_2009.pdf) NIPS, 2009.

<span id="npee"></span>

**Non-parametric Differential Entropy Estimation.** Estimating the differential entropy given only sampled points without any prior knowledge of the distribution is a difficult task. We proposed the Meann-NN estimator for the main information theoretic measures such as differential entropy, mutual information and KL-divergence. The Mean-NN estimator is related to classical k-NN entropy estimations. However, Unlike the k-NN based estimator, the Mean-NN entropy estimator is a smooth function of the given data points and is not sensitive to small perturbations in the values of the data. Hence, it can be used within optimization procedures that are based on computing the derivatives of the cost function we optimize. We demonstrated the usefulness of the Mean-NN entropy estimation technique on the ICA problem, on clustering and on supervised and unsupervised dimensionality reduction.

- [Dimensionality reduction based on non-parametric mutual information.](https://www.eng.biu.ac.il/~goldbej/papers/NEURO_2012.pdf) Neurocomputing 2012.
- [Unsupervised Feature Selection based on Non-Parametric Mutual Information.](https://www.eng.biu.ac.il/~goldbej/papers/MLSP_2012.pdf) MLSP, 2012.
- [A nonparametric information theoretic clustering algorithm. ](https://www.eng.biu.ac.il/~goldbej/papers/icml_2010.pdf) ICML, 2010.
- [ICA based on a smooth estimation of the differential entropy.](https://www.eng.biu.ac.il/~goldbej/papers/nips_2008.pdf) NIPS 2008.

<span id="ldpc"></span>

**LDPC Serial Scheduling.** LDPC is decoded by running an iterative belief-propagation algorithm over the factor graph of the code. In the traditional message passing schedule, in each iteration all the variable nodes, and subsequently all the factor nodes, pass new messages to their neighbors. We showed that serial scheduling, in which messages are generated using the latest available information, significantly improves the convergence speed in terms of the number of iterations. It was observed experimentally in several studies that the serial schedule converges in exactly half the number of iterations compared to the standard parallel schedule. We provided a theoretical motivation for this observation by proving it for single-path graphs. Joint work with Haggai Kfir, Eran Sharon and [Simon Litsyn](http://www.eng.tau.ac.il/~litsyn/).

- [Serial schedules for belief-propagation: analysis of convergence time.](https://www.eng.biu.ac.il/~goldbej/papers/IT_Kfir_2008.pdf) IEEE Trans. on Information Theory, 2008.
- [Efficient serial message-passing schedules for LDPC decoding.](https://www.eng.biu.ac.il/~goldbej/papers/IT_Sharon_2007.pdf) IEEE Trans. on Information Theory, 2007.
- [An efficient message-passing schedule for LDPC decoding.](https://www.eng.biu.ac.il/~goldbej/papers/engisrael.pdf) Proc. Electrical and Electronic Engineers in Israel, 2004.

<span id="nca"></span>

**Neighbourhood Components Analysis (NCA)** is a method for learning a Mahalnobis distance measure for k-nearest neighbors (kNN). In particular, it finds a distance metric that maximizes the leave-one-out error on the training set for a stochastic variant of kNN. NCA can also learn a low-dimensional linear embedding of labeled data for data visualization and for improved kNN classification speed. Unlike other methods, this classification model is non-parametric without any assumption on the shape of the class distributions or the boundaries between them. Joint work with [Sam Roweis](http://www.cs.nyu.edu/~roweis/), [Geoffrey Hinton ](http://www.cs.toronto.edu/~hinton/) and [Ruslan Salakhutdinov](http://www.cs.cmu.edu/~rsalakhu/).

[Neighbourhood Component Analysis.](https://www.eng.biu.ac.il/~goldbej/papers/ncanips.pdf) NIPS 2004. [matlab code](http://www.ics.uci.edu/~fowlkes/software/nca/) [C code](https://www.eng.biu.ac.il/~goldbej/papers/nca.zip)

<span id="mog"></span>

**Mixture of Gaussians, Distance and Simplification.** The Mixture of Gaussians (MoG) is one of the simplest graphical models. It is a flexible and powerful parametric framework for unsupervised data grouping. We suggested several approaches for computing meaningful distances between two MoGs and for MoG model simplification. The Unscented Transform is traditionally used for generalized Kalman filters in non-linear dynamical systems. We proposed the usage of the Unscented Transform for computing the KL divergence between two MoGs and for model simplification.

[Simplifying mixture models using the unscented transform.](https://www.eng.biu.ac.il/~goldbej/papers/TPAMI-2008-08.pdf) IEEE PAMI, 2008.  
[A distance measure between GMMs based on the unscented transform and its application to speaker recognition.](https://www.eng.biu.ac.il/~goldbej/papers/eurospeech05.pdf) Eurospeech, 2005.  
[Hierarchical clustering of a mixture model.](https://www.eng.biu.ac.il/~goldbej/papers/mognips.pdf) NIPS, 2004.  
[An efficient similarity measure based on approximations of KL-divergence between two Gaussian mixtures.](https://www.eng.biu.ac.il/~goldbej/papers/iccv031.pdf) ICCV, 2003.
