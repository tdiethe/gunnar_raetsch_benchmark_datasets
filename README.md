# Gunnar Raetsch's Benchmark Datasets

This is a re-packaging of the thirteen benchark datasets from Gunnar Raetsch's web-site in order to conserve disk-space and preserve for posterity, since the original website has been taken down. These benchmark datasets have been widely used in model selection studies in kernel learning methods (e.g. [1-3]). Each benchmark is stored in a structure containing the unique input and target patterns, and a set of indices giving the 100 training and test splits (20 in the case of the image and splice datasets). For example, to reconstitute the forty-second realisation of the banana benchmark,

      >> load bencharks.mat banana
      >> x_train = banana.x(banana.train(42,:),:);
      >> t_train = banana.t(banana.train(42,:));
      >> x_test  = banana.x(banana.test(42,:),:);
      >> t_test  = banana.t(banana.test(42,:));

## Downloads:

For Matlab V7 (about 8Mb) 
[benchmarks.mat](../master/benchmarks.mat)

For Matlab V6 (about 17Mb) 
[benchmarks_v6.mat](../master/benchmarks_v6.mat)


## References:

[1]	G. Raetsch, T. Onoda and K.-R. Muller, "Soft margins for AdaBoost", Machine Learning, vol. 43, no. 3, pp 287-320, March 2001.

[2]	S. Mika, G. Raetsch, J. Weston, B. Scholkopf and K.-R. Muller, "Fisher discriminant analysis with kernels", in Neural Networks for Signal Processing IX, pp 41-48, 1999.

[3]	Cawley, G. C. and Talbot, N. L. C., "Efficient leave-one-out cross-validation of kernel Fisher discriminant classifiers", Pattern Recognition, vol. 36, pp 2585-2592, 2003.

[4]   Diethe, T. "13 benchmark datasets derived from the UCI, DELVE and STATLOG repositories". https://github.com/tdiethe/gunnar_raetsch_benchmark_datasets/, 2015.

This was cloned from http://theoval.cmp.uea.ac.uk/~gcc/matlab/default.html#benchmarks  
