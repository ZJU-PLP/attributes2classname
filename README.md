
This repository contains a TensorFlow implementation of the [Attributes2Classname: A discriminative model for attribute-based unsupervised zero-shot learning](https://arxiv.org/pdf/1705.01734.pdf).
<p align="center">
<img src="images/output.png" align="center" width="500px" height="250px"/>
</p>

### License

attributes2classname is released under the MIT License (refer to the LICENSE file for details).

### Citing attributes2classname

If you find attributes2classname useful in your research, please consider citing:

    @article{demirel2017attributes2classname,
        title={Attributes2Classname: A discriminative model for attribute-based unsupervised zero-shot learning},
        author={Demirel, Berkan and Cinbis, Ramazan Gokberk and Cinbis, Nazli Ikizler},
        journal={arXiv preprint arXiv:1705.01734},
        year={2017}
    }
  
### How to train and evaluate a model:
1. Modify the training script (i.e. `master.py`) to point to your data directory.
2. Run the training script (i.e. `master.py`) to learn best parameters for your features. The applyCrossValidation variable must be marked True (`applyCrossValidation=True`) in order to learn the parameters.
3. After learning the relevant parameters, the training script is executed with these parameters to train and evaluate the PBT or IBT model. The applyCrossValidation variable must be marked False (`applyCrossValidation=False`) in order to learn and evaluate the correct model.

### Pretrained models:
Pretrained models and related parameters will be provided for AwA and aPaY datasets.
