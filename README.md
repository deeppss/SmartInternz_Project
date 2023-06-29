# **Time Series Analysis For Bitcoin Price Prediction using Prophet**

Assignment link: https://drive.google.com/drive/folders/1GIqEj4eqfH2MJNmHEPrg_VMD6Qo5PeGx?usp=sharing

Video demo link: https://drive.google.com/file/d/16M7wr6_YEKhiwVEH7zBz7Vwns8PhUhz6/view?usp=sharing

Prophet is on PyPI, so you can use ```pip``` to install it.
```python
python -m pip install prophet
```
* From v0.6 onwards, Python 2 is no longer supported.
* As of v1.0, the package name on PyPI is "prophet"; prior to v1.0 it was "fbprophet".
* As of v1.1, the minimum supported Python version is 3.7.

After installation, you can get started!

## Anaconda
Prophet can also be installed through conda-forge.

```python
conda install -c conda-forge prophet
```

### Installation in Python - Development version

To get the latest code changes as they are merged, you can clone this repo and build from source manually. This is not guaranteed to be stable.

```python
git clone https://github.com/facebook/prophet.git
cd prophet/python
python -m pip install -e .
```

By default, Prophet will use a fixed version of ```cmdstan``` (downloading and installing it if necessary) to compile the model executables. If this is undesired and you would like to use your own existing ```cmdstan``` installation, you can set the environment variable ```PROPHET_REPACKAGE_CMDSTAN``` to ```False```:

```python
export PROPHET_REPACKAGE_CMDSTAN=False; python -m pip install -e .
```

## Windows
Using ```cmdstanpy``` with Windows requires a Unix-compatible C compiler such as mingw-gcc. If cmdstanpy is installed first, one can be installed via the ```cmdstanpy.install_cxx_toolchain``` command.

## Download market data from yfinance

### Installation
Install yfinance using pip:

```python
$ pip install yfinance --upgrade --no-cache-dir
```

### Requirements

* Python >= 2.7, 3.4+
* Pandas >= 1.3.0
* Numpy >= 1.16.5
* requests >= 2.26
* lxml >= 4.9.1
* appdirs >= 1.4.4
* pytz >=2022.5
* frozendict >= 2.3.4
* beautifulsoup4 >= 4.11.1
* html5lib >= 1.1
* cryptography >= 3.3.2

## Note

The ```requirements.txt``` file should list all Python libraries that your notebooks depend on, and they will be installed using:

```python
pip install -r requirements.txt
```
