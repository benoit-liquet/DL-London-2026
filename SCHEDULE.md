# Afternoon session — schedule and notebooks

**Thursday 17 September 2026 — Deep Learning day**
Exposome Analytics Summer School, Imperial School of Public Health, London.

[← back to the main page](README.md)

---

## Before we start

**Make your own copy of every notebook.** The links below open shared,
read-only notebooks. Use **File → Save a copy in Drive** and work in the copy,
otherwise nothing you type is saved.

**Two different environments, and that is on purpose.** The first notebooks use
**Keras/TensorFlow**, the ones on images use **PyTorch**. They are the two
libraries you will meet in the literature, they do the same things with a
different syntax, and seeing both is useful. The concepts of the morning
— layers, loss, epochs, batches — are identical in each.

> *A word on Keras, since the question comes up.* Keras is not abandoned:
> version **3** is current, and it now runs on top of **TensorFlow, PyTorch or
> JAX** indifferently. What has changed is that PyTorch has become dominant in
> research, and TensorFlow less visible than it was.

---

## Schedule

Three hours of notebooks, after half an hour of slides.

| | | Duration | Running total |
|---|---|---|---|
| **0** | **Slides** — *Deep Learning in Practice* | 30 min | 0:30 |
| **1** | **A small network in R** — demonstration | 20 min | 0:50 |
| **2** | **Practice 1** — a first network on a table of data | 30 min | 1:20 |
| **3** | **Practice 4** — MNIST, and can you beat it? | 40 min | 2:00 |
| **4** | **CNN Practice 1** — a pretrained VGG19 in action | 10 min | 2:10 |
| **5** | **CNN Practice 3** — the same MNIST, with a CNN | 30 min | 2:40 |
| **6** | **CNN Practice 4** — MedMNIST, medical images | 30 min | 3:10 |
| **7** | **CNN Practice 5** — transfer learning | 20 min | 3:30 |

If the group moves quickly, two more are ready at the end.

---

## 1 — A small network in R *(20 min, demonstration)*

No Python here, and nothing heavy to install:

```r
install.packages(c("neuralnet", "ggplot2", "MASS"))
```

| | |
|---|---|
| A shallow network, Boston housing | [read](https://benoit-liquet.github.io/DL-London-2026/PRACTICE_R/Illustration-Shallow-NN.html) |
| Binary classification, breast cancer | [read](https://benoit-liquet.github.io/DL-London-2026/PRACTICE_R/Illustration-Binary-classification-task.html) |
| A non-linear boundary, two spirals | [read](https://benoit-liquet.github.io/DL-London-2026/PRACTICE_R/Illustration-Non-linear-bundary.html) |
| Approximation ability | [read](https://benoit-liquet.github.io/DL-London-2026/PRACTICE_R/Illustration_Approx_Ability.html) |

The point of this first half hour: a network on a few hundred rows is an
ordinary model, and it lives perfectly well in the environment you already use.

---

## 2 — Practice 1: a first network on a table of data *(30 min)*

[**Open in Colab**](https://colab.research.google.com/github/benoit-liquet/DL-London-2026/blob/main/notebooks/DNN_Practice_1_London.ipynb)

Breast cancer data, 569 patients, 30 features — the same data as the R
illustration, now in Keras.

* a logistic regression, written as a network with **no hidden layer**
* one hidden layer with 4 neurons, then 10, then two layers
* the parameter count of each, and the two curves to watch
* `EarlyStopping`: stop at the right epoch instead of a round number

Mostly you press *Run*. Take the time to read `model.summary()` each time.

---

## 3 — Practice 4: MNIST, and can you beat it? *(40 min)*

[**Open in Colab**](https://colab.research.google.com/github/benoit-liquet/DL-London-2026/blob/main/notebooks/DNN_Practice_4_London.ipynb)

> Switch to a GPU first: **Runtime → Change runtime type → T4 GPU**.

We run together down to *Improve our model by tuning some parameters*, and note
the test accuracy of the first model.

**Then it is your turn.** A red panel in the notebook lists what to change, one
thing at a time: the number of units, a third layer, another optimizer, the
batch size, early stopping, batch normalisation, dropout. Try to beat the first
result, and keep a note of what worked.

The rest of the notebook does the same sweep systematically, so run your own
variants **before** reading the answer.

---

## 4 — CNN Practice 1: a pretrained VGG19 in action *(10 min)*

[**Open in Colab**](https://colab.research.google.com/drive/1dtH3UHSfbK5Ss9E9ogtYG5YQzc5fTXNE)

No training at all. We download a network with 144 million parameters, already
trained on ImageNet, give it an image, and read what comes out. Ten minutes for
the figure you saw this morning, running for real.

---

## 5 — CNN Practice 3: the same MNIST, with a CNN *(30 min)*

[**Open in Colab**](https://colab.research.google.com/drive/1Foo-KTWMiJV-sl0mRaZnWHnk05VQLyUB)

Same data as Practice 4, same task, but convolutions instead of dense layers.
Compare the accuracy with the score you wrote down earlier, and compare the
number of parameters too. This is the point of the whole morning on
convolutions, in a single number.

---

## 6 — CNN Practice 4: MedMNIST *(30 min)*

[**Open in Colab**](https://colab.research.google.com/drive/1kmTZ-ypepEpcfNZB_qIB8ILK201KhkEp)

Medical images, in PyTorch. A complete pipeline: loading, a small convolutional
network, training over 5 epochs, evaluation.

---

## 7 — CNN Practice 5: transfer learning *(20 min)*

[**Open in Colab**](https://colab.research.google.com/drive/1EEevV5WUsRwmALZDxTl57Ol5nT89ylbd)

Same data as the previous one. Instead of training from nothing, we take a
network already trained on ImageNet, freeze it, and replace only its last layer.
This is the recipe from the slides, and the one that matters when you have a few
hundred images rather than a million.

---

## If there is time left

| | | |
|---|---|---|
| **RNN Practice 1** | RNN and LSTM on a synthetic time series | [open in Colab](https://colab.research.google.com/drive/1VMNmL1YKZHZBJip8f5tcEMxj5VlCIfbM) |
| **RNN Practice 4** | classification of ECG signals | [open in Colab](https://colab.research.google.com/drive/10sCO57yzS2env2RHSFH5eO2NwCxv6VL2) |

---

## Not covered today, but yours to keep

These run exactly as they are, at home, with a GPU runtime:

| | | |
|---|---|---|
| DNN Practice 2, Practice 3 | more on dense networks | [2](https://colab.research.google.com/drive/1gpr8Xl5Y51-dYDQ1BA6lNcJ8yZq3GPvr) · [3](https://colab.research.google.com/drive/12PETdpB2B0Y2mTGzYUQ8X6M0GxRo4cQN) |
| CNN Practice 2 | CIFAR-10, in PyTorch *and* in Keras | [open](https://colab.research.google.com/drive/1Ru1wRki8yUxx5W2G4Of5-drTRtsZ3_Ym) |
| RNN Practice 2 | sentiment on IMDb, with RNN and LSTM | [open](https://colab.research.google.com/drive/1MnvITjntB9AmHL2BN_03hGQcDxNVom4B) |
| RNN Practice 3 | the same, with a transformer | [open](https://colab.research.google.com/drive/10HN5da584vuDld6Go9QceNIyGRfrsKCg) |
| RNN Practice 5 | classification of symptoms | [open](https://colab.research.google.com/drive/1agCKQMWCrs85yciGEMWQQTnWEBzF_9IF) |

---

<details>
<summary><b>Solutions</b> — open this at the end of the session</summary>

<br>

| | |
|---|---|
| Solution, CNN Practice 2 | [open in Colab](https://colab.research.google.com/drive/1fhdo9d2UE5EsVppW2-s6yQngvFiwYGIg) |
| Solution, CNN Practice 3 | [open in Colab](https://colab.research.google.com/drive/1wZ_LJTmoCfJ4Ca7B38Hd7TnwuitBMAKV) |

</details>

---

[← back to the main page](README.md)
