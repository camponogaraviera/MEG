# Magnetoencephalography (MEG) Data Processing
**Description:** This repository is intended for reading, processing, and analysis of [MEG](https://en.wikipedia.org/wiki/Magnetoencephalography) data with MNE-Python.

> The goal is to perform MEG data processing with the aid of Deep Neural Networks.

# Prerequisites
- **Programming Language:** `Python V3.8.3`
- **MNE-Python:** `MNE V0.21.0` 
- **Year:** `2020`

# Conda Environment
**Setting up a conda environment with [MNE-Python](https://mne.tools/stable/install/mne_python.html).**

1. Download [Anaconda](https://www.anaconda.com/products/individual).
1. Open Ubuntu terminal console window: `ctrl+alt+t`:
```console
Terminal

(base) user@user:~$ cd Downloads
#Grant execute permission
(base) user@user:~$ chmod +x Anaconda3-2020.07-Linux-x86_64.sh
#Run the above .sh file script and install Anaconda
(base) user@user:~$ ./Anaconda3-2020.07-Linux-x86_64.sh
```
3. Create a `Conda env`:
```console
Terminal

#Listing new conda envs
(base) user@user:~$ conda env list #To list the current environments.
#Creating a new conda env
(base) user@user:~$ conda create -n meg python=3.8.3 #To create an environment termed "meg" with python version 3.8.3.
(base) user@user:~$ conda activate meg #To activate meg environment.
#Upgrading pip
(meg) user@user:~$ pip install --upgrade pip #To upgrade the pip package-management.
#Installing MNE 
(meg) user@user:~$ pip install mne #To install mne.
#Listing Installed Packages
(meg) user@user:~$ conda list -n meg #To check all installed packages in the current environment.
(meg) user@user:~$ conda list -n meg mne #To check if mne was installed in the current environment.
#Testing
(meg) user@user:~$ python -c "import mne; mne.sys_info()" #To display system information along with MNE-Python version and its dependencies.
#For jupyter notebook Users
(meg) user@user:~$ conda install -c anaconda ipykernel #To install ipykernel.
(meg) user@user:~$ python -m ipykernel install --user --name=meg #To assign the env to jupyter notebook.
(meg) user@user:~$ jupyter kernelspec list #To list current jupyter kernels.
(meg) user@user:~$ conda deactivate #To exit the current env.
(base) user@user:~$ jupyter notebook #To open jupyter notebook. 
#Deleting a conda kernel
(meg) user@user:~$ jupyter kernelspec uninstall meg #To remove the "meg" kernel if necessary.
#Deleting a conda env
(base) user@user:~$ conda env remove -n meg #To delete the environment if necessary.
```

## Jupyter Notebook

```Python
import sys
import mne

print('Running Python Version ==', sys.version, '\n')
print('Running MNE Version ==', mne.__version__)
```

# Author 

Created and maintained by [@camponogaraviera][1].

[1]: https://github.com/camponogaraviera

# References

\[1] [Hansen, P. C., Kringelbach, M. L., & Salmelin, R. (Eds.). (2010). MEG: An introduction to methods. Oxford University Press.](https://doi.org/10.1093/acprof:oso/9780195307238.001.0001)

\[2] [Peter Hore. Nuclear Magnetic Resonance. May 2015. ISBN: 9780198703419.](https://global.oup.com/ukhe/product/nuclear-magnetic-resonance-9780198703419?cc=tw&lang=en&)

# License

This work is licensed under a [Creative Commons Zero Attribution v1.0 Universal](LICENSE) license.

