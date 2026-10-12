# Term Project Overview

In this term project, you will design, implement, and evaluate a complete **machine learning project** for a real-world problem.

The goal of the project is not simply to run several machine learning algorithms and report their performance. You should clearly define the learning problem, understand and prepare the data or environment, establish appropriate baselines, design a meaningful evaluation strategy, compare machine learning approaches, analyze the results, and discuss the limitations of your work.

The project may involve different machine learning settings, including:

- **Supervised Learning**
  - Classification
  - Regression
- **Unsupervised Learning**
  - Clustering
  - Dimensionality Reduction
  - Anomaly Detection
  - Representation Learning
- **Semi-Supervised Learning**
- **Reinforcement Learning**
- Other appropriate machine learning problems with instructor approval

Students who do not already have a research dataset are encouraged to use the **NHTSA Crash Report Sampling System (CRSS)** dataset described below.

If you already have your own research project or research dataset, you may use it for the term project with instructor approval.

The project will be completed through the following components:

- **Project Proposal**
- **Project Progress Report**
- **Project Final Report**

---

## Problem Statement

One of the main goals of this course is to help you learn how to design and evaluate a machine learning system from beginning to end.

You will propose, develop, evaluate, and report a machine learning project in an application or research area that interests you.

Your project should include the major stages appropriate for your machine learning problem, such as:

1. Clearly define the problem.
2. Understand the data, observations, or learning environment.
3. Define the learning objective.
4. Prepare and preprocess the data when appropriate.
5. Identify possible data leakage or other experimental-design issues.
6. Establish a meaningful baseline.
7. Develop one or more machine learning approaches.
8. Design an appropriate validation and evaluation strategy.
9. Compare methods or experimental settings.
10. Analyze the results and limitations.
11. Clearly communicate your methodology and findings.

---

## Objectives

By the end of this project, you should be able to:

- Formulate a real-world problem as a machine learning problem.
- Design and implement a complete machine learning workflow.
- Select machine learning methods appropriate for a particular problem.
- Prepare and analyze data appropriately.
- Design a meaningful experimental evaluation.
- Recognize possible data leakage and other methodological problems.
- Establish appropriate baselines.
- Compare machine learning approaches fairly.
- Analyze model generalization, performance, and limitations.
- Interpret experimental results.
- Clearly explain your methods and findings.
- Develop a reproducible machine learning project.

---

## Project Data

### Recommended Dataset: NHTSA CRSS Crash Data

The recommended dataset for this project is the **National Highway Traffic Safety Administration (NHTSA) Crash Report Sampling System (CRSS)**.

