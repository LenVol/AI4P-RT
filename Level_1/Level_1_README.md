# Level 1 — Coding with LLMs

Level 1 is intended for non-coders or learners with very limited coding experience who would like to use modern LLMs as coding collaborators.

You do **not** need previous AI experience.

Basic familiarity with opening a Google Colab notebook and running cells is helpful, but we will not assume that you are already comfortable writing Python from scratch.

The goal is to learn how to use an LLM to help with coding without handing over responsibility for the result.

## What to expect

Level 1 follows one continuous idea:

```text
share information safely
↓
ask clearly
↓
build something small
↓
debug and review it
```

The lessons use public medical-imaging examples and small Python/MONAI exercises.

The main questions to be answered: 

```text
Does this code do what I intended?
Do the assumptions make sense?
Is the code unnecessarily complicated?
What evidence do I have that the result is correct?
```

## Lessons

### Lesson 1 — Before You Paste

Before asking an LLM for help, we need to clearly set some rules:

> Am I allowed to give this information to this AI system?

Topics include:

- Shadow AI;
- institutional policy;
- patient and personal data;
- confidential information and secrets;
- data minimization;
- pseudonymisation versus anonymisation;
- DICOM metadata;
- using synthetic examples for debugging;
- why local or open-weight models are not automatically compliant or approved.

This lesson is educational material. Your institution's policies and applicable rules always take precedence over whats written here.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/lenvol/AI4P-RT/blob/main/Level_1/Level1_Lesson01_Before_You_Paste_Colab.ipynb]


### Lesson 2 — From Prompt to Program

We start with the basic question:

> How do I use an LLM as a coding collaborator *well*? 

where "well" in this context refers to: scientifically accurate, and technically sound. 

Topics include:

- why vague coding prompts lead to unpredictable code;
- how to specify context, task, constraints, expected output, and verification;
- why it is often useful to ask for a plan before asking for code;
- building programs in small testable steps;
- checking shapes, values, plots, and expected behaviour;
- recognizing unnecessary complexity;
- distinguishing **"the code ran"** from **"the code is correct."**

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/lenvol/AI4P-RT/blob/main/Level_1/Level1_Lesson02_From_Prompt_to_Program_Colab.ipynb]


### Lesson 3 — Build a Small AI Pipeline with an LLM

We then combine the previous lessons and use an LLM to help construct a small 3D medical-imaging AI pipeline.

The emphasis is on:

```text
small steps
clear scope
visible assumptions
verification
```

You do not need to understand every component in detail. You should, however, be able to explain what the code does and judge its scientific accuracy.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/lenvol/AI4P-RT/blob/main/Level_1/Level1_Lesson03_Build_a_Segmentation_Model_with_an_Open_LLM.ipynb]


### Lesson 4 — Debugging and Reviewing LLM-Generated Code

Finally:  

> the LLM generated my project codebase, now what? 

We look at:

- execution errors;
- logical errors;
- scientific errors;
- unnecessary complexity;
- debugging without replacing the whole program;
- preserving checks instead of deleting them;
- testing behaviour before and after refactoring;
- hidden notebook state and reproducibility;
- asking an LLM to review code without treating agreement as evidence.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/lenvol/AI4P-RT/blob/main/Level_1/Level1_Lesson04_Debugging_and_Reviewing_LLM_Code.ipynb]


## Which LLM should I use?

For the practical exercises, use an LLM that you are allowed to use.

If you work in Google Colab, Google's integrated Gemini interface is a convenient option because it is available directly next to the notebook.

The exact model is not important for the course and will probably change over time.

What **is** important:

- follow your institutional rules;
- do not enter patient or confidential institutional information unless that use is explicitly approved;
- use public or synthetic information for the course exercises;

## Computing environment

Level 1 is designed to run in **Google Colab**.

Before the course, please make sure that you can:

1. open a Colab notebook;
2. run individual cells;
3. restart a runtime;
4. upload a file if needed;
5. find the Colab file browser;
6. open the integrated Gemini panel, if you plan to use it.

You do not need to install Python locally.

A free Colab account is sufficient for the intended exercises.

## What LLM should I use
Use any capable model that you can access in an approved way. If you run these notebooks under Google colab, you could, for example, directly use Google's Gemini which you can access pressing the "toggle Gemini" button at the buttom of the page.

However, the exact model is intentionally not part of the lesson because available models and interfaces change quickly.

Examples of possible access patterns include:

```text
open-weight model in a browser interface
open-weight model hosted by your institution
local model through Ollama / LM Studio
approved research compute
```

For these lessons, the model only sees:

```text
public dataset names
generic Python code
generic error messages
```


## What you should bring

- a laptop;
- internet access;
- access to Google Colab;
- access to an LLM that you are permitted to use.

No patient data are required or should be brought for the exercises.

## Is Level 1 right for me?

Level 1 is probably a good choice if:

```text
"I do not really code."
"I can read some Python but would not write a program myself."
"I already use ChatGPT/Gemini for coding but I am not sure how much I should trust it."
"I want to understand how to ask for code and review the result."
```

If you already write Python comfortably and want to understand AI training, data pipelines, and MONAI in more depth, **Level 2 is probably a better starting point**.

You can change levels on site.
