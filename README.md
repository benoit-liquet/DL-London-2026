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
| **Tutorial** | real-world applications, hands-on in Google Colab — [schedule](SCHEDULE.md) |

---

## Slides

| Slides | |
|---|---|
| **Overview of Deep Learning: Key Algorithms** | [PDF](slides/Deep_Learning_Lecture_London_2026.pdf) |
| **Deep Learning in Practice** — what to set, and why | [PDF](slides/Deep_Learning_Practice_London_2026.pdf) |

---

## Tutorials

The afternoon is hands-on, in **Google Colab**: nothing to install, a browser
and a Google account are enough.

> ### **[→ Schedule and notebooks for the afternoon](SCHEDULE.md)**
>
> The running order, the timing, and every notebook link are on that page.

**One thing to do first, for each notebook:** they open as shared, read-only
copies. Choose **File → Save a copy in Drive** and work in *your* copy,
otherwise nothing you type is kept. If a notebook asks for a GPU, use
**Runtime → Change runtime type → T4 GPU**.

---

## A small network in R, with nothing to install

Deep learning is usually written in Python, but a **small network on a small
table** is perfectly at home in R. These four illustrations use the
[`neuralnet`](https://cran.r-project.org/package=neuralnet) package, which is
pure R: no Python, no reticulate, no TensorFlow.

```r
install.packages(c("neuralnet", "ggplot2", "MASS"))
```

| Illustration | What it shows | |
|---|---|---|
| **A shallow network** | Boston housing: a linear model, then 3 neurons, then 8, then two layers. Which one wins? | [read](https://benoit-liquet.github.io/DL-London-2026/PRACTICE_R/Illustration-Shallow-NN.html) · [source](PRACTICE_R/Illustration-Shallow-NN.Rmd) |
| **Binary classification** | Breast cancer data: a logistic regression *is* a network with no hidden layer, then hidden layers are added and the parameters counted | [read](https://benoit-liquet.github.io/DL-London-2026/PRACTICE_R/Illustration-Binary-classification-task.html) · [source](PRACTICE_R/Illustration-Binary-classification-task.Rmd) |
| **A non-linear boundary** | two interleaved spirals, which no linear model can separate | [read](https://benoit-liquet.github.io/DL-London-2026/PRACTICE_R/Illustration-Non-linear-bundary.html) · [source](PRACTICE_R/Illustration-Non-linear-bundary.Rmd) |
| **Approximation ability** | how a network approaches an arbitrary function as units are added | [read](https://benoit-liquet.github.io/DL-London-2026/PRACTICE_R/Illustration_Approx_Ability.html) |

The data file for the second one, `Breast_cancer.RData`, sits next to the
sources in [PRACTICE_R](PRACTICE_R).

**What this is, and what it is not.** `neuralnet` trains fully connected
networks and nothing else: no convolutions, no sequence models, no mini-batches,
no dropout. It is the right tool to see a network work on a few hundred rows,
and the wrong one for anything in Parts 2 and 3 above. The last illustration is
provided as a rendered page only, because its source relies on Keras for R.

> Going further in R, outside this course: the
> [torch](https://torch.mlverse.org/) package runs natively, without Python.
> We do not use it here.

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
[chap3 (zip)](https://github.com/benoit-liquet/MLDL/blob/main/chap3.pdf.zip) ·
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
