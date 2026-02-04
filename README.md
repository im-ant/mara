# KL-Regularized Reinforcement Learning is Designed to Mode Collapse

**ICLR 2026**

[Anthony GX-Chen](https://im-ant.github.io/), [Jatin Prakash](https://bicycleman15.github.io/), [Jeff Guo](https://guojeff.github.io/), [Rob Fergus](https://cs.nyu.edu/~fergus/), [Rajesh Ranganath](https://cims.nyu.edu/~rajeshr/)

[[arXiv]](https://arxiv.org/abs/2510.20817) [[OpenReview]](https://openreview.net/forum?id=flBRtdIihA)

## Abstract

Classical intuitions cast minimizing reverse KL as "mode seeking" and forward KL as "mass covering". In KL-regularized reinforcement learning, however, the regularizer determines *both* the target distribution's shape *and* the divergence being implicitly minimized, making its role more nuanced than simply inducing generic mode-seeking or mass-covering behaviour. Specifically, the target distribution is defined jointly by the reward function, the reference model, the type of regularizer, and the regularization strength. We show that under common settings—such as low regularization strength and equal verifiable rewards—both forward and reverse KL regularization tend to specify target distributions whose mass concentrates on a single high-reward region. Thus, the objective itself *by construction* induces diversity collapse, regardless of the policy optimization algorithm used.

Building on this perspective, we introduce a simple and scalable modification that rescales rewards to induce target distributions assigning substantial probability across *all* high-reward regions. This yields a principled objective that maintains high solution quality while achieving broad reward-mode coverage. Empirically, this approach improves post-training diversity and performance for Large Language Models and Chemical Language Models, and is effective with either forward or reverse KL regularization, while using either naively fails.

## BibTeX

```bibtex
@inproceedings{
    gxchen2026mara,
    title={KL-Regularized Reinforcement Learning is Designed to Mode Collapse},
    author={Anthony GX-Chen and Jatin Prakash and Jeff Guo and Rob Fergus and Rajesh Ranganath},
    booktitle={The Fourteenth International Conference on Learning Representations},
    year={2026},
    url={https://arxiv.org/abs/2510.20817}
}
```

## Acknowledgments

This project page was built using the [Academic Project Page Template](https://github.com/eliahuhorwitz/Academic-project-page-template), adopted from the [Nerfies](https://nerfies.github.io/) project page.

## License

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.
