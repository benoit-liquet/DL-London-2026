# Deep Learning — Exposome Analytics Summer School, London 2026

Material for the **Deep Learning** day of the Exposome Analytics Summer School,
Imperial School of Public Health, London, 14–18 September 2026.

> Course page:
> [Exposome Analytics: from Causal Models to AI](https://www.imperial.ac.uk/school-public-health/study/short-courses/exposome-analytics-from-causal-models-to-ai/)

**Thursday 17 September — Prof. Benoit Liquet**
LMAP, Université de Pau et des Pays de l'Adour

---

## How to get the material

The simplest way is to take everything at once:

> Click the green **`< > Code`** button at the top of this page, then
> **Download ZIP**. Unzip it, and you have the slides and this page on your
> machine.

You can also open any single file above and use its own download button.
The **tutorials are not in the ZIP**: they run online, see below.

---

## Programme of the day

| | |
|---|---|
| **Overview of Deep Learning** | what the models are, and the mathematics behind them |
| **Key Algorithms** | fully connected networks, convolutional networks, sequence models, attention, transformers |
| **Tutorial** | real-world applications, hands-on in Google Colab |

---

## Slides

| Slides | |
|---|---|
| **Overview of Deep Learning: Key Algorithms** | [PDF](slides/Deep_Learning_Lecture_London_2026.pdf) |
| **Deep Learning in Practice** — what to set, and why | [PDF](slides/Deep_Learning_Practice_London_2026.pdf) |

---

## Tutorials

All practicals run in **Google Colab**. Nothing to install: a browser and a
Google account are enough.

### Before you start — please follow this procedure

The notebooks below are **shared, read-only** copies. If you type in them
directly, your work is not saved. Make your own copy first:

1. **Click** the link of the notebook. It opens in Google Colab.
2. **Sign in** with your Google account, top right.
3. In the menu, choose **File → Save a copy in Drive**.
4. A new tab opens, titled *Copy of ...* — **this is your copy**. Work in that
   one. It is saved automatically in your Drive, and you can come back to it
   after the school.

The first cell may take a minute to start: Colab is allocating a machine for
you. If a notebook asks for a GPU, use **Runtime → Change runtime type → GPU**.

### Part 1 — Deep Neural Networks

| | Notebook |
|---|---|
| 1 | [Practice 1](https://colab.research.google.com/drive/1GDdmVTk_Y_SUKvDrVWPf8CKj-M6r0NyG) |
| 2 | [Practice 2](https://colab.research.google.com/drive/1gpr8Xl5Y51-dYDQ1BA6lNcJ8yZq3GPvr) |
| 3 | [Practice 3](https://colab.research.google.com/drive/12PETdpB2B0Y2mTGzYUQ8X6M0GxRo4cQN) |
| 4 | [Practice 4](https://colab.research.google.com/drive/1Msg2GDt5P0kB0MVPSPUcGZGIxDjOgoDb?usp=sharing) |

### Part 2 — Convolutional Neural Networks

| | Notebook |
|---|---|
| 1 | [Practice 1](https://colab.research.google.com/drive/1dtH3UHSfbK5Ss9E9ogtYG5YQzc5fTXNE) |
| 2 | [Practice 2](https://colab.research.google.com/drive/1Ru1wRki8yUxx5W2G4Of5-drTRtsZ3_Ym) |
| 3 | [Practice 3 — MNIST](https://colab.research.google.com/drive/1Foo-KTWMiJV-sl0mRaZnWHnk05VQLyUB) |
| 4 | [Practice 4 — medMNIST](https://colab.research.google.com/drive/1kmTZ-ypepEpcfNZB_qIB8ILK201KhkEp) |
| 5 | [Practice 5 — Transfer Learning](https://colab.research.google.com/drive/1EEevV5WUsRwmALZDxTl57Ol5nT89ylbd) |

### Part 3 — Sequence Models

| | Notebook |
|---|---|
| 1 | [Practice 1](https://colab.research.google.com/drive/1VMNmL1YKZHZBJip8f5tcEMxj5VlCIfbM) |
| 2 | [Practice 2](https://colab.research.google.com/drive/1MnvITjntB9AmHL2BN_03hGQcDxNVom4B) |
| 3 | [Practice 3](https://colab.research.google.com/drive/10HN5da584vuDld6Go9QceNIyGRfrsKCg) |
| 4 | [Practice 4 — ECG classification](https://colab.research.google.com/drive/10sCO57yzS2env2RHSFH5eO2NwCxv6VL2) |
| 5 | [Practice 5 — Symptoms classification](https://colab.research.google.com/drive/1agCKQMWCrs85yciGEMWQQTnWEBzF_9IF) |

---

## Going further

The full three-day course on machine learning and deep learning is available in
a separate repository:

**[benoit-liquet/MLDL](https://github.com/benoit-liquet/MLDL)**

### Lecture notes and course notebooks

The [DeepLearning](https://github.com/benoit-liquet/MLDL/tree/main/DeepLearning)
folder contains, for each topic, the lecture slides and the full course notebook:

| | |
|---|---|
| Deep Neural Networks | [lecture (PDF)](https://github.com/benoit-liquet/MLDL/blob/main/DeepLearning/Lecture_DNN_2025.pdf) · [notebook](https://github.com/benoit-liquet/MLDL/blob/main/DeepLearning/Deep_learning_DNN_2025.nb.html.zip) |
| Convolutional Neural Networks | [lecture (PDF)](https://github.com/benoit-liquet/MLDL/blob/main/DeepLearning/Lecture_CNN_2025.pdf) · [notebook](https://github.com/benoit-liquet/MLDL/blob/main/DeepLearning/Deep_learning_CNN_2025.nb.html.zip) |
| Sequence Models | [lecture (PDF)](https://github.com/benoit-liquet/MLDL/blob/main/DeepLearning/Lecture_RNN_2025.pdf) · [notebook](https://github.com/benoit-liquet/MLDL/blob/main/DeepLearning/Deep_learning_RNN_2025_new.nb.html.zip) |

The [MachineLearning](https://github.com/benoit-liquet/MLDL/tree/main/MachineLearning)
folder covers supervised learning, and
[DATA](https://github.com/benoit-liquet/MLDL/tree/main/DATA) holds the datasets
used in the practicals.

### The mathematical background

If you want to revise the mathematics before the day, start here:

> **[Navigating Mathematical Basics: A Primer for Deep Learning in Science](https://github.com/benoit-liquet/MLDL/blob/main/deep_learning_math_background.pdf)**

### Book chapters

Chapters of *Mathematical Engineering of Deep Learning*, in the MLDL repository:

[chap1](https://github.com/benoit-liquet/MLDL/blob/main/chap1.pdf) ·
[chap2](https://github.com/benoit-liquet/MLDL/blob/main/chap2.pdf) ·
[chap3](https://github.com/benoit-liquet/MLDL/blob/main/chap3.pdf) ·
[chap4](https://github.com/benoit-liquet/MLDL/blob/main/chap4.pdf) ·
[chap5](https://github.com/benoit-liquet/MLDL/blob/main/chap5.pdf) ·
[chap6](https://github.com/benoit-liquet/MLDL/blob/main/chap6.pdf) ·
[chap7](https://github.com/benoit-liquet/MLDL/blob/main/chap7.pdf)

---

## Book

The material is based on:

> Liquet, B., Moka, S., Nazarathy, Y. (2024).
> *Mathematical Engineering of Deep Learning*, 1st edition.
> Available online: [deeplearningmath.org](https://deeplearningmath.org)

---

## Contact

Benoit Liquet — benoit.liquet@univ-pau.fr
