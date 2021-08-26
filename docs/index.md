**University of California, Berkeley, Department of Physics**

**PHY188/288: Fall 2021**

Bayesian Data Analysis and Machine Learning for Physical Sciences
====================================================================

Instructor: Uro&#353; Seljak, <useljak@berkeley.edu> <br>
&nbsp; Office hours: I welcome an opportunity to learn from and get to know all my students; thus, I invite you to visit me during my office hours scheduled as follows: Thursday 11:00AM-12:00PM on zoom (see syllabus on bcourses for link) or in person Campbell Hall 359.


GSI: Adrian Bayer, <abayer@berkeley.edu> <br>
&nbsp; Office hours: Tuesday 7:00PM-8:00PM, Physics North 109, or via zoom (email for link).

  
Lecture: <b>Tuesday, Thursday 9:30AM-11:00AM, North Gate 105 </b> <br>
Discussion: <b>Wednesday 1:00PM-2:00PM, Wheeler 204 </b> <br>
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp;  &nbsp; &nbsp; or <b>Wednesday 5:00PM-6:00PM, Cory 241 </b> <br>
Units: <b>4.0</b>

Link to Piazza: <https://piazza.com/berkeley/fall2021/physics188288>

Class Number: 25131

Course Syllabus
---------------

**Learning goals**:
The goal of the course is to get acquainted with modern computational methods used in the physical sciences, including numerical analysis methods, data science and Bayesian statistics. We will introduce a number of concepts that are useful in physical sciences at varying levels of depth. We will cover the main numerical methods used in physical sciences. Most of the statistical concepts will be Bayesian, emphasizing the concepts that have a connection to physical sciences, such as classical and statistical mechanics. We will focus on data science and data analysis applications that are often encountered in real world of physical sciences. We will review many of machine learning concepts and methods.

**Target audience**:
The target student population is upper division undergraduates from physical science departments, as well as beginning graduate students from the same departments. The course is also suitable for graduate students looking for an introduction to programming and numerical methods in python.

**Course structure**:
Each week there will be a set of 3 hour lectures discussing the theoretical and practical underpinnings of the specific topic, together with its most common applications in the physical sciences. Class participation is expected via weekly reading of the lecture notes in advance, submitting comments and questions on the lecture, and answering a short set of questions. There will be eight python-based homework assignments, which will apply the methods to physical science based examples. A weekly one hour discussion will focus on the lecture material and homeworks. There will be 3 longer projects spread over the term.

**Prerequsites**:
Undergraduate students: basic introduction to Python programming at the level of PHY77 or permission from instructor.
Graduate students: none.

**Grades**: 40% projects, 40% homeworks, 20% quizzes.

Lecture 1: Introduction to probability and Bayesian inference: general rules of probability, generating functions, moments and cumulants, binomial and multinomial, Poisson, gaussian distributions, multi-variate distributions, joint probability, marginal probability, Bayes theorem, forward and inverse probability, from probability to inference and the meaning of probability, prior, likelihood and posterior, interval estimates, comparison between Bayesian and classical statistics, Bayesian versus classical hypothesis testing (p-value) 
  References: Ch. 2.1-2.3, 3 of MacKay, Ch. 2 of Kardar, Ch. 1-2 of Gelman et al, Bayesian data analysis
Lecture 2: More on Bayesian inference and intro to data modeling: informative and noninformative priors, maximum a posteriori (MAP) and maximum likelihood estimator (MLE), asymptotic theorems, least square as MAP/MLE, fitting data to a straight line and a general linear least square model, normal equations
  Reference: Ch. 15 of NR, Ch. 3, 4 of Gelman et al. 
Lecture 3: Linear Algebra: gaussian and Gauss-Jacobi elimination, backsubstitution, pivoting, LU decomposition, Cholesky decomposition, QR decomposition, sparse matrix linear algebra, solving linear equations with linear algebra, QR decomposition and tridiagonal forms, diagonalization of a symmetric and non-symmetric matrix, principal axes and covariance matrix, singular value decomposition (SVD), application to normal equations, principal component analysis (PCA) and dimensionality reduction, independent component analysis (ICA)
  Reference: Ch. 2,11 of NR & Ch. 6 of Newman, https://arxiv.org/pdf/1404.2986.pdf
Lecture 4: Information theory: Shannon information and mixing entropy, entropy for continuous variables and maximum entropy distributions, Kullback-Leibler divergence, negentropy, statistical independence, mutual and multi-information (application: FastICA), ensemble averaging: log likelihood as entropy, curvature matrix (Hessian) as Fisher information matrix. Experiment design. 
  Reference: Ch. 2 of MacKay, Ch. 2 of Kardar, https://arxiv.org/pdf/1404.2986.pdf
Lecture 5: Nonlinear equations and 1-d optimization: bisection, Newton-Raphson, secant, false position method. Golden ratio, parabolic optimization. Relaxation methods. Optimization in many dimensions: 1st order:gradient descent, stochastic gradient descent, mini-batch gradient descent. Momentum and Nesterov acceleration, ADAM. 2nd order methods: general strategies: choosing direction, doing line search or trust region. Newton, quasi-Newton, Gauss-Newton, conjugate gradient, Levenberg-Malmquardt method. 
  Reference: Newman Ch. 6, NR Ch. 9, Nocedal & Wright, Optimization. NR 9,10,15. 
