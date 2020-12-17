# Tabular Distributional Reinforcement Learning Implementations

This [notebook](TabularDistRL.ipynb) implements and trains several recent
distributional RL algorithms on a simple linear Markov Decision Process
inspired by the toy example in [4].

The following algorithms are implemented:

* Traditional (non-distributional) Q-learning [1]
* Categorical Distributional Q-learning [2]
* Quantile Distributional Q-learning [3]
* Expectile Distributional Q-learning [4, 5]
    * Naive imputation strategy (known to be incorrect, included here to
      demonstrate the nature of its flaws)
    * Optimisation-based imputation strategy (overcomes those flaws, but
      pretty slow)

The code is not intended for readability, sorry about that. You should refer
to the papers for full details of these algorithms.
And follow this implementation at your own risk: There may be subtle errors,
I have not checked the implementation carefully.

Note: For more information on the method used to calculate expectiles, see
[this other repo](https://github.com/matomatical/expectiles).

## References

[1] R. S. Sutton and A. G. Barto, *Reinforcement learning: An introduction.*
    MIT press, 2018.

[2] M. G. Bellemare, W. Dabney, and R. Munos,
    "A distributional perspective on reinforcement learning,"
    in *Proceedings of the 34th International Conference on Machine Learning*
    2017.

[3] W. Dabney, M. Rowland, M. G. Bellemare, and R. Munos,
    "Distributional reinforcement learning with quantile regression,"
    in *AAAI*, 2018.

[4] M. Rowland, R. Dadashi, S. Kumar, R. Munos, M. G. Bellemare, and
    W. Dabney,
    "Statistics and samples in distributional reinforcement learning,"
    in *International Conference on Machine Learning*, 2019.

[5] W. Dabney, Z. Kurth-Nelson, N. Uchida et al.
    "A distributional code for value in dopamine-based reinforcement
    learning,"
    *Nature 577*, 2020.
