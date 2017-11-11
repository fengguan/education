Hinton, Geoffrey E., Simon Osindero, and Yee-Whye Teh. "A fast learning algorithm for deep belief nets." Neural computation 18.7 (2006): 1527-1554. [pdf](http://www.cs.toronto.edu/~hinton/absps/ncfast.pdf) (Deep Learning Eve)

* EM algorithm and latent variable
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
        * A key point of departure from the RBM is that the posterior distribution over the hidden units (given the visibles) is no longer tractable, due to the interactions between the hidden units.
        * Question: how is this related to the fact that Ising model is difficult to solve.
          * Ising model is difficult because that particals are interact with each other, that is why mean field method can simplify this model. For Deep Boltzmann machine, the difficulty comes from the fact that hidden units are not directly determined by visible units, and they can affect visible units. (Can we consider visibal units as boundary conditions in Ising model?)
      * [Bengio, Joint Training of Deep Boltzmann Machines for Classification (2013)](https://arxiv.org/pdf/1301.3568.pdf)
      * [Hinton, Deep Boltzmann Machines](http://proceedings.mlr.press/v5/salakhutdinov09a/salakhutdinov09a.pdf)
      * [Hinton, An Efficient Learning Procedure for Deep Boltzmann Machines(2012)](http://www.utstat.toronto.edu/~rsalakhu/papers/neco_DBM.pdf)
      * [GoodFellow, Bengio, Multi-Prediction Deep Boltzmann Machines(PPT)](http://swoh.web.engr.illinois.edu/courses/IE598/handout/fall2016_slide3.pdf)
      * [GoodFellow, Bengio, Multi-Prediction Deep Boltzmann Machines(Paper)](https://papers.nips.cc/paper/5024-multi-prediction-deep-boltzmann-machines.pdf)
      
  * relation between: 
    * believe network
    * Boltzmann machine, 
    * deep believe network, 
    * restricted boltzmann machine, 
    * deep boltzmann machine, 
  * wake sleep algorithm & explain away
  * stack of RBM
  
* applications: auto-encoder  

* 文章解读：
  * [DBN 的理解](http://blog.sciencenet.cn/blog-110554-889016.html)
  * [Explaining away理解](http://blog.sciencenet.cn/blog-110554-889475.html)
  * [Complementary Prior](https://www.douban.com/note/344374111/)
  * [翻译](https://wenku.baidu.com/view/4fbe320db14e852459fb5740.html?re=view)
  * [paper presentation PPT](http://www.cs.purdue.edu/homes/alanqi/Courses/ML-08/Deep_Belief_nets.pptx)
