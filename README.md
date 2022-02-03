# SSD MobileNet Based Blender Gestural Input Interface

SSD MobileNet Based Blender Gestural Input Interface is a Python based project that aims at creating a Human Computer Interface for navigation and object manipulation in Blender through the use of hand gestures.  
This repository contains all the relevant data and steps required to produce a custom dataset for training, training and hooking to a Blender instance.  


https://user-images.githubusercontent.com/73691795/148990685-6ff03416-1f1b-4dd0-9d76-a4d393b1094c.mp4


## Installation

The version of Python used is Python 3.9.9, which can be installed following this guide:
[Python install](https://www.python.org/downloads/)

All the dependencies and submodules of this project can be installed through the [requirements.txt](https://github.com/MarzioVallero/ML-Based-Blender-Gestural-Input-Interface/blob/master/requirements.txt) file, by cloning this project as follows:
```bash
git clone -recursive https://github.com/MarzioVallero/ML-Based-Blender-Gestural-Input-Interface.git
pip install -r requirements.txt
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

For installing Tensorflow 2, required to train and run the neural network, I suggest to check out the official guide:  
[Tensorflow installation](https://www.tensorflow.org/install)  

For installing LabelImg and learning how to use it, I suggest the GitHub repository of the project:  
[LabelImg GitHub](https://github.com/tzutalin/labelImg)  

For computing performance metrics with Open-Source Visual Interface for Object Detection Metrics and learning how to use the tool, I suggets the repository of the project:
[Review Object Detection Metrics GitHub](https://github.com/rafaelpadilla/review_object_detection_metrics)

The compiler used to process the LaTeX documentation is MiKTeX, which can be installed at the following link (although any LaTeX compiler can be used):  
[MiKTeX installation](https://miktex.org/download)

## Usage

When not specifically stated, all shell commands should be run from the root directory of the project.
The trained model can be tested through the [ModelTest.ipynb](https://github.com/MarzioVallero/ML-Based-Blender-Gestural-Input-Interface/blob/master/ModelTest.ipynb) script.

The model is able to recognize gestures exclusive to the left or the right hand, at the same time. Swapping the gestures of the hands generally should not produce detections, apart from some known cases of aliasing.  
Follows a list of classes and their supposed linked action.  

![Gestures Map]("Technical Paper\resources\image\GestureMap.png")  

Left Hand Classes:   
L shape -> Object Root Select  
Fist shape -> Grab/Move  
O shape -> Rotate  
V shape -> View/Transform Select (Global/Local and Wireframe/Solid/Rendered)  
Open Hand -> Unhide all objects / Hide current object  

Right Hand Classes:  
Index pointing up -> Z positive axis  
Index pointing down -> Z negative axis  
Index pointing left -> X negative axis, previous  
Index pointing right -> X positive axis, next  
Index pointing forward -> Y positive axis  
Thumb pointing backwards -> Y negative axis  
C shape (all fingers with the index) -> Clear current transformation  


## Contributing
Contribution to the project is welcome, although the project won't be maintained in the future.  

## Authors and Acknowledgement

The project has been developed by Marzio Vallero as part of the [Computer Engineering Masters Degree](https://didattica.polito.it/pls/portal30/sviluppo.offerta_formativa.corsi?p_sdu_cds=37:18&p_lang=EN) exam [Machine Learning for Vision and Multimedia](https://didattica.polito.it/pls/portal30/gap.pkg_guide.viewGap?p_cod_ins=01URPOV&p_a_acc=2021&p_header=S&p_lang=EN&multi=N), taught by professors F. Lamberti, B. Bottino, E. Masala, L. Morra and A. Servetti, during the first semester of the academic year 2021/2022 at the [Politecnico di Torino University](https://www.polito.it/).

## License
For right to use, copyright and warranty of this software, refer to this project's [License](License.md).
