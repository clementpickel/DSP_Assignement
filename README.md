# DSP_Assignement

Data science programming assignements

# Setting up the Python environment

The Python exercises and assignments in this course will be based on Jupyter Notebooks. To facilitate setting up the environment, I am also providing you with a pre-defined Conda environment that installs all required packages for you. You should have learned to use both Conda and Jupyter in the Machine Learning course; please review the material there if necessary.

## Installing the Conda Environment

To install the Conda environment, download [environment.yml](environment.yml) and run the following commands:

```bash
conda env create -f environment.yml
conda activate dsp
python -m ipykernel install --user --name=python3-dsp
```

This will install a new Conda environment named **"dsp"**, as well as the corresponding Jupyter kernel named **"python3-dsp"**. All notebooks I provide you will be saved under the kernel **"python3-dsp"**.  

If you don't name your kernel the same way, you will get a warning message from Jupyter the first time you open each notebook and will have to select the kernel manually.

## Installing Packages Manually

If you prefer to install the packages some other way (e.g., through pip), the core packages you'll need for this course are:

```bash
matplotlib~=3.5
numpy~=1.22
pandas~=1.4
pingouin~=0.5
scikit-learn
scipy~=1.8
seaborn~=0.11
statsmodels~=0.13
streamlit~=1.7
```

The notebooks also use **rich~=12.0**, but this is entirely optional. You can comment out the following line in the notebook if you can't or don't want to install this package:

```python
%load_ext rich
```