Lecture 6: Monte Carlo methods for integration and posteriors: Simple Monte Carlo. Random number generators: transform method, Box-Muller for gaussian, Cholesky for multivariate gaussians, rejection sampling. Importance sampling for posteriors and for integration. Markov Chain Monte Carlo: Metropolis and Metropolis-Hastings. Convergence tests: burn-in, Gelman-Rubin statistic and chain correlation length. Improving efficiency: proposal function, Gibbs sampler with conditional conjugate distributions. Simulated annealing and simulated tampering. Hamiltonian Monte Carlo. Other MCMC approaches. 
  References: NR, Press etal., Ch.7, Newman, Ch. 10, Gelman et al. Ch 10-12, MacKay Ch. 20-22
Lecture 7: More advanced Bayesian analysis: probabilistic graphical models, hierarchical Bayesian models, model checking and evaluation, dealing with outliers
  References: Gelman et al. Ch. 5, 6, 7, 17
Lecture 8: Variational approximations: conditional and marginal approximations, expectation maximization and gaussian mixture model, variational inference and variational Bayes, expectation propagation
  References: Gelman Ch 13, 22
Lecture 9: Best practices of statistical analysis: Model checking, evaluating, Model comparison, bootstrap, jackknife, cross-validation tests, p-hacking, blind analysis, decision theory
  References: Gelman Ch 6-9, Mackay Ch 36
Lecture 10: Interpolation and extrapolation of data: polynomial, rational and spline interpolation, gaussian processes for regression and for classification
  References: NR Ch. 5, Gelman Ch. 21
Lecture 11: Fourier methods: Fast Fourier transforms (FFT), FFT convolutions, power spectrum and correlation function, Wiener filtering and missing data, matched filtering, wavelets
  References: NR Ch. 12, 13
Lecture 12: Classification: supervised and unsupervised learning, naive Bayes, Decision Tree-Based methods, random forest
  References: Bishop Ch 3, Gelman Ch 20-21
Lecture 13: Neural networks, deep networks, Convolutional nets: neural networks, deep networks, automated differentiation: back and forward propagation, inference: logistic function, ReLU
  References: http://cs231n.github.io/, https://arxiv.org/pdf/1803.08823.pdf, http://www.deeplearningbook.org/
Lecture 14: Unsupervised Learning: generative adversarial networks, autoencoders, normalizing flows

Literature
----------

- [Numerical Recipes](http://numerical.recipes), by Press. W. et al.

- [Information Theory, Inference and Learning Algorithms](http://www.inference.phy.cam.ac.uk/mackay/itila/book.html), by David MacKay

- Bayesian data analysis, 3rd edition, by Gelman A., et al.

- [An Introduction to Statistical Learning](http://www-bcf.usc.edu/~gareth/ISL/ISLR%20Sixth%20Printing.pdf), by James G. etal, 

- [A Survey of Computational Physics](http://www.compadre.org/psrc/items/detail.cfm?ID=11578) by Landau, R., Paez, M-J., Bordeianu, C.

- <http://greenteapress.com/wp/think-bayes/>

- <https://github.com/CamDavidsonPilon/Probabilistic-Programming-and-Bayesian-Methods-for-Hackers>

- [Computational Physics](http://www-personal.umich.edu/~mejn/cp/chapters/int.pdf) by Mark Newman

- Effective Computation in Physics, by A. Scopatz and K. D. Huff

- [From Python to Numpy](https://www.labri.fr/perso/nrougier/from-python-to-numpy/) by N. P. Rougier

[//]: # (THESE WERE COMMENTED OUT )

[//]: # (opinionated lectures in statistics by Press W., )

[//]: # (http://wpressutexas.net/coursewiki/index.php/OpinionatedLessons.org/ )

[//]: # (mathematicalmonk series of videos by Jeff Miller, https://www.youtube.com/user/mathematicalmonk/playlists?spfreload=10 )

[//]: # (Various other resources )

[//]: # (https://arxiv.org/pdf/1505.02965.pdf)

[//]: # (https://arxiv.org/abs/1701.02434)

Other resources will be provided according to the needs.


Software
--------

We will use Python Jupyter hub environment. You are expected to use existing numerical analysis routines and not write your own. Most of these are already implemented in python libraries (scipy, numpy...).

[//]: # (Routines that go with Landau's book are at)
[//]: # (http://www.science.oregonstate.edu/~landaur/Books/CPbook/Codes/PythonCodes/)

Homeworks and Projects
--------

Throughout the course, students will complete and electronically submit one homework assignment (code) per week. This code will be run on test cases to check if it produces appropriate results. Students are encouraged to discuss homeworks with other students, but should submit their own solutions. Homeworks will use the concepts developed in the lectures and apply to relatively simple problems. 
Projects are larger assignments intended to teach you how to combine ideas from the course in interesting ways and apply them to real data. There are three projects during the semester, and are in lieu of the midterm and final exam. Homeworks and projects are to be submitted using Jupyter notebook in Python.

