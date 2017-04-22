# Two-mode-HOSVD
Two-mode Higher-Order Tensor Singular Value Decomposition 

The main function is HOSVD_extend.m. It implements the two-mode HOSVD algorithm described in https://arxiv.org/abs/1612.03839. 
The algorithm efficiently approximates the robust eigenvalue/vector pairs for a nearly orthogonal and symmetric tensor of order p. Compared to other decomposition algorithms based on power iteration or joint diagonalization, our algorithm estimates the components more accurately from a noisy input tensor. For graphical model applications, order-3 tensors are of main interest, for which we improve the perturbation tolerance from 1/d to 1/sqrt(d).

tenfact_extend.m is based on the orthogonal joint diagonalization. We optimized the original algorithm  (Kuleshov et al AISTATS 2015) and extended it to allow order-p tensors. 

tmp_extend.m is based on the tensor power iteration. We optimized the original algorithm (Anandkumar et al JMLR 2014) and extended it to allow order-p tensors. 

See the comments in each file for input/output format. 

