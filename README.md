Hands-on-Machine Learning Notebooks
==========================

This repository aims at teaching you the fundamentals of Machine Learning in
python.

## Quick Start

### Want to install this repository on your own machine?

Start by installing [Anaconda](https://www.anaconda.com/distribution/) (or [Miniconda](https://docs.conda.io/en/latest/miniconda.html)), [git](https://git-scm.com/downloads), and if you have a TensorFlow-compatible GPU, install the [GPU driver](https://www.nvidia.com/Download/index.aspx), as well as the appropriate version of CUDA and cuDNN (see TensorFlow's documentation for more details).

Next, clone this project by opening a terminal and typing the following commands (do not type the first `$` signs on each line, they just indicate that these are terminal commands):

    $ git clone https://github.com/Sangramsingkayte/Hands-on-Machine-Learning.git 
    $ cd Hands-on-Machine-Learning

Next, run the following commands:

    $ conda env create -f environment.yml
    $ conda activate tf1
    $ python -m ipykernel install --user --name=python3

Finally, start Jupyter:

    $ jupyter notebook


**Which Python version should I use?**

I recommend Python 3.7. If you follow the installation instructions above, that's the version you will get. Most code will work with other versions of Python 3, but some libraries do not support Python 3.8 or 3.9 yet, which is why I recommend Python 3.7.

**I'm getting an error when I call `load_housing_data()`**

Make sure you call `fetch_housing_data()` *before* you call `load_housing_data()`. If you're getting an HTTP error, make sure you're running the exact same code as in the notebook (copy/paste it if needed). If the problem persists, please check your network configuration.

**I'm getting an SSL error on MacOSX**

You probably need to install the SSL certificates (see this [StackOverflow question](https://stackoverflow.com/questions/27835619/urllib-and-ssl-certificate-verify-failed-error)). If you downloaded Python from the official website, then run `/Applications/Python\ 3.7/Install\ Certificates.command` in a terminal (change `3.7` to whatever version you installed). If you installed Python using MacPorts, run `sudo port install curl-ca-bundle` in a terminal.

**I've installed this project locally. How do I update it to the latest version?**

See [INSTALL.md](INSTALL.md)

**How do I update my Python libraries to the latest versions, when using Anaconda?**

See [INSTALL.md](INSTALL.md)

## Contributors
I would like to thank everyone [who contributed to this project](https://github.com/ageron/handson-ml/graphs/contributors), either by providing useful feedback, filing issues or submitting Pull Requests. Special thanks go to Haesun Park and Ian Beauregard who reviewed every notebook and submitted many PRs, including help on some of the exercise solutions. Thanks as well to Steven Bunkley and Ziembla who created the `docker` directory, and to github user SuperYorio who helped on some exercise solutions.
