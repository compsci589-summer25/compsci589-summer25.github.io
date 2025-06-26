# Assignment 1
📁 [Starter code](/pages/assignments/lib/assignment1_cs589.zip)

## Table of contents
- [Setup](#setup) (please read this carefully)
- [Goals](#goals)
- [Q1: k-Nearest Neighbor classifier](#q1-k-nearest-neighbor-classifier-30-points)
- [Q2: Training a Support Vector Machine](#q2-training-a-support-vector-machine-35-points)
- [Q3: Implement a Softmax classifier](#q3-implement-a-softmax-classifier-35-points)
- [Submitting your work](#submitting-your-work)


### [Setup](#setup)

Please familiarize yourself with the [recommended workflow](/pages/notes/doc/setup-instructions.html) before starting the assignment. 

The assignment would be using Python = 3.10

**Note**. Ensure you are periodically saving your notebook (`File -> Save`) so that you don't lose your progress if you step away from the assignment and the Colab VM disconnects.

Once you have completed all Colab notebooks **except `collect_submission.ipynb`**, proceed to the [submission instructions](#submitting-your-work).

#### Colab
If using colab, make a new folder, (ex. `cs589`) in Google Drive and upload the `assignment1` folder. Then, you right-click on any `.ipynb` file and click "Open with" → "Google Colaboratory".

After opening any notebook in Colab you will need to uncomment and run the first code cell. This will mount Google Drive, install all the datasets, and `cd` into the `assignment1` directory. You should be able to start then. If there is any problem, please feel free to ask us on Piazza.


#### Running locally

##### Downloading the datasets
Once you have the starter code, you will need to download the CIFAR-10 dataset.

Inside a colab notebook (ex. `knn.ipynb`), you can create a new cell (`Insert -> Code cell`) and run the following:

```bash
cd ./cs589/datasets
!bash get_datasets.sh
cd ../../
```

Alternatively, on your local computer run the following from the `assignment1` directory:

###### Mac & Linux
```bash
cd ./cs589/datasets
./get_datasets.sh
```

###### Windows

You can either download it directly from this [link](http://www.cs.toronto.edu/~kriz/cifar-10-python.tar.gz) and unzip it to `cifar-10-batches-py` in your `assignment1/cs589/datasets` folder.

Or, you can install it through your terminal with `bash` but this will be a lot more complicated. First, you need to install `bash` using [this guide](https://hackernoon.com/how-to-install-bash-on-windows-10-lqb73yj3). Then, you can run the following command.

```bash
cd ./cs589/datasets
bash get_datasets.sh
```

#### Jupyter Notebook
After you have the CIFAR-10 data, if you are not using colab you should start the Jupyter Notebook server from the
`assignment1` directory. You can do this in VSCode by downloading the [Jupyter extension](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter). 

If you are unfamiliar with Jupyter, you should read our
[Jupyter tutorial](/pages/notes/doc/jupyter-tutorial.html).

You can start the exercise by reading the instructions carefully and complete the **TODOs**. Do not forget to answer the inline questions. To write your response click on the text and then click the edit pencil icon that appears in the top right.

**NOTE:** If you are working in a virtual environment on OSX, you may encounter
errors with matplotlib due to the [issues described here](http://matplotlib.org/faq/virtualenv_faq.html). You can work around this issue by starting the Jupyter server using the `start_jupyter_osx.sh` script from the `assignment1` directory; the script assumes that your virtual environment is named `.env`.

### [Goals](#goals)

In this assignment you will practice putting together a simple image classification pipeline, based on the k-Nearest Neighbor or the SVM/Softmax classifier. The goals of this assignment are as follows:

- Understand the basic **Image Classification pipeline** and the data-driven approach (train/predict stages)
- Understand the train/val/test **splits** and the use of validation data for **hyperparameter tuning**.
- Develop proficiency in writing efficient **vectorized** code with numpy
- Implement and apply a k-Nearest Neighbor (**kNN**) classifier
- Implement and apply a Multiclass Support Vector Machine (**SVM**) classifier
- Implement and apply a **Softmax** classifier
- Understand the differences and tradeoffs between these classifiers
- Get a basic understanding of performance improvements from using **higher-level representations** than raw pixels (e.g. color histograms, Histogram of Gradient (HOG) features)

### [Q1: k-Nearest Neighbor classifier (30 points)](#q1-k-nearest-neighbor-classifier-30-points)

The Notebook **knn.ipynb** will walk you through implementing the kNN classifier.

### [Q2: Training a Support Vector Machine (35 points)](#q2-training-a-support-vector-machine-35-points)

The Notebook **svm.ipynb** will walk you through implementing the SVM classifier.

### [Q3: Implement a Softmax classifier (35 points)](#q3-implement-a-softmax-classifier-35-points)

The Notebook **softmax.ipynb** will walk you through implementing the Softmax classifier.

### [Submitting your work](#submitting-your-work)

**Important**. Please make sure that the submitted notebooks have been run and the cell outputs are visible.

Once you have completed all notebooks and filled out the necessary code, you need to follow the below instructions to submit your work:

To make sure everything is working properly, **remember to do a clean run ("Kernel -> Restart & Run All") after you finish work for each notebook** and submit the final version with all the outputs. 

**1.** Generate a zip file of your code (`.py` and `.ipynb`) called `<UmassID>.zip` (For email address `arnaik@umass.edu` - zip file name is `arnaik.zip`). Please ensure you do not include the dataset folder in the zip.

If you run code on your local machine on Linux or macOS,  you can run the provided `collectSubmission.sh` script from `assignment1/` to produce a file `<UmassID>.zip`. Alternatively, in any colab notebook you can run the command `!bash collectSubmission.sh`. Make sure to rename the zip to `<UmassID>.zip`.

**2.** Convert all notebooks (`.ipynb` files) into a single PDF file. In colab this can be done by selecting `File -> Print -> Print to PDF`.

**3.** Please submit <UmassID>.zip and the pdf to Gradescope.