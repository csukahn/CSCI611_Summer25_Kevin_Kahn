1. The project contains two Jupyter Notebooks (.ipynb files). The code within each notebook can be run as is, starting from the top as long as you have a python environment and the following Python libraries installed, or you can use the included conda environment:
- matplotlib
- cv2
- numpy
- torch
- torchvision
- torchviz
- torchinfo
- IPython

2. To activate and use the Conda environment, use these two commands:
    - `conda env create -f environment.yml`
    - `conda activate torch_env`

3. If you would like to use these notebooks, you will unfortunately have to download the CIFAR 10 file `cifar-10-python.tar.gz` and add it to the `build_cnn/data` directory since github doesn't allow files over 100MB to be uploaded.

3. The `image_filtering.ipynb` notebook isn't optimized for running on a GPU, but the build_cnn.ipynb is optimized to run on either a GPU or CPU. It will automatically run the correct commands dependent on if a proper GPU is available to run on.

4. The CNN notebook contains a couple extra code blocks at the bottom to display summary information and a plot of the CNN architecture.

5. File details:
    - The `Report.ipynb` file contains some results and observations taken from the CNN playbook
    - The `image_filtering.ipynb` file contains some basic filtering and transformations for images
    - The `build_cnn.ipynb` file contains the code needed to train a model on the CIFAR-10 image dataset with images of pixel size 32x32, and containing 10 classifications of images (i.e. airplane, bird, cat, etc.)
    - `environment.yml` contains all of the python packages needed for the project if you don't want to use your own environment.