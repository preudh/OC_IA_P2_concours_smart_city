Project Setup Guide
Introduction

This guide outlines the steps to set up the development environment for our project using Miniconda. While it's feasible
to set up the environment using pure Python, we highly recommend Miniconda for more efficient dependency management.
This document also explains how to manage your project's dependencies using requirements.txt and environment.yml, 
ensuring reproducibility and seamless collaboration.
Why Miniconda?

Miniconda is a minimal installer for Conda, an open-source package management system and environment management system.
Here are some advantages of using Miniconda for this project:

    Efficient Management of Environments: Easily create and manage isolated environments for different projects, preventing conflicts between project dependencies.
    Flexible Dependency Management: Use environment.yml for Conda-specific dependencies and requirements.txt for pip-installable packages, combining the best of both worlds.
    Cross-Platform Compatibility: Miniconda works on Windows, macOS, and Linux, ensuring consistency across development setups.

Setting Up the Development Environment
Step 1: Install Miniconda

    Download and install Miniconda from the official website, following the instructions for your operating system.

Step 2: Create a Conda Environment

Create a new Conda environment with a specific Python version:

sh

conda create --name my_project_env python=3.8

Step 3: Activate the Environment

Activate the environment:

sh

conda activate my_project_env

Step 4: Manage Dependencies
Using requirements.txt

For pip-installable packages, use pip freeze to generate a requirements.txt file:

sh

pip freeze > requirements.txt

This file should be committed to your project repository. To install these dependencies:

sh

pip install -r requirements.txt

Using environment.yml

For managing dependencies that are installed via Conda, including those not available through pip,
create an environment.yml file:

yaml

name: my_project_env
channels:
  - conda-forge
  - defaults
dependencies:
  - numpy=1.19.2
  - pandas=1.1.3
  - matplotlib=3.3.4
  - pip:
      - some-pip-package==0.1.0

This file should also be committed to your project repository. To create an environment from this file:

sh

conda env create -f environment.yml

Step 5: Deactivate the Environment

Deactivate the environment when you're done:

sh

conda deactivate

Conclusion

Using Miniconda as the base for your project's development environment allows for efficient management of dependencies 
across multiple platforms. By leveraging requirements.txt for pip packages and environment.yml for Conda packages,
you can ensure that your environment is reproducible and manageable, making collaboration and deployment easier.
This setup strikes a balance between the flexibility of pip and the powerful environment management capabilities of Conda.