## Non-cost extension request justification

**Request type:** No-cost extension

**Current end date:** 31 December 2025

**Proposed end date:** 31 June 2025 (**extension of 6 months**)

**Reason for request:**
We experienced a one-year recruitment delay because finding good software engineers with expertise in Bonsai programming, neuroscience, and machine learning is difficult and time-consuming.

---

**Unused funds:**

*Staff*

Requested:

Role Name /Post Identifier Total cost on grant (£)
Researcher Co-Investigator Dr Joaquin Rapela 196864
Researcher Research Software Engineer 2 196864
Total £ 393728

Unused: £ 33,229

Justification:

One year delay in hiring Researcher Research Software Engineer 2

*Travel and Subsistence*

Requested:

Destination and purpose Total £
Outside UK RSE Conference travel and accommodation x 2 14400
Outside UK Travel and accommodation for invited speakers 13200.00
Total £ 27,600.00

Unused: £21,826

Justification:

- We did not attend the RSE conference.

- The invited speakers to our 2024 Bonsai Developers Conference paid their own tickets.


*Other Directly Incurred Costs*

Requested:

Description Total £
Bonsai workshop x2 2400
Conference fees x 2 2640
Engagement event 2400
Laptop x 2 6000
Training courses 2400
Total £ 15,840

Unused: £10,744

Justification:

- We hosted two Bonsai workshops at the SWC, with no cost.

- We attended the 2024 and 2025 SfN conference. The registration fees were paid by NeuroGEARS.

- The engagement events were hosted at the SWC, with no cost.

- We bought only one laptop, since the other laptop was donated by NeuroGEARS.

- The training courses were hosted at the SWC, with no cost.

---

**Progress to date:**

*Interoperability*

