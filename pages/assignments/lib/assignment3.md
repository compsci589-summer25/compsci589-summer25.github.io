# Assignment 3
📁 [Starter code](/pages/assignments/lib/assignment3.zip)

## Table of contents
- [Setup](#setup)
- [Goals](#goals)
- [Q1: Deep Generative Model (50 points)](#q1-deep-generative-model-50-points)
- [Q2: Reinforcement Learning (50 points)](#q2-reinforcement-learning-50-points)
- [Submitting your work](#submitting-your-work)


### [Setup](#setup)

Please familiarize yourself with the [recommended workflow](/pages/notes/doc/setup-instructions.html) before starting the assignment. 

The assignment would be using Python = 3.10

Make sure you install all the requirements with the command below in your terminal

```bash
pip install -r requirements.txt
```

**Note**. Ensure you are periodically saving your notebook (`File -> Save`) so that you don't lose your progress if you step away from the assignment and the Colab VM disconnects.

Once you have completed all Colab notebooks **except `collect_submission.ipynb`**, proceed to the [submission instructions](#submitting-your-work).

#### Colab

If using colab, make a new folder, (ex. `cs589`) in Google Drive and upload everything into the `assignment2` folder. Then, you right-click on any `.ipynb` file and click "Open with" → "Google Colaboratory".

If there is any issue with module being missing, try adding the line below:

```bash
!pip install -r missing-library
```

#### Running locally

If you're planning to run the code locally, make sure you downloaded this [VSCode extension](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter). 

### [Goals](#goals)

In **Q1**, you will be building a simple LLM with an autoregressive model and completing some free-response exercises.

In **Q2**, you will use the Q-learning algorithm to build an agent that can move through a 2D environment and help it reach its target

### [Q1: Neural Network (50 points)](#q1-neural-network-35-points)

For **Q1.1**, the notebook **dgm.ipynb** will walk you through building an autoregressive model.

**Q1.2** will be free-response questions. Keep your answer relatively concise (Max 5 sentences).

### [Q2: Reinforcement Learning (50 points)](#q2-decision-tree-35-points)

The notebook **rl.ipynb** will walk you through implementing an agent with Q-learning algorithm to evaluate reward and move closer to the target grid.

### [Submitting your work](#submitting-your-work)

**Important**. Please make sure that the submitted notebooks have been run and the cell outputs are visible.

1. Select every files in the `assignment3` folder and compress them into a zip file. Your zip file's contents should have the following structure:

```
├── dgm.ipynb
├── rl.ipynb
```

2. Convert all notebooks (`.ipynb` files) into a single PDF file. In colab this can be done by selecting `File -> Print -> Print to PDF`. After that, merge them into one PDF to submit to Gradescope. I recommend using this [website](https://tools.pdf24.org/en/merge-pdf) for merging but you can use any tool you like. Submit the merged PDF file to Gradescope and assign each page to their corresponding question. You might lose points if there are missing pages assigned to the question so make sure you assign the pages correctly.

If you have any question, please feel free to message us on Piazza. Thanks for your time!