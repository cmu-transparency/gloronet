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

This site introduces GloRo Nets (for "globally robust networks"), a family of Deep Neural Networks that is verifiably robust against $\ell_p$-norm-bounded perturbations. Our Lipschitz-based robustness verification is *instant* and *deterministic* (so there is no false positive case) and scales favorably well to ImageNet-scale models. GloRo Nets have inspired a set of follow-up works in deep learning safety, explainability, overfitting and privacy. Read each individual post [HERE] for more information about GloRo-based works.

## Contributions of GloRo Nets to Robustness Research
### State-of-the-art Provable Robustness 
#### (last update: 2023-02)

GloRo Nets provide the *state-of-the-art* determinristic robustness guarantee on image classification. We provide a quick overview of the best VRA (verified-robust accuracy) results here (these are more up-to-date and may surpass the results reported in the original paper).  

dataset       |norm| radius | architecture     | VRA
--------------|----|--------|------------------|----------
MNIST         |$\ell_2$| 0.3    | Conv 2C2F        | **0.957**
MNIST         |$\ell_2$| 1.58   | Conv 4C3F        | **0.628**
CIFAR-10      |$\ell_2$| 0.141  | Conv 6C2F        | 0.600
CIFAR-10      |$\ell_2$| 0.141  | LiResNet 18L256W | **0.651**
CIFAR-100     |$\ell_2$| 0.141  | LiResNet 18L256W | **0.363**
Tiny-Imagenet |$\ell_2$| 0.141  | Conv 8C2F        | 0.224
Tiny-Imagenet |$\ell_2$| 0.141  | LiResNet 18L256W | **0.292**
ImageNet      |$\ell_2$| 1.0    | LiResNet 18L588W | **0.142**

TODO: paper urls.

### Towards Provable Top-K Robustness 

TODO

### Exploring Overfitting with GloRo Nets and TruLens

TODO


### Exploring Privacy Leakage in Robust Models with GloRo Nets

TODO


### A Pitfall of Robustness Certification: A Denial-of-service Attack.

TODO

## Making A Pull Request for GloRo-based Projects and Publications

Please feel free to make a pull request at the github page of this website (https://github.com/cmu-transparency/gloronet) to include your own GloRo-based work. A pull request should add another MARKDOWN file to `_posts/` following the template `_templates/project_post.md`.

## Bitex Citation
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

