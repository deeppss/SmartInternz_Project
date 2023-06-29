# **Time Series Analysis For Bitcoin Price Prediction using Prophet**

Prophet is on PyPI, so you can use ```pip``` to install it.
```python
python -m pip install prophet
```
* From v0.6 onwards, Python 2 is no longer supported.
* As of v1.0, the package name on PyPI is "prophet"; prior to v1.0 it was "fbprophet".
* As of v1.1, the minimum supported Python version is 3.7.

After installation, you can get started!

Anaconda
Prophet can also be installed through conda-forge.

```
conda install -c conda-forge prophet
```

### Installation in Python - Development version

To get the latest code changes as they are merged, you can clone this repo and build from source manually. This is not guaranteed to be stable.

```
git clone https://github.com/facebook/prophet.git
cd prophet/python
python -m pip install -e .
```

By default, Prophet will use a fixed version of ```cmdstan``` (downloading and installing it if necessary) to compile the model executables. If this is undesired and you would like to use your own existing ```cmdstan``` installation, you can set the environment variable ```PROPHET_REPACKAGE_CMDSTAN``` to ```False```:

```
export PROPHET_REPACKAGE_CMDSTAN=False; python -m pip install -e .
```

Windows
Using ```cmdstanpy``` with Windows requires a Unix-compatible C compiler such as mingw-gcc. If cmdstanpy is installed first, one can be installed via the ```cmdstanpy.install_cxx_toolchain``` command.
