# Interactive Computer Graphics_HW-3-models-with-3-different-shadings-
## Prerequisites

## Introduction
This is a CG homework implemented in WebGL (Javascript with WebGL library/GLSL) which will display 3 models together with 3 different kinds of shadings:
1) Flat Shading
2) Gouraud Shading
3) Phong Shading 

## WHERE & HOW TO EDIT
For each kind of shading, we need to implement fragment and vertex shaders.\
Under line 327 (function initShaders), edit the 2 lines below with fragment shader and vertex shader\
To switch between 3 kinds of shading:\
FlatFragmentShader/FlatVertexShader\
GouraudFragmentShader/GouraudVertexShader\
PhongFragmentShader/PhongVertexShader\
\
Under loadTeapot()/loadKangaroo()/loadEaster() functions, we load our json model with these functions.\
To change the model you want to display, simply change the model into the path to your desired model under open request.

If you need to display more different models, you have to create their own respective buffers and set up their own projection matrices.\
\
Translate, rotate and scale functions are alike, you can adjust the variables inside in terms of x, y, z axes.\
\
For shearing, the shearing matrix is already created for you. You can adjust the angle inside the shear matrix within a range of (0, 90) exclusive.\
The shear matrix will then be multiplied by model view projection matrix as the final result to be displayed or viewed.\
\
Under functionwebGLStart(), u can simply add or erase additional loading model functions if necessary.
