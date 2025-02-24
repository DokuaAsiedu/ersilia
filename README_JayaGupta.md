<div id="top" align="center">
  
# Welcome to the **Ersilia Model Hub**!

[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/uk/fundraiser/charity/4145012) [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg)](code_of_conduct.md) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

[![documentation](https://img.shields.io/badge/-Documentation-purple?logo=read-the-docs&logoColor=white)](https://ersilia.gitbook.io/ersilia-book/) [![PyPI version fury.io](https://badge.fury.io/py/ersilia.svg)](https://pypi.python.org/pypi/ersilia/) [![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-370/) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?logo=Python&logoColor=white)](https://github.com/psf/black) [![Gitpod Ready-to-Code](https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/ersilia-os/ersilia)

</div>

![logo](https://github.com/ersilia-os/ersilia/blob/master/assets/Ersilia_Plum.png)

## Table of content
1. [Project Description](https://github.com/ersilia-os/ersilia#project-description)
2. [Features](https://github.com/ersilia-os/ersilia#features)
3. [Getting started](https://github.com/ersilia-os/ersilia#getting-started)
4. [Contribution](https://github.com/ersilia-os/ersilia#contribution)
5. [Roadmap](https://github.com/ersilia-os/ersilia#roadmap)
6. [License and citation](https://github.com/ersilia-os/ersilia#license-and-citation)
7. [About us](https://github.com/ersilia-os/ersilia#about-us)
8. [Follow us](https://github.com/ersilia-os/ersilia#Follow-us)  


# Project Description

The Ersilia Model Hub is the main project of the [Ersilia Open Source Initiative](https://ersilia.io). The Ersilia Model Hub's objective is to provide a platform for a user-friendly deployment of Artificial Intelligence and Machine Learning (AI/ML) models for drug discovery, where scientists can browse through the assets, identify those which is relevant to their research and obtain predictions without the need of coding expertise. We are building the Ersilia Model Hub, a free, open-source repository of Artificial Intelligence and Machine Learning (AI/ML) models for drug discovery. Our platform is aimed at helping researchers identify drug candidates for orphan and neglected diseases, design molecules de novo, understand mechanisms of action or anticipate adverse side effects.

The ultimate goal of Ersilia is to lower the barrier to drug discovery, encouraging academic groups and companies to pursue the development of new medicines following the principles of Open Science. Ersilia disseminates AI/ML models existing in the literature, as well as an in-house collection of models focused on diseases that are currently neglected by the pharmaceutical industry due to estimated low return on investment. We focus on establishing collaborations in low-resourced settings where the costs of drug discovery are prohibitive. We are on a mission to make scientific progress accessible to all. 

The models embedded in the hub include both models published in the literature (with appropriate third party acknowledgement) and models developed by the Ersilia team or contributors. All assets are open source, but please do check the Licenses of each model before using them.
* Read more about the project better at the [Ersilia Book](https://ersilia.gitbook.io/ersilia-book/)
* Available models can be checked at [Ersilia Model Hub](https://airtable.com/shr9sYjL70nnHOUrP/tblZGe2a2XeBxrEHP)

<img width="50%" src ="https://github.com/Jaya3112/ersilia/blob/5a06477b27692afc8901db590313f87d8ce0f892/assets/Ersilia%20goal%20img.png">


# Features

| Feature | Description |
| --- | --- |
| Data driven | Ersilia technology achieves state-of-the-art performance thanks to the integration of chemical, genomic and biomedical text data. Our AI tools are trained on millions of data points collected from the scientific literature and are available at no cost. [Click here](https://www.ersilia.io/publications)|
| Bioactivity signatures | Unlike conventional methods, we build upon bioactivity signatures, a richer representation of molecules. These embed all the experimental data for each compound, including targets and side-effects profiles, and are thus more powerful and clinically relevant predictors. [Click here](https://bioactivitysignatures.org/)|
| User friendly platform | Our tools are designed to facilitate the use of AI/ML tools. Scientists can browse a collection of models, choose the ones relevant to their research interests and run predictions without writing a single line of code. [Click here](https://www.ersilia.io/coming-soon)|
| Open source | All our assets are released under a permissive open source license. This means the scientific community can review, contribute and improve our code, resulting in tools validated more extensively than in the traditional peer-review system.  [Click here](https://github.com/ersilia-os)|
<p align="right">(<a href="#top">back to top</a>)</p>


# Getting Started

## Before you start

There are a few third-party pre-requisites and you need to have them installed on your computer before proceeding with the installation of the Ersilia tool.
1. [Python 3.7 and above](https://www.python.org/)
2.  [Conda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html) / [Anaconda](https://docs.anaconda.com/anaconda/install/index.html) / [Miniconda](https://docs.conda.io/en/latest/miniconda.html): the Ersilia tool will try to use it in order to handle dependencies safely and efficiently. 
3. [Docker](https://www.docker.com/): Please install Docker to ensure that all our AI/ML assets will work smoothly in your local device.
4. [Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) and [Git LFS](https://git-lfs.github.com/): All of our code is hosted in the Ersilia Github Organization profile

## Installation

### Install on Linux and MacOSX
**Open a terminal. The best is to set up a Conda environment.**

```
1 #create a [Conda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html) environment
2 conda create -n ersilia [Python 3.7](https://www.python.org/)
3 #activate the environment
4 conda activate ersilia
```
**Then, simply install the Ersilia Python package.**
```
1 #clone from github
2 https://github.com/ersilia-os/ersilia.git
3 cd ersilia
4 #install with pip (use -e for developer mode)
5 pip install -e .
```
**You should be done! Quickly check that the CLI works on your terminal.**
```
1 #see ersilia CLI options
2 ersilia --help
```
## The Isaura data lake
We highly recommend installation of the[Python 3.7](https://github.com/ersilia-os/isaura) data lake. With Isaura, you will be able to cache your model predictions (i.e. store them in your local computer). Isaura is a relatively light Python package:
```
1 #clone from github
2 git clone https://github.com/ersilia-os/isaura.git
3 cd isaura
4 #install with pip (use -e for developer mode)
5 pip install -e
```
## Install on Windows
>We are not testing Windows installation consistently. If you encounter problems, please reach out to us at hello@ersilia.io.

We recommend that you install Ubuntu on your Windows machine. This can be now done very easily with WSL. You will need at least Windows 10.
Open a Power Shell with Admin permissions and type:
```
1 wsl --install
```
Then simply install the [Ubuntu](https://www.microsoft.com/en-us/p/ubuntu/9nblggh4msv6#activetab=pivot:overviewtab) terminal on Windows.
Inside the Ubuntu terminal, you can now follow the installation instructions [above](https://github.com/ersilia-os/ersilia###Install-on-Linux-and-MacOSX).

For better installation guide of the Ersilia API Model, follow the detailed steps on the [ Ersilia Model Book](https://ersilia.gitbook.io/ersilia-book/quick-start/installation/).


# Contribution
The Ersilia Model Hub is developed and maintained by a small team of Ersilia employees and volunteers, and any contribution is highly valued! Below are the ways in which you can contribute to the development of this project:
* To improve our tool as a developer, check out the [Issues](https://github.com/ersilia-os/ersilia/issues)
* To include a Model you developed in the Hub, kindly [Contact us](https://ersilia.io/) or open an [Issue](https://github.com/ersilia-os/ersilia/issues)
* If you are a scientist with a cool dataset, also [Contact us](https://ersilia.io/) or open an [Issue](https://github.com/ersilia-os/ersilia/issues) as we might be interested in developing a Model based on the data!
* If there is a third-party model you have identified and would like to see it in the Hub, open an [Issue](https://github.com/ersilia-os/ersilia/issues) with the relevant information and we will get back to you as soon as possible.
* If you have any questions or concerns about this Model, kindly [Contact us](https://ersilia.io/)
The Ersilia Open Source Initiative adheres to the [Contributor Covenant](https://ersilia.gitbook.io/ersilia-wiki/code-of-conduct) guidelines.

*Contributions of any kind are Welcomed!!*


# Roadmap
We are working to grow the Hub organically and responding to our users needs. Here a detail of the next features to come, stay tuned!

1. Deployment for Windows System (expected: February 2022)
2. Automated third-party model contributions (expected: March 2022)
3. Possibility to run lite models online (expected: May 2022)

# License and Certification
This repository is open-sourced under the MIT License. Please [cite us](https://github.com/ersilia-os/ersilia/blob/master/CITATION.cff) if you use it.

# About us
The [Ersilia Open Source Initiative](https://ersilia.io/) is a Non Profit Organization incorporated with the Charity Commission for England and Wales (number 1192266). Our mission is to reduce the imbalance in biomedical research productivity between countries by supporting research in underfunded settings.
You can support us via [Open Collective](https://github.com/opencollective.com/ersilia).

# Follow us
* Subscribe to our [mailing list](https://twitter.com/ersiliaio)
* Twitter profile of [Gemma Turon](https://twitter.com/ersiliaio)
* Twitter profile of [Miquel Duran-Frigola](https://twitter.com/mduranfrigola) 
