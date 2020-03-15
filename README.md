# [TorchIO](http://torchio.rtfd.io/)

[![PyPI downloads](https://img.shields.io/pypi/dm/torchio.svg?label=PyPI%20downloads&logo=python&logoColor=white)](https://pypi.org/project/torchio/)
[![PyPI version](https://badge.fury.io/py/torchio.svg)](https://badge.fury.io/py/torchio)
[![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/112NTL8uJXzcMw4PQbUvMQN-WHlVwQS3i)
[![Build status](https://img.shields.io/travis/fepegar/torchio/master.svg?label=Travis%20CI%20build&logo=travis)](https://travis-ci.org/fepegar/torchio)
[![Coverage status](https://codecov.io/gh/fepegar/torchio/branch/master/graphs/badge.svg)](https://codecov.io/github/fepegar/torchio)
[![Code quality](https://img.shields.io/scrutinizer/g/fepegar/torchio.svg?label=Code%20quality&logo=scrutinizer)](https://scrutinizer-ci.com/g/fepegar/torchio/?branch=master)
[![Code maintainability](https://api.codeclimate.com/v1/badges/518673e49a472dd5714d/maintainability)](https://codeclimate.com/github/fepegar/torchio/maintainability)
[![Slack](https://img.shields.io/badge/TorchIO-Join%20on%20Slack-blueviolet?style=flat&logo=slack)](https://join.slack.com/t/torchioworkspace/shared_invite/enQtOTY1NTgwNDI4NzA1LTEzMjIwZTczMGRmM2ZlMzBkZDg3YmQwY2E4OTIyYjFhZDVkZmIwOWZkNTQzYTFmYzdiNGEwZWQ4YjgwMTczZmE)

---

### 🎉 News: the paper is out! 🎉

See the [Credits](#credits) section below for more information.

---

<table align="center">
    <tr>
        <td align="center">Original</td>
        <td align="center">Random blur</td>
    </tr>
    <tr>
        <td align="center"><img src="docs/images/gifs_readme/1_Lambda_mri.png" alt="Original"></td>
        <td align="center"><img src="docs/images/gifs_readme/2_RandomBlur_mri.gif" alt="Random blur"></td>
    </tr>
    <tr>
        <td align="center">Random flip</td>
        <td align="center">Random noise</td>
    </tr>
    <tr>
        <td align="center"><img src="docs/images/gifs_readme/3_RandomFlip_mri.gif" alt="Random flip"></td>
        <td align="center"><img src="docs/images/gifs_readme/4_Compose_mri.gif" alt="Random noise"></td>
    </tr>
    <tr>
        <td align="center">Random affine transformation</td>
        <td align="center">Random elastic transformation</td>
    </tr>
    <tr>
        <td align="center"><img src="docs/images/gifs_readme/5_RandomAffine_mri.gif" alt="Random affine transformation"></td>
        <td align="center"><img src="docs/images/gifs_readme/6_RandomElasticDeformation_mri.gif" alt="Random elastic transformation"></td>
    </tr>
    <tr>
        <td align="center">Random bias field artifact</td>
        <td align="center">Random motion artifact</td>
    </tr>
    <tr>
        <td align="center"><img src="docs/images/gifs_readme/7_RandomBiasField_mri.gif" alt="Random bias field artifact"></td>
        <td align="center"><img src="docs/images/gifs_readme/8_RandomMotion_mri.gif" alt="Random motion artifact"></td>
    </tr>
    <tr>
        <td align="center">Random spike artifact</td>
        <td align="center">Random ghosting artifact</td>
    </tr>
    <tr>
        <td align="center"><img src="docs/images/gifs_readme/9_RandomSpike_mri.gif" alt="Random spike artifact"></td>
        <td align="center"><img src="docs/images/gifs_readme/10_RandomGhosting_mri.gif" alt="Random ghosting artifact"></td>
    </tr>
</table>



TorchIO is a Python package containing a set of tools to efficiently
read, sample and write 3D medical images in deep learning applications
written in [PyTorch](https://pytorch.org/),
including intensity and spatial transforms
for data augmentation and preprocessing. Transforms include typical computer vision operations
such as random affine transformations and also domain-specific ones such as
simulation of intensity artifacts due to
[MRI magnetic field inhomogeneity](http://mriquestions.com/why-homogeneity.html)
or [k-space motion artifacts](http://proceedings.mlr.press/v102/shaw19a.html).

This package has been greatly inspired by [NiftyNet](https://niftynet.io/).


## Credits

If you like this repository, please click on Star!

If you use this package for your research, please cite the paper:

[Pérez-García et al., 2020, *TorchIO: a Python library for efficient loading, preprocessing, augmentation and patch-based sampling of medical images in deep learning*](https://arxiv.org/abs/2003.04696).


BibTeX entry:

```bibtex
@misc{fern2020torchio,
    title={TorchIO: a Python library for efficient loading, preprocessing, augmentation and patch-based sampling of medical images in deep learning},
    author={Fernando Pérez-García and Rachel Sparks and Sebastien Ourselin},
    year={2020},
    eprint={2003.04696},
    archivePrefix={arXiv},
    primaryClass={eess.IV}
}
```


## [Documentation](https://torchio.readthedocs.io/)

The documentation is hosted on
[Read the Docs](https://torchio.readthedocs.io/).
It is a work in progress, but some classes such as
[`ImagesDataset`](https://torchio.readthedocs.io/data/image.html)
are already fairly well documented.