* Developed the [Python scripting package](https://bonsai-rx.org/python-scripting/) for interfacing Bonsai (C#) with Python.
* Developed the [Bonsai.ML.Torch package](https://bonsai-rx.org/machinelearning/articles/Torch/torch-overview.html), bringing Torch functionality to the Bonsai ecosystem.
* Added [Linux support to Bonsai](https://github.com/bonsai-rx/bonsai/releases/tag/2.8.20).

*Functionality integration*

* [Bonsai.ML.LinearDynamicalSystems](https://bonsai-rx.org/machinelearning/articles/LinearDynamicalSystems/lds-overview.html) — brought linear dynamical systems into Bonsai, enabling:

  * [Real-time inference of mouse kinematics](https://bonsai-rx.org/machinelearning/examples/examples/LinearDynamicalSystems/Kinematics/ModelOptimizationForagingMouse/README.html)
  * [Visual receptive-field estimation](https://bonsai-rx.org/machinelearning/examples/examples/LinearDynamicalSystems/LinearRegression/ReceptiveFieldSimpleCell/README.html)

* [Bonsai.ML.HiddenMarkovModels](https://bonsai-rx.org/machinelearning/articles/HiddenMarkovModels/hmm-overview.html) — integrated HMMs into Bonsai for tasks such as:

  * [Inferring mouse behavioral states from kinematics](https://bonsai-rx.org/machinelearning/examples/examples/HiddenMarkovModels/InferringBehavioralStateFromKinematics/README.html)

* [PointProcessDecoder](https://github.com/ncguilbeault/PointProcessDecoder): C# implementation of the Python point-process decoder [replay_trajectory_classification](https://github.com/Eden-Kramer-Lab/replay_trajectory_classification).

* [Bonsai.ML.PointProcessDecoder](https://bonsai-rx.org/machinelearning/articles/PointProcessDecoder/ppd-overview.html) — integrated [PointProcessDecoder](https://github.com/ncguilbeault/PointProcessDecoder) into Bonsai for neural decoding, including:

  * [Decoding position from hippocampal spikes](https://bonsai-rx.org/machinelearning/examples/examples/PointProcessDecoder/DecodePositionFromHippocampusClusterless/README.html)
  * [Decoding position from striatal spikes](https://bonsai-rx.org/machinelearning/examples/examples/PointProcessDecoder/DecodePositionFromStriatumSortedUnits/README.html)

*Dissemination*

* Organized the [Bonsai Developers Conference 2024](https://conference.bonsai-rx.org/2024/), which included a [Bonsai.ML session](https://conference.bonsai-rx.org/2024/program/#machine-learning).
* Hosted a Bonsai booth at the [Society for Neuroscience 2024](https://www.sfn.org/meetings/neuroscience-2024), with Bonsai.ML presentations.
* Visited Janelia Research Campus in 2024 and delivered talks on Bonsai and Bonsai.ML.
* Delivered Bonsai and Bonsai.ML lectures at the 2024 edition of the [Neuroinformatics course](https://neurogears.org/neuroinformatics-2024/), at University College London.
* Delivered Bonsai and Bonsai.ML lectures at the 2025 edition of the [Statistical Neuroscience course](https://neurogears.org/neuroinformatics-2025/), at University College London.
* Will host a Bonsai booth at the [Society for Neuroscience 2025](https://www.sfn.org/meetings/neuroscience-2025), with Bonsai.ML presentations.

---

**In progress**

*Functionality integration*

* [Bonsai.ML.Lds.Torch](https://github.com/bonsai-rx/machinelearning/pull/70) — TorchSharp implementation of [Bonsai.ML.LinearDynamicalSystems](https://bonsai-rx.org/machinelearning/articles/LinearDynamicalSystems/lds-overview.html), and its application to the [online estimation of neural latent processes](https://ncguilbeault.github.io/machinelearning/examples/examples/LinearDynamicalSystems/NeuralLatents/EstimatingParameters/README.html).
* [Bonsai.ML.OnlineBayesianLinearRegression](https://github.com/joacorapela/bonsai-Bonsai.ML-OnlineBayesianLinearRegression) — online Bayesian linear regression in Bonsai, with applications to [receptive-field estimation in cortical visual cells](https://github.com/joacorapela/bonsai-oblr-corticalSimpleCellEx).
* [Bonsai.ML.RecursiveLeastSquares](https://github.com/joacorapela/bonsai-rlsSimpleLinearRegression) — online recursive least-squares regression in Bonsai.

---

**Work remaining and plan:**

* Improve Bonsai.ML’s documentation:

  * Use the [style of scikit-learn’s documentation](https://scikit-learn.org/).
  * Create documentation for method developers, as Bonsai.ML currently only has documentation for method users.
* Enhance the [Bonsai.ML.PointProcessDecoder package](https://bonsai-rx.org/machinelearning/articles/PointProcessDecoder/ppd-overview.html) by adding clusterless decoding support for Neuropixels recordings; the current implementation only supports tetrode data.
* Collaborate with experimental neuroscientists in the application of Bonsai.ML tools to address state-of-the-art real-time experimental control problems and in the creation of Bonsai.ML use cases:

  * [Prof. Aman Saleem](https://www.saleemlab.com/), Institute of Behavioral Neuroscience, University College London: *Real-time forecasting of mouse position and head orientation for zero-lag stimuli display* (forecasting behavior with linear dynamical systems and deep neural networks).
  * [Prof. John O'Keefe](https://www.sainsburywellcome.org/web/groups/okeefe-lab), Sainsbury Wellcome Center, University College London: *Real-time detection of theta-sweeps in goal-driven navigation in the honeycomb maze* (point-process decoding with Neuropixels probes).
  * [Dr. Josh Siegle](https://alleninstitute.org/person/josh-siegle/), Allen Institute for Neural Dynamics, Seattle, US: *Real-time visualisation and forecasting of neural latent variables* (inference and forecasting with Gaussian and Poisson linear dynamical systems).

---

**Budget / resources:**
This is a **no-cost** request. The remaining work will be delivered within the existing award budget. 

