# Virtual mouse using hand and eye gesture and chatbot

## 1. Create a clean conda environment with Python 3.8.5
Create an environment named ai mouse (or any name) using Run project in Anaconda.
Create an environment named aimouse (or any name) using Python 3.8.5

### Bash:
### conda create -n aimouse python=3.8.5 pip -y conda activate aimouse python --version
### should print: Python 3.8.5
### Why conda: it manages binary Run project in Anaconda.

## 2. Install system prerequisites (Windows) - important Some packages (dlib, mediapipe, compiled C extensions) need build tools or system ### libraries. Install or verify:
### 1)Visual C++ Build Tools /Visual Studio Build Tools
Install from Microsoft: choose "Desktop development with C++" workload (CMake + MSVC).
### 2)After install, restart your PC or at least restart Anaconda Prompt.
CMake (if you expect to build from source)
You can install with conda: conda install -c conda-forge cmake -y
### 3)(Optional) For audio/sound drivers, make sure microphone and speaker are enabled in Windows Settings.

## 3. Prefer conda installs for heavy packages (fast & compatible)
Before running pip install -r requirements.txt, install the most fragile/binary packages via conda (using conda-forge) - this reduces build errors.
### Bash:
### core numeric + vision
### conda install -c
### conda-forge numpy=1.24.4 -у
### conda install -c
### conda-forge opencv=4.10.0 -y
### GUI
### conda install -c
### conda-forge pyqt=5.15.9 -y
### dlib (very sensitive)

