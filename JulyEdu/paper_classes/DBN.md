Hinton, Geoffrey E., Simon Osindero, and Yee-Whye Teh. "A fast learning algorithm for deep belief nets." Neural computation 18.7 (2006): 1527-1554. [pdf](http://www.cs.toronto.edu/~hinton/absps/ncfast.pdf) (Deep Learning Eve)

* Boltzmann machine & Ising model
  * phase transition
  * solve an Ising model:
    * Solving an Ising model is to compute the free energy function from parameters.
    * All statistical mechanism values can be obtained as derivatives of Free energy.
* representation arbitrary distributions (Boltzmann machine & Ising model)
  * [Le Boux and Bengio](http://www.iro.umontreal.ca/~lisa/publications2/index.php/attachments/single/22)
* Training of this model (layer by layer)
  * difficulty in training Boltzmann machine directly.
    * intractible partition function:
      * no analytic solution for 3D Ising model
      * mean field method
    * intractible inference:
      * MCMC method
      * [Bengio, On Training Deep Boltzmann Machines (2012)](https://arxiv.org/pdf/1203.4416.pdf)
      * [Bengio, Joint Training of Deep Boltzmann Machines for Classification (2013)](https://arxiv.org/pdf/1301.3568.pdf)
      * [Hinton, An Efficient Learning Procedure for Deep Boltzmann Machines(2012)](http://www.utstat.toronto.edu/~rsalakhu/papers/neco_DBM.pdf)

  * relation between: 
    * Boltzmann machine, 
    * deep believe network, 
    * restricted boltzmann machine, 
    * deep boltzmann machine, 
    * deep nueron network.
* applications: auto-encoder  
