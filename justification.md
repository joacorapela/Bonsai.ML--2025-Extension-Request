## Non-cost extension request justification

**Request type:** No-cost extension

**Current end date:** 31 December 2025

**Proposed end date:** 31 June 2025 (**extension of 6 months**)

**Reason for request:**
Experienced a one-year recruitment delay, because finding good software engineers with expertise in Bonsai programming, neuroscience and machine learning is difficult and time consuming.

**Progress to date:**

*Interoperability*
- developed the [Python scripting package](https://bonsai-rx.org/python-scripting/), for interfacing Bonsai (C#) with Python.
- developed the [Bonsa.ML.Torch package](https://bonsai-rx.org/machinelearning/articles/Torch/torch-overview.html), brining Torch functionality to the Bonsai ecosystem.
- added [support for Linux to Bonsai](https://github.com/bonsai-rx/bonsai/releases/tag/2.8.20).

*Functionality integration*
- created the [Bonsai.ML.LinearDynamicalSystems package](https://bonsai-rx.org/machinelearning/articles/LinearDynamicalSystems/lds-overview.html), integrating linear dynamical systems into Bonsai for, for example, [real-time inference of mice kinematics](https://bonsai-rx.org/machinelearning/examples/examples/LinearDynamicalSystems/Kinematics/ModelOptimizationForagingMouse/README.html) and [visual receptive field estimation](https://bonsai-rx.org/machinelearning/examples/examples/LinearDynamicalSystems/LinearRegression/ReceptiveFieldSimpleCell/README.html).
- created the [Bonsai.ML.HiddenMarkovModels package](https://bonsai-rx.org/machinelearning/articles/HiddenMarkovModels/hmm-overview.html), integrating hidden Markov models into Bonsai for, for example, [inferring mice behavioral states](https://bonsai-rx.org/machinelearning/examples/examples/HiddenMarkovModels/InferringBehavioralStateFromKinematics/README.html).
- created the [Bonsai.ML.PointProcessDecoder package](https://bonsai-rx.org/machinelearning/articles/PointProcessDecoder/ppd-overview.html), integrating a point-process decoder into Bonsai for, for example, [decoding animal position from hippocampal](https://bonsai-rx.org/machinelearning/examples/examples/PointProcessDecoder/DecodePositionFromHippocampusClusterless/README.html) or [strialal](https://bonsai-rx.org/machinelearning/examples/examples/PointProcessDecoder/DecodePositionFromStriatumSortedUnits/README.html) spikes.
- creating the [Bonsai.ML.Lds.Torch package](https://github.com/bonsai-rx/machinelearning/pull/70), a TorchSharp implementation of the Bonsai.ML.LinearDynamicalSystems package.
- creating an application of the [Bonsai.ML.Lds.Torch package](https://github.com/bonsai-rx/machinelearning/pull/70) for real-time estimation, visualisation and forecasting of neural latent variables.
- creating the Bonsai.ML.OnlineBayesianLinearRegression package to perform online Bayesian linear regression in Bonsai, with applications for the [estimation of receptive fields of cortical visual cells](https://github.com/joacorapela/bonsai-oblr-corticalSimpleCellEx).
- creating the [Bonsai.ML.RecursiveLeastSquares package](https://github.com/joacorapela/bonsai-rlsSimpleLinearRegression) to perform online recursive least squares regression in Bonsai.

*Dissemination*
- organized the [Bonsai Developers Conference 2024](https://conference.bonsai-rx.org/2024/), which included a [Bonsai.ML session](https://conference.bonsai-rx.org/2024/program/#machine-learning).
- hosted a Bonsai booth at the [Society for Neuroscience 2024](https://www.sfn.org/meetings/neuroscience-2024), with Bonsai.ML presentations.
- visited Janelia Research Campus in 2024 and delivered talks on Bonsai and Bonsai.ML.
- delivered Bonsai and Bonsai.ML lectures at the 2024 edition of the [Neuroinformatics course](https://neurogears.org/neuroinformatics-2024/), at the [Sainsbury Wellcome Centre](https://www.sainsburywellcome.org/web/).
- delivered Bonsai and Bonsai.ML lectures at the 2025 edition of the [Statistical Neuroscience course](https://neurogears.org/neuroinformatics-2025/), at the [Sainsbury Wellcome Centre](https://www.sainsburywellcome.org/web/).
- will host a Bonsai booth at the [Society for Neuroscience 2025](https://www.sfn.org/meetings/neuroscience-2025), with Bonsai.ML presentations.

**Work remaining and plan:**
- improve Bonsai.ML's documentation:
    - use the [style of scikit-learn's documentation](https://scikit-learn.org/).
    - create documentation for methods developers, as currently Bonsai.ML only has documentation for methods users.
- enhance [Bonsai.ML.PointProcessDecoder package](https://bonsai-rx.org/machinelearning/articles/PointProcessDecoder/ppd-overview.html) to add clusterless decoding support for Neuropixels recordings; the current implementation only supports tetrodes data.
- collaborate with experimental neuroscientists in the applications of Bonsai.ML tools to address state-of-the-art real-time experimental control problems and create Bonsai.ML use cases:
    - [Prof. Aman Saleem](https://www.saleemlab.com/) , Institute of Behavioral Neuroscience, University College London: *Real-time forecasting of mice position and head orientation for zero-lag stimuli display* (forecasting behavior with linear dynamical systems and deep neural networks).
    - [Prof. John O'Keefe](https://www.sainsburywellcome.org/web/groups/okeefe-lab), Sainsbury Wellcome Center, University College London: *Real-time detection of theta-sweeps in goal-driven navigation in the honeycomb maze* (point-process decoding with Neuropixels probes).
    - [Dr. Josh Siegle](https://alleninstitute.org/person/josh-siegle/), Allen Institute for Neural Dynamics, Seattle, US: *Real-time visualisation and forecasting of neural latent variables* (inference and forecasting with Gaussian and Poisson linear dynamical systems).

**Budget / resources:**
This is a **no-cost** request. The remaining work will be delivered within the existing award budget.
