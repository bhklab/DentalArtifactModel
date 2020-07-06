# dental-artifact-model
This repository hosts the contributor source files for the dental-artifact-model model. ModelHub integrates these files into an engine and controlled runtime environment. A unified API allows for out-of-the-box reproducible implementations of published models. For more information, please visit [www.modelhub.ai](http://modelhub.ai/) or contact us [info@modelhub.ai](mailto:info@modelhub.ai).
## meta
| | |
|-|-|
| id | f8063322-cbba-4dd4-85cc-3a939b1bb608 | 
| application_area | Head and Neck Computed Tomography Images | 
| task | Classification | 
| task_extended | Classification of dental artifact presence in H&N CT | 
| data_type | Image in form compatible with SimpleITK loading - .nrrd prefered | 
| data_source |  | 
## publication
| | |
|-|-|
| title | External validation and transfer learning of convolutional neural networks for computed tomography dental artifact classification | 
| source | Physics in Medicine & Biology | 
| url | https://iopscience.iop.org/article/10.1088/1361-6560/ab63ba | 
| year | 2020 | 
| authors | Mattea L Welch, Chris McIntosh, Alberto Traverso, Leonard Wee, Tom G Purdie, Andre Dekker, Benjamin Haibe-Kains and David A Jaffray | 
| abstract | Quality assurance of data prior to use in automated pipelines and image analysis would assist in safeguarding against biases and incorrect interpretation of results. Automation of quality assurance steps would further improve robustness and efficiency of these methods, motivating widespread adoption of techniques. Previous work by our group demonstrated the ability of convolutional neural networks (CNN) to efficiently classify head and neck (H&N) computed-tomography (CT) images for the presence of dental artifacts (DA) that obscure visualization of structures and the accuracy of Hounsfield units. In this work we demonstrate the generalizability of our previous methodology by validating CNNs on six external datasets, and the potential benefits of transfer learning with fine-tuning on CNN performance. 2112 H&N CT images from seven institutions were scored as DA positive or negative. 1538 images from a single institution were used to train three CNNs with resampling grid sizes of 64^3, 128^3 and 256^3. The remaining six external datasets were used in five-fold cross-validation with a data split of 20% training-fine-tuning and 80% validation. The three pre-trained models were each validated using the five-folds of the six external datasets. The pre-trained models also underwent transfer learning with fine-tuning using the 20% training-fine-tuning data, and validated using the corresponding validation datasets. The highest micro-averaged AUC for our pre-trained models across all external datasets occurred with a resampling grid of 256^3 (AUC = 0.91). Transfer learning with fine-tuning improved generalizability when utilizing a resampling grid of 256^3 to a micro-averaged AUC of 0.92. Despite these promising results, transfer learning did not improve AUC when utilizing small resampling grids or small datasets. Our work demonstrates the potential of our previously developed automated quality assurance methods to generalize to external datasets. Additionally, we showed that transfer learning with fine-tuning using small portions of external datasets can be used to fine-tune models for improved performance when large variations in images are present. | 
| google_scholar | N/A | 
| bibtex | @article{welch2020external, title={External validation and transfer learning of convolutional neural networks for computed tomography dental artifact classification}, author={Welch, Mattea L and McIntosh, Chris and Traverso, Alberto and Wee, Leonard and Purdie, Tom G and Dekker, Andre and Haibe-Kains, Benjamin and Jaffray, David A},  journal={Physics in Medicine & Biology},  volume={65},  number={3},  pages={035017},  year={2020},  publisher={IOP Publishing}, doi={https://doi.org/10.1088/1361-6560/ab63ba}} | 
## model
| | |
|-|-|
| description | A PyTorch three-dimensional convolutional neural network with a depth of five | 
| provenance | Contributed by author | 
| architecture | A three-dimensional (3D) convolutional neural network (CNN). | 
| learning_type | Supervised Learning | 
| format | .pth.tar | 
| I/O | model I/O can be viewed [here](contrib_src/model/config.json) | 
| license | model license can be viewed [here](contrib_src/license/model) | 
## run
To run this model and view others in the collection, view the instructions on [ModelHub](http://app.modelhub.ai/).
## contribute
To contribute models, visit the [ModelHub docs](https://modelhub.readthedocs.io/en/latest/).
