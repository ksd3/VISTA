# VISTA
Python implementation of the VISTA (Video Imputation with SoftImpute, Temporal smoothing and Auxiliary data) algorithm of Sun et al.

If you use this code, please shoot me an email at kshitijd[at]bu.edu! I'd like to know if you run into any problems.

If you use VISTA for your own work, please cite the following two papers:

Sun, H., Hua, Z., Ren, J., Zou, S., Sun, Y., & Chen, Y. (2022). Matrix completion methods for the total electron content video reconstruction. Annals of Applied Statistics, 16(3), 1333–1358. https://doi-org.proxy.lib.umich.edu/10.1214/21-aoas1541

Sun, H., Chen, Y., Zou, S., Ren, J., Chang, Y., Wang, Z., & Coster, A. (2023). Complete global total electron content map dataset based on a video imputation algorithm vista. Scientific Data, 10(1), 236. https://doi-org.proxy.lib.umich.edu/10.1038/s41597-023-02138-7


To run VISTA, simply run the first 8 cells of the Jupyter Notebook, then call the function **VISTA()** with the appropriate initial conditions, values, and regularizers. Be warned that VISTA requires a large amount of memory and may not be suitable for tensors occupying a large amount of memory. 

The choice of initial condition, regularization, and auxiliary data is left to the user. Some tests on random data have shown that a low rank and l1, l2, l2 all set to values between 0.8 and 1.2 seem to reconstruct the missing data 'well', with low average errors. However this testing it **not** exhaustive.