- **Dataset:** [NHTSA Crash Report Sampling System (CRSS)](https://www.nhtsa.gov/crash-data-systems/crash-report-sampling-system)

CRSS contains a nationally representative sample of police-reported motor vehicle crashes in the United States.

The dataset includes information related to:

- crashes,
- vehicles,
- drivers,
- roadway conditions,
- environmental conditions,
- and crash outcomes.

CRSS provides opportunities to work with realistic machine learning challenges such as:

- categorical and numerical features,
- missing values,
- imbalanced outcomes,
- feature selection,
- data leakage,
- model interpretation,
- and generalization.

Possible project questions include:

- Can we predict whether a crash will result in an injury?
- Can we predict crash severity using information available about the roadway, environment, vehicles, and drivers?
- Which factors are most strongly associated with severe crash outcomes?
- How well does a machine learning model trained on earlier years generalize to a later year?
- Can crashes be grouped into meaningful patterns using unsupervised learning?
- Can unusual or high-risk crash patterns be identified using anomaly detection?

These are only examples. You may define a different machine learning problem using the CRSS data.

---

## Using Your Own Research Data

If you already have a research project or another meaningful dataset, you may use your own data instead of the NHTSA CRSS dataset.

This option is encouraged when the term project can contribute to:

- your thesis,
- a research paper,
- a faculty research project,
- an internship or professional project,
- or another ongoing research activity.

Your project does **not** need to be limited to classification or regression.

Examples of acceptable machine learning settings include:

- supervised learning,
- unsupervised learning,
- semi-supervised learning,
- reinforcement learning,
- and other appropriate machine learning settings.

Before using your own dataset, please discuss your proposed project with the instructor.

Your proposal should clearly explain:

- the research or application problem,
- the dataset or learning environment,
- the machine learning setting,
- the learning objective,
- the available data,
- the proposed methods,
- the evaluation strategy,
- and how the project connects to topics in CIS 678.

The project should be sufficiently challenging to support meaningful machine learning development and evaluation.

---

## Machine Learning Problem Formulation

Clearly define the machine learning problem addressed by your project.

Your proposal should answer the following questions:

- What problem are you trying to solve?
- Why is the problem important or interesting?
- What data, observations, or environment are available?
- What information is available to the learning algorithm?
- What should the machine learning system learn?
- What methods do you plan to investigate?
- How will you determine whether the system is successful?
- What baseline will you compare against?

---

## Learning Objective

Clearly describe what the machine learning system is expected to learn.

### Supervised Learning

For a supervised learning project, define:

$$
X \rightarrow Y
$$

where:

- $X$ represents the input features,
- $Y$ represents the prediction target.

Clearly state whether the task is:

- classification,
- regression,
- or another supervised learning problem.

Also describe when the prediction is being made and which information is available at prediction time.

---

### Unsupervised Learning

For an unsupervised learning project, clearly describe what structure or representation you want to discover.

Examples include:

- identifying meaningful clusters,
- discovering latent representations,
- detecting anomalies,
- reducing dimensionality,
- or identifying patterns in unlabeled data.

You should explain what would make the discovered structure meaningful or useful.

---

### Semi-Supervised Learning

For a semi-supervised learning project, describe:

- the labeled portion of the data,
- the unlabeled portion of the data,
- how the unlabeled data will be used,
- and why semi-supervised learning is appropriate.

A useful comparison is often:

$$
\text{Supervised model using labeled data only}
$$

versus

$$
\text{Semi-supervised model using labeled + unlabeled data}.
$$

---

### Reinforcement Learning

For a reinforcement learning project, clearly define:

- the environment,
- the state space,
- the action space,
- the reward,
- the policy,
- and the learning objective.

You should also describe how the learned policy will be evaluated.

---

## Data Leakage

For projects involving prediction, you must carefully examine your features for possible **data leakage**.

A feature should not be used if it directly or indirectly provides information that would not actually be available when the prediction is made.

For example, if you are predicting whether a crash results in an injury, a variable recorded after the injury outcome is known should not be used as an input feature.

Your report should include a short discussion of:

> **Which variables could cause data leakage, which variables were excluded, and why?**

Data leakage may not apply in exactly the same way to every project type. If it is not relevant to your project, explain why.

---

## Experimental Design

Your experimental design should match the type of machine learning problem.

The project should clearly explain:

- how the data are divided or sampled,
- how models are trained,
- how model or method choices are made,
- how hyperparameters are selected,
- how evaluation is performed,
- and how unfair comparison or information leakage is avoided.

---

## Training, Validation, and Test Data

For supervised learning problems, the data should normally be separated into:

- **Training set:** used to fit model parameters.
- **Validation set:** used for model selection and hyperparameter tuning.
- **Test set:** used only for final evaluation.

The test set should **not** be repeatedly used during model development.

Possible splitting strategies include:

- random splits,
- stratified splits,
- group-based splits,
- cross-validation,
- chronological or temporal splits.

The splitting strategy should match the structure of the problem.

For example, if the goal is to predict future outcomes, a chronological split may be more appropriate than a random split.

For unsupervised, semi-supervised, reinforcement learning, or other projects, use an evaluation design appropriate for that learning setting.

---

## Baseline

Every project must include at least one meaningful **baseline**.

A baseline provides a reference point for determining whether the proposed machine learning approach actually improves performance.

Examples include:

### Supervised Learning

- majority-class prediction,
- mean prediction,
- logistic regression,
- linear regression,
- a simple decision tree,
- or another simple model.

### Unsupervised Learning

- random assignment,
- a simple clustering method such as K-means,
- PCA,
- a basic anomaly-detection method,
- or another simple reference method.

### Semi-Supervised Learning

A useful baseline may be:

- a supervised model trained using only the labeled data.

### Reinforcement Learning

Possible baselines include:

- a random policy,
- a simple rule-based policy,
- or another standard policy appropriate for the environment.

The baseline should be appropriate for your specific problem.

---

## Machine Learning Methods

You should investigate machine learning approaches appropriate for your problem.

Possible methods include, but are not limited to:

### Supervised Learning

- Logistic Regression
- Linear Regression
- Naïve Bayes
- Decision Trees
- Random Forest
- Gradient Boosting
- XGBoost
- Support Vector Machines
- Neural Networks

### Unsupervised Learning

- K-means
- Hierarchical Clustering
- DBSCAN
- PCA
- Autoencoders
- Isolation Forest
- Other clustering, representation-learning, or anomaly-detection methods

### Semi-Supervised Learning

- Self-training
- Pseudo-labeling
- Label propagation
- Semi-supervised neural networks
- Other appropriate approaches

### Reinforcement Learning

- Value-based methods
- Policy-based methods
- Q-learning
- Deep Q-learning
- Actor-Critic methods
- Other appropriate reinforcement learning approaches

You do **not** need to use every method covered in class.

Choose methods that are appropriate for your problem and explain why you selected them.

---

## Model Selection and Hyperparameter Tuning

When your project involves model selection or hyperparameter tuning, the choices should be made using appropriate development or validation data.

Do **not** choose the final model based on repeated evaluation of the final test set.

Clearly describe:

- which hyperparameters were tuned,
- how candidate values were selected,
- how models or methods were compared,
- which evaluation criterion was used,
- and how the final approach was selected.

For projects where traditional model selection does not apply, describe the equivalent experimental procedure used to avoid biased evaluation.

---

## Evaluation

The evaluation strategy should match the type of machine learning problem.

### Classification

Possible metrics include:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC
- PR-AUC
- Confusion Matrix

For imbalanced classification problems, accuracy alone is usually not sufficient.

---

### Regression

Possible metrics include:

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- $R^2$

---

### Unsupervised Learning

Possible evaluation methods include:

- silhouette score,
- cluster stability,
- comparison with known labels when appropriate,
- reconstruction error,
- anomaly-detection metrics,
- visualization,
- and domain-based interpretation.

Because unsupervised learning does not always have a single ground-truth answer, you should carefully justify how the quality of the results will be evaluated.

---

### Semi-Supervised Learning

Possible evaluations include:

- comparison with a supervised baseline,
- performance with different amounts of labeled data,
- comparison of supervised and semi-supervised methods,
- and learning curves.

---

### Reinforcement Learning

Possible evaluation criteria include:

- cumulative reward,
- average episode reward,
- success rate,
- learning curves,
- sample efficiency,
- policy stability,
- and comparison with baseline policies.

---

### Other Machine Learning Problems

If your problem does not fit one of the categories above, define an evaluation strategy appropriate for the task.

You must explain why the selected metrics or evaluation methods are appropriate.

---

## Analysis and Interpretation

Your final project should go beyond reporting a single performance number.

Depending on your problem, consider questions such as:

- Why does one method perform better than another?
- Which features or representations are important?
- What types of examples are predicted correctly or incorrectly?
- Are there important failure cases?
- Does the model appear to overfit?
- How sensitive are the results to hyperparameters?
- How stable are the results across different random seeds?
- Does performance vary across important subgroups?
- What patterns were discovered?
- Are the discovered clusters or representations meaningful?
- How stable is the learned reinforcement-learning policy?
- What are the major limitations of the approach?

Appropriate analysis methods may include:

- feature importance,
- model coefficients,
- permutation importance,
- SHAP,
- visualization,
- ablation studies,
- sensitivity analysis,
- error analysis,
- subgroup analysis,
- or other methods appropriate for your project.

---

## Reproducibility

Your project should be reproducible.

You should keep your:

- source code and/or notebooks,
- data-loading instructions,
- package information,
- experiment settings,
- and code used to generate the reported results

organized throughout the semester.

Use fixed random seeds when appropriate.

If your dataset is too large or cannot legally be shared, provide clear instructions explaining how the data can be obtained and prepared.

Additional instructions for project code submission and repository organization will be provided later.

---

## Groups

This is a **team-based project**.

Each team may have up to **4 members**.

All team members are expected to contribute meaningfully to the project.

Possible contributions include:

- problem formulation,
- literature review,
- data preparation,
- model implementation,
- experiments,
- evaluation,
- analysis,
- visualization,
- and report writing.

The final report should briefly describe the contribution of each team member.


---

## Project Schedule

| Period | Task |
| --- | --- |
| Weeks 7–9 | [Project Proposal](./project-proposal.md) |
| Weeks 10–12 | [Project Progress Report](./project-progress-report.md) |
| Weeks 13–15 | [Project Final Report](./project-final-report.md) |

Specific deadlines will be posted on Blackboard.

---

## Grading

The term project counts for **30% of your final course grade**.

The project will be evaluated based on:

- quality of the problem formulation,
- appropriateness of the dataset or environment,
- quality of the experimental design,
- correctness of the machine learning methodology,
- quality of the baseline,
- appropriateness of the selected methods,
- model or method comparison,
- evaluation strategy,
- analysis and interpretation of results,
- reproducibility,
- quality of the final report,
- and clarity of the conclusions.

Different types of machine learning projects may require different evaluation criteria. The goal is not to force every project into the same experimental structure, but every project must demonstrate a rigorous and meaningful machine learning investigation.

---

## Academic Honesty and Use of Existing Code

All components of the project are subject to GVSU and the School of Computing's academic honesty policies.

You may use standard machine learning libraries such as:

- scikit-learn,
- PyTorch,
- TensorFlow,
- XGBoost,
- and other appropriate libraries.

You may also consult documentation, tutorials, papers, and other learning resources.

However, the project must demonstrate your team's own understanding of the complete machine learning workflow.

If you use code, ideas, models, or implementations from external sources, you must clearly cite those sources.

Simply copying an existing:

- Kaggle notebook,
- GitHub repository,
- tutorial,
- course project,
- or published solution

and making minor modifications does **not** constitute an acceptable term project.

You should be able to explain the major decisions in your project, including:

- problem formulation,
- data preparation,
- experimental design,
- algorithm selection,
- hyperparameter choices,
- evaluation strategy,
- and interpretation of the results.

---

## Minimum Expectations

Regardless of the type of machine learning project, every project should include:

1. A clearly defined machine learning problem.
2. A meaningful dataset, environment, or source of observations.
3. At least one appropriate baseline.
4. At least one meaningful machine learning approach beyond the baseline.
5. A well-defined experimental or evaluation protocol.
6. A fair comparison of methods or experimental settings.
7. Analysis and interpretation of the results.
8. Discussion of limitations.
9. Reproducible code.
10. A written final report.

Projects that simply apply an existing algorithm to a dataset without meaningful experimental design, comparison, analysis, or interpretation will not be sufficient.

---

## Getting Help

If you are unsure whether your dataset, research question, or machine learning setting is appropriate, please discuss your idea with the instructor **before submitting the proposal**.

You are encouraged to bring questions about:

- project scope,
- dataset selection,
- problem formulation,
- supervised vs. unsupervised learning,
- semi-supervised learning,
- reinforcement learning,
- feature selection,
- data leakage,
- baseline selection,
- evaluation metrics,
- model selection,
- experimental design,
- and research methodology

to office hours or project meetings.