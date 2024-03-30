In this open challenge, you will conduct an exploratory analysis with a dataset on the trees of the city of Paris as part
of the "Greening the City" program.

Your results will contribute to optimizing the rounds for the maintenance of the city's trees. Indeed, fewer rounds mean
fewer trips, and more trees maintained.

You will thus have a real impact on the future of the city of Paris!

### Data:

Download the dataset of the city of Paris trees.
You can also view it in context at opendata.paris.fr. https://opendata.paris.fr/explore/dataset/les-arbres


### Challenge Rules:

If you haven't done so already, set up your development environment on your computer, and create a virtual environment
dedicated to this challenge.
The data must be explored using Python and its libraries.
Submit your analysis in the form of a presentation, containing the following information:
- General presentation of the dataset
- Methodological approach to data analysis
- Synthesis of data analysis
The second deliverable will be in the form of a Jupyter Notebook. The Notebook will be documented to clarify the various
processes, calculations, or graphs that you perform using Jupyter's text editing features. Your explanations should allow
a non-technical audience to understand the different steps of your analysis and your synthesis.


### Setup:
- install anaconda, see https://www.anaconda.com/products/distribution
- in anaconda prompt, create a new environment as follows:
- Move to the directory where you want to create the environment
- in our case, create the environment in your project directory
- for example, if you want to create the environment .env in the directory D:\OC_IA\P2\OC_IA_P2_concours_smart_city
, you can do the following:
conda create --prefix D:\OC_IA\P2\OC_IA_P2_concours_smart_city\.env python=3.9
- Use 2 versions anterior to the latest version of python to ensure compatibility with the libraries you will use in 
your project. this will create a new environment in the directory D:\OC_IA\P2\OC_IA_P2_concours_smart_city\.env
- activate the environment
conda activate D:\OC_IA\P2\- Alternatively, after activating your environment, you can install libraries individually
using `pip`. This can be done within your Integrated Development Environment (IDE):
  - Open your IDE.
  - Open a terminal within the IDE.
  - Activate your environment with:
    ```
    conda activate D:\OC_IA\P2\OC_IA_P2_concours_smart_city\.env
    ```
  - Then install the libraries one by one using `pip`. For example:
    ```
    pip install pandas
    pip install numpy
    pip install matplotlib
    pip install seaborn
    pip install notebook  # This will install Jupyter Notebook
    ```

- install the libraries you will use in your project :
for example, to install pandas, numpy, matplotlib, seaborn, and jupyter notebook, you can do the following:
conda install pandas numpy matplotlib seaborn jupyter
- Alternatively, after activating your environment, you can install libraries individually using `pip`. This can be done
within your Integrated Development Environment (IDE):
  - Open your IDE.
  - Open a terminal within the IDE.
  - Activate your environment with:
    ```
    conda activate D:\OC_IA\P2\OC_IA_P2_concours_smart_city\.env
    ```
  - Then install the libraries one by one using `pip`. For example:
    ```
    pip install pandas
    pip install numpy 
    pip install matplotlib
    pip install seaborn
    pip install notebook  # This will install Jupyter Notebook
    ```
    
- For example ine the IDE Pycharm pro, you can open the project directory D:\OC_IA\P2\OC_IA_P2_concours_smart_city,
- you go to settings, then project: OC_IA_P2_concours_smart_city, then python interpreter, then you click on the gear
add, then select conda environment, then choose existing environment
- (i.e. in our case D:\OC_IA\P2\OC_IA_P2_concours_smart_city\.env), then click on ok, then click on ok
- 
### References:
- For details on conda and virtual environments, refer to the [Conda Environment Management Guide]
(https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html).
- Jupyter Notebook is typically included with the Anaconda installation. For more information, visit [Jupyter Installation]
(https://jupyter.org/install). If you do not have Anaconda, you can install Jupyter Notebook separately.
- Pandas may not be installed by default with Jupyter Notebook if you are not using the Anaconda distribution.
For installation instructions, see the [Pandas Installation Guide](https://pandas.pydata.org/docs/getting_started/install.html). 
With Anaconda, Pandas is included.
- Matplotlib is a separate library that does not come pre-installed with Pandas unless you are using Anaconda.
For standalone installation, consult the [Matplotlib Installation Guide](https://matplotlib.org/stable/users/installing.html).
- Seaborn is a visualization library that is not installed with Pandas by default. You can install it following the
[Seaborn Installation Instructions](https://seaborn.pydata.org/installing.html), though it is included with Anaconda.
- Numpy is a fundamental package for scientific computing with Python and is a dependency for Pandas. While installing
Pandas will typically install Numpy as well, you may need to install it separately if not using Anaconda. For more, see
[Numpy for Absolute Beginners](https://numpy.org/doc/stable/user/absolute_beginners.html).
