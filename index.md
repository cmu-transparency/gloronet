---
#
# By default, content added below the "---" mark will appear in the home page
# between the top bar and the list of recent posts.
# To change the home page layout, edit the _layouts/home.html file.
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
#
layout: home
---


![Logo](media/logo_img.png#center)

This site introduces GloRo Nets (for "globally robust networks"), a family of Deep Neural Networks that is verifiably robust against L2-norm-bounded perturbations. Our Lipschitz-based robustness verification is *instant* and *deterministic* (so there is no false positive case) and scales favorably well to ImageNet-scale models. GloRo Nets have inspired a set of follow-up works in deep learning safety, explainability, overfitting and privacy. Read each individual post [HERE] for more information about GloRo-based works.

## Contributions of GloRo Nets to Robustness Research
### State-of-the-art Provable Robustness 
#### (last update: 2023-06)

GloRo Nets provide the *state-of-the-art* deterministic robustness guarantee. We provide a quick overview of the best VRA (verified-robust accuracy) results here. These are more up-to-date and may surpass the results reported in the original paper.  

dataset       |norm| radius | architecture     | VRA (%)
--------------|----|--------|------------------|----------
MNIST         |l2| 1.58   | Conv 4C3F        | 62.8
CIFAR-10      |L2| 0.141  | LiResNet 18L256W | 70.1
CIFAR-100     |L2| 0.141  | LiResNet 18L256W | 41.5
Tiny-Imagenet |L2| 0.141  | LiResNet 18L256W | 33.6
ImageNet      |L2| 0.141    | LiResNet 18L588W | 35.0

:book: Read our [ICML](http://proceedings.mlr.press/v139/leino21a/leino21a.pdf) paper for GloRo Nets and the recent [follow-up](https://arxiv.org/pdf/2301.12549.pdf) paper of LiResNet architecture.

:computer: Check out our implementations for popular deep learning frameworks (click the icon below).

[<img src="https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white">](https://github.com/klasleino/gloro) [<img src="https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white">](https://github.com/klasleino/gloro/tree/master/snapshots)



---

### Towards Provable Top-K Robustness 

TODO

---

### Exploring Overfitting with GloRo Nets and TruLens

TODO

---

### Exploring Privacy Leakage in Robust Models with GloRo Nets

TODO

---

### A Pitfall of Robustness Certification: A Denial-of-service Attack.

TODO



## Making A Pull Request for GloRo-based Projects and Publications

Please feel free to make a pull request at the github page of this website (https://github.com/cmu-transparency/gloronet) to include your own GloRo-based work. A pull request should add another MARKDOWN file to `_posts/` following the template `_templates/project_post.md`.


## Bibtex Citation
If you use the code of GloRo Net in your own project, please consider to using the following citations. If you are using a particular follow-up work described in [HERE], please additionally include the citation at the end of the project post.

```
@INPROCEEDINGS{leino21gloro,
    title = {Globally-Robust Neural Networks},
    author = {Klas Leino and Zifan Wang and Matt Fredrikson},
    booktitle = {International Conference on Machine Learning (ICML)},
    year = {2021}
}

@misc{kaiscaling2023,
  author = {Hu, Kai and Zou, Andy and Wang, Zifan and Leino, Klas and Fredrikson, Matt},
  title = {Scaling in Depth: Unlocking Robustness Certification on ImageNet},
  publisher = {arXiv},
  year = {2023}
}
```

### Main Contributors

[Klas Leino](https://www.cs.cmu.edu/~kleino/), [Zifan Wang](https://sites.google.com/west.cmu.edu/zifan-wang/home), [Matt Fredrikson](https://www.cs.cmu.edu/~mfredrik/), Kai Hu, [Andy Zou](https://andyzoujm.github.io)

