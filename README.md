# AI4P-RT

A collection of Python notebooks for teaching AI, with a particular focus on MONAI, to learners in the radiotherapy domain.

These notebooks were created for the 2nd UPLIFT School on **AI in Radiotherapy** and the AI4P|RT workshop held November 1–7, 2026, in Monte Verità, Switzerland.

The school [website](https://indico.psi.ch/event/18878/registrations/2885/) provides further information on the lectures.

## Choose your level

The hands-on tutorial is separated into three levels. Please choose the level that best matches your current experience and interests before the course.

| Level | Intended for | Main focus |
|---|---|---|
| **Level 1** | Non-coders or learners with very limited coding experience | Coding with LLMs, safe use of AI tools, and reviewing LLM-generated code |
| **Level 2** | Learners with Python experience who want to get started with AI | AI fundamentals, good practices, medical-imaging pipelines, and MONAI |
| **Level 3** | Learners with substantial AI/deep-learning experience | Competitive AI challenge based on an existing working pipeline |

Each level is intended to cover roughly **3 hours**.

Level hopping is welcome. If you start a level and find that it is too easy, too difficult, or simply not what you expected, move to another one.

### Before the course

Please choose a level and make sure that the required environment works on your laptop.

For **Levels 1 and 2**, please familiarize yourself with [Google Colab](https://colab.research.google.com/). You should be able to open a notebook, run cells, restart a runtime, and upload files.

For **Level 3**, please also make sure that you know how to select a GPU runtime and navigate/edit files in Colab. The actual challenge code and data will be supplied on site. See the Level 3 README for the spoiler-free preparation information.

You do not need to install a local Python environment for the course.

## Level 1 — Coding with LLMs

Level 1 is intended for non-coders or learners with very limited coding experience.

The focus is not on becoming a Python programmer in three hours. Instead, the goal is to learn how to use an LLM as a coding collaborator without giving up responsibility for the result.

Topics include:

- how to ask an LLM for code;
- how to break a problem into manageable steps;
- what information may or may not be appropriate to share with an external AI tool;
- debugging and reviewing generated code;
- recognizing unnecessary complexity;
- checking whether code is scientifically meaningful, not only whether it runs.

## Level 2 — AI fundamentals for medical imaging

Level 2 is intended for learners who already have some Python experience and want to understand the basic principles behind AI workflows in medical imaging.

The tutorial builds from data and problem formulation toward a small 3D segmentation workflow with MONAI.

The emphasis is on understanding what the pipeline is doing, what assumptions are being made, and how apparently small technical choices can affect the scientific result.

## Level 3 — AI challenge

Level 3 is intended for people with substantial AI/deep-learning experience.

Instead of following a step-by-step tutorial, you will receive a working baseline and compete to improve it.

The challenge package and data are supplied on site. The public repository intentionally does not reveal the full challenge in advance.

A small prize is offered during the UPLIFT School.

## Other tutorials and resources

This course heavily builds on existing tutorials and partly copies or reuses the same material. For in-depth documentation, refer to the official resources below.

- [MONAI tutorials](https://github.com/Project-MONAI/tutorials/)
- [The Carpentries deep-learning introduction](https://carpentries-lab.github.io/deep-learning-intro/)

The tutorial gears toward [MONAI](https://project-monai.github.io/) because it is tailored to medical applications and very useful for radiotherapy. In many radiotherapy applications, MONAI already provides the building blocks needed. In addition, MONAI is PyTorch at its core, so much of the training applies directly to PyTorch as well.

If you are looking for a more in-depth AI course, I can recommend the Carpentries tutorials. They are instructive and kept up to date.

A deep-learning book I recommend is *Deep Learning* by Ian Goodfellow, Yoshua Bengio, and Aaron Courville. It covers the fundamentals in considerably more depth than this tutorial.

## What this tutorial does not cover

Most modern AI applications go far beyond this deliberately simple tutorial.

We do not try to cover everything. In particular, we do not go deeply into topics such as transformer architectures, ensembles, or uncertainty estimation.

This is intentional. There are already many excellent resources for these topics, and adding more material would not necessarily make the hands-on course better.

The aim here is to provide a practical starting point and to make the important assumptions in an AI workflow visible.

## Course structure

The first hands-on block is dedicated to Levels 1–3.

In the second 3-hour block, you will be shown an overview of commercial software and 3D Slicer.

## FAQ — UPLIFT School participants

**Can I change level on site?**

Sure! We welcome level hopping depending on your skills and interests.

**Can I enter the challenge later?**

Yes. If you would like to compete, you can join Level 3 later or work on it in parallel with another level.

**When will the challenge winners be announced?**

The challenge concludes during the second hands-on course.

**Is the prize worth it?**

I think so, certainly.
