# Level 2 — AI Fundamentals for Medical Imaging

Level 2 is intended for those have some Python experience and would like to understand how to build an AI workflow from scratch.

You do not need previous AI experience. We go over the most important basics. 

The examples are aimed at learners from radiotherapy and medical imaging. Domain know-how is assumed as a give. The lessons teach what info an AI model sees. how it learns, and how we judge whether the result is meaningful.

## What to expect

Level 2 moves from understanding *the problem* and *available data* toward a complete *model* for image segmentation. 

The overall progression is:

```text
What is the problem?
↓
What information is in the data?
↓
How does a neural network learn?
↓
How do we build a medical-imaging data pipeline?
↓
How do we combine everything into a 3D segmentation model?
```

The goal is explicitely not state-of-the-art performance.

After the course, you should understand the main components of an AI workflow well enough to reason about them.

## Lessons

### Lesson 1 — Understanding the Data

We start with questions such as:

```text
What are data and labels/targets?
What information has preprocessing preserved or removed?
What is the independent unit in the dataset?
Could there be leakage?
Could the model exploit a shortcut?
Does this dataset actually contain the information needed for the task?
```

The central idea is:

> A sophisticated model cannot recover information that was never presented to it.

We use a small medical-imaging classification dataset so that we can focus on problem formulation, representation, dataset suitability, splitting, leakage, and exploratory analysis.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/lenvol/AI4P-RT/blob/main/Level_2/Level2_Lesson01_Understanding_Data.ipynb]

### Lesson 2 — A First AI Model

We then train a small neural network.

We use the model to understand:

- batches and epochs;
- model parameters;
- logits and probabilities;
- cross-entropy loss;
- gradients;
- optimization;
- training versus validation;
- convergence and overfitting;
- loss versus metrics;
- learned representations.

We want to understand:

> What exactly did the model learn from the information we gave it?

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/lenvol/AI4P-RT/blob/main/Level_2/Level2_Lesson02_My_First_AI_Model.ipynb]


### Lesson 3 — From Medical Images to Model-Ready Data with MONAI

Next we build on a generic image to achieve a realistic medical-imaging data pipeline.

We use MONAI to look at:

- dictionary-based transforms;
- `Compose`;
- image orientation and voxel spacing;
- intensity preprocessing;
- image versus label interpolation;
- deterministic preprocessing versus random augmentation;
- patch sampling;
- `Dataset`, `CacheDataset`, and `DataLoader`;
- separate training and validation pipelines.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/lenvol/AI4P-RT/blob/main/Level_2/Level2_Lesson03_MONAI_Data_Pipelines.ipynb]


### Lesson 4 — Our First 3D Segmentation Model with MONAI

The final lesson combines the previous lessons into a complete small 3D segmentation workflow:

```text
medical-image files
↓
MONAI transforms
↓
training patches
↓
3D U-Net
↓
voxel-wise prediction
↓
Dice loss
↓
training
↓
sliding-window inference
↓
3D segmentation
```

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/lenvol/AI4P-RT/blob/main/Level_2/Level2_Lesson04_3D_Segmentation_with_MONAI.ipynb]


## What you should be comfortable with

Level 2 assumes familiarity with basic **Python**.

You do not need to be an experienced software developer. You also do not need to know deep learning frameworks such as PyTorch, TensorFlow or MONAI in advance.

If basic Python syntax is already a major obstacle, **Level 1 may be a better starting point**.

If you already train deep-learning models independently and want a less guided task, challenge yourself with **Level 3**.

## Computing environment

Level 2 is designed to run in **Google Colab**.

Before the course, please make sure that you can:

1. open and run a Colab notebook;
2. restart a runtime;
3. use the file browser;
4. change the runtime type;
5. enable a GPU when one is available.

Most of the early lessons are lightweight.

A GPU is useful for the final 3D segmentation exercise, but no paid compute is required.

You do not need to install a local Python environment.

## Data

The course uses small public or synthetic teaching datasets.

The notebooks download or create the data they use.

## What this level does not try to cover

We deliberately keep the examples relatively lightweigth.

Topics such as large transformer models, ensembles, deployment, and uncertainty estimation are outside the scope of Level 2.

