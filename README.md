# SSD MobileNet Based Blender Gestural Input Interface

SSD MobileNet Based Blender Gestural Input Interface is a Python based project that aims at creating a Human Computer Interface for navigation and object manipulation in Blender through the use of hand gestures.  
This repository contains all the relevant data and steps required to produce a custom dataset for training, training and hooking to a Blender instance.  

// TODO: add video

## Installation

The version of Python used is Python 3.9.9, which can be installed following this guide:
[Python install](https://www.python.org/downloads/)

The version of OpenCV used for this project is version 4.5.3, which can be installed using the shell command:  
```bash
pip install opencv-python==4.5.3
```

For installing Jupyter Notebook, use the shell command:  
```bash
pip install notebook
```
Be sure to activate the local server necessary to run jupyter notebooks, using the shell command:  
```bash
jupyter notebook
```
Then, from the URL [Jupyter Notebook Tree](http://127.0.0.1:8888/tree) you'll be able to select notebooks to run. 
Else, define a Python interpreter and run the notebooks through an IDE like Visual Studio Code.
To install visual studio code, run the shell command:
```bash
code .
```

For installing Tensorflow, required to train the neural network, I suggest to check out the official guide:  
[Tensorflow installation](https://www.tensorflow.org/install)  

For installing LabelImg and learning how to use it, I suggest the GitHub repository of the project:  
[LabelImg GitHub](https://github.com/tzutalin/labelImg)  

The compiler used to process the LaTeX documentation is MiKTeX, which can be installed at the following link (although any LaTeX compiler can be used):  
[MiKTeX installation](https://miktex.org/download)

## Usage

When not specifically stated, all shell commands should be run from the root directory of the project.

// TODO: add usage information

## Contributing
Contribution to the project is welcome, although the project won't be maintained in the future by the development team.

## Authors and Acknowledgement

The project has been developed by Marzio Vallero as part of the [Computer Engineering Masters Degree](https://didattica.polito.it/pls/portal30/sviluppo.offerta_formativa.corsi?p_sdu_cds=37:18&p_lang=EN) exam [Machine Learning for Vision and Multimedia](https://didattica.polito.it/pls/portal30/gap.pkg_guide.viewGap?p_cod_ins=01URPOV&p_a_acc=2021&p_header=S&p_lang=EN&multi=N), taught by professors F. Lamberti, B. Bottino, E. Masala, L. Morra and A. Servetti, during the first semester of the academic year 2021/2022 at the [Politecnico di Torino University](https://www.polito.it/).

## License
For right to use, copyright and warranty of this software, refer to this project's [License](License.md).
