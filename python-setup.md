# Python Environment Setup
## Anaconda
### 1. Install Anaconda 
* Go to the Anaconda distribution [page](https://www.anaconda.com/products/distribution), scroll to the bottom and find the Anaconda installer file for your Operating System. 
* Run the installer .exe and follow all recommendations in the installer. This [installation docs page](https://docs.anaconda.com/anaconda/install/) provides step-by-step guidance depending on your OS and use-case.
* When Anaconda asks you "Do you wish the installer to initialize Anaconda3?" Say Yes
### 2. Test your Anaconda Installation
* Open your command-prompt/shell/terminal and type `conda list`. You should see something like this.

![kaza_readme_condalist](https://user-images.githubusercontent.com/51868526/184011797-51781e24-396c-42a8-8ee8-d516e92fbb64.JPG)

* notice we're in the `base` environment by default, as indicated by the command-line. We want to operate from a custom python environment.
### 3. Create a custom virtual environment
Keep your shell open and paste each one of these commands.
* Create a new conda env named 'gee'
```
conda create -n gee 
```
* Activate your new 'gee' env
```
conda activate gee
```
* In your shell, run this code block:
```
conda install -c conda-forge earthengine-api scikit-learn pandas
```
* Wait for package solver to finish and type y to proceed with installation.

## Visual Studio Code
### 1. Install VS code with the installer for your machine's operating system (Windows, MacOS, Linux)
* stuff
* stuff
### 2. Setup VS Code
* get helpful extensions
* generally get familiar
* 
