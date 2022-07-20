# DeepCADD

This repository contains the source files of our research on DeepCADD: a Deep Neural Network for Automatic Detection of Coronary Artery Disease (CAD). The study contains three main features: CAD segmentation using mainly the Frangi filter; CAD Classification using a ResNet-50; CAD detection using a Mask R-CNN-based architecture.

This repository contains the following algorithms:
* **Right Coronary Artery (RCA) Segmentation**, introduced in [2], which provides a technique for image segmentation of the right coronary artery (RCA) main segment. See experiment at `segmentation/CAD-segmentation.ipynb`
* **CNN for coronary segment classification**, introduced in [1], which evaluates the performance of ResNet-50 architecture on classifying CAD segments into `stenosed` and `non-stenosed`. See experiment at `colab/DeepCADD-backbone-ResNet50.ipynb`
* **Mask R-CNN for CAD detection**, introduced in [1], which introduces the use of [Mask-RCNN](https://github.com/matterport/Mask_RCNN) for CAD detection. See experiment at `colab/DeepCADD-running-with-ResNet50-backbone.ipynb` and `colab/DeepCADD-training-with-ResNet50.ipynb`


## Publications

1. FREITAS, Samuel A.; RAMOS, Gabriel de O.; COSTA, Cristiano André da. DEEPCADD: A Deep Neural Network for Automatic Detection of Coronary Artery Disease. In: CONCURSO DE TESES E DISSERTAÇÕES - SIMPÓSIO BRASILEIRO DE COMPUTAÇÃO APLICADA À SAÚDE (SBCAS), 22. , 2022, Teresina/PI. Anais [...]. Porto Alegre: Sociedade Brasileira de Computação, 2022 . p. 25-32. ISSN 2763-8987. [[link]](https://doi.org/10.5753/sbcas_estendido.2022.222389).

2. FREITAS, Samuel A.; NIENOW, Débora; COSTA, Cristiano A. da; RAMOS, Gabriel de O.. Functional Coronary Artery Assessment: a Systematic Literature Review. In: Wiener Klinische Wochenschrift, 2021. [[link]](https://link.springer.com/article/10.1007/s00508-021-01970-4)

3. FREITAS, Samuel A.; COSTA, Cristiano A. da; RAMOS, Gabriel de O.. Coronary Artery Disease Automatic Classification. In: ESCOLA REGIONAL DE COMPUTAÇÃO APLICADA À SAÚDE (ERCAS), 8. , 2021, São Paulo. Anais […]. Porto Alegre: Sociedade Brasileira de Computação, 2021 . p. 26-29. [[link]](https://sol.sbc.org.br/index.php/ercas/article/view/17431/17267)

4. FREITAS, Samuel; RAMOS, Gabriel; SCHMITH, Jean; COSTA, Cristiano. Nodal Analysis for Coronary Artery Ischemia Diagnosis. In: SIMPÓSIO BRASILEIRO DE COMPUTAÇÃO APLICADA À SAÚDE (SBCAS), 20. , 2020, Evento Online. Anais […]. Porto Alegre: Sociedade Brasileira de Computação, 2020 . p. 262-272. [[link]](https://sol.sbc.org.br/index.php/sbcas/article/view/11519/11382)

5. NIENOW, Débora; FREITAS, Samuel; SCHMITH, Jean. Software para auxílio no diagnóstico de estenoses em artérias coronárias. Arq. Bras. Cardiol: 113 (2 sup l. 1) p. 254. 2019. [[link]](http://publicacoes.cardiol.br/portal/abc/portugues/2019/v11303/pdf/sbc-2019-programa-trabalhos.pdf)

## Requirements

Before you begin, ensure you have met the following requirements:

* Python v3.6
* Tensorflow v1.x
* h5py v2.10.0
* Ipython v7.31.0
* OpenCV v4.1.2

## Usage

We decided to execute all the experiments using Google Colab PRO, powered by the existing available libraries and avoiding to overload the local machine.

For `CAD segmentation`, copy the notebook available at `segmentation/CAD-segmentation.ipynb`. 

For `DeepCADD backbone` classification, copy the notebook available at `colab/DeepCADD-backbone-ResNet50.ipynb`.

For `DeepCADD` detection, copy the notebook available at `colab/DeepCADD-training-with-ResNet50.ipynb`.

_tbc_

## Contributors

Thanks to the following people who have contributed to this project:

* [Samuel Armbrust](https://github.com/armbrustsamuel)
* [Felipe Andre Zeiser](https://github.com/felipezeiser)

## How to cite this research

For citing this work, please use the following entries. For entries of the other works, go to [https://armbrustsamuel.github.io/publications/](https://armbrustsamuel.github.io/publications/).

```bibtex
@inproceedings{freitas2022sbcas,
  title={DEEPCADD: A Deep Neural Network for Automatic Detection of Coronary Artery Disease},
  author={FREITAS, Samuel A.; RAMOS, Gabriel de O.; COSTA, Cristiano André da.},
  booktitle={Concurso de Teses e Dissetações - Anais do Simpósio Brasileiro de Computa{\c{c}}{\~a}o Aplicada {\`a} Sa{\'u}de},
  pages={25-32},
  year={2022},
  organization={SBC}
}
```

```bibtex
@article{freitas2021functional,
  title={Functional Coronary Artery Assessment: a Systematic Literature Review},
  author={Freitas, Samuel A and Nienow, D{\'e}bora and da Costa, Cristiano A and Ramos, Gabriel de O},
  journal={Wiener klinische Wochenschrift},
  pages={1--17},
  year={2021},
  publisher={Springer}
}
```

## License

This project uses the following license: [MIT](https://github.com/armbrustsamuel/DeepCADD/blob/main/LICENSE).
