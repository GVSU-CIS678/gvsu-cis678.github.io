# Project Final Report

The final report should present your completed machine learning project in a clear, rigorous, and professional manner.

Your report should explain:

- the problem you studied,
- why it is important,
- the data or learning environment,
- the machine learning methods you developed or evaluated,
- the experimental design,
- the results,
- what you learned from the results,
- and the limitations of the project.

The final report should go beyond simply listing model performance. It should demonstrate that your team understands the complete machine learning workflow and can analyze and communicate the results appropriately.

Please review the [Term Project Overview](./project-overview.md), your project proposal, and your progress report before preparing the final report.

---

## Format

Please prepare your final report using **Overleaf** and the official **IEEE Conference Template**:

- [IEEE Conference Template on Overleaf](https://www.overleaf.com/latex/templates/ieee-conference-template/grfzhhncsfqn)

If you do not already have an Overleaf account, create a **free Overleaf account** at:

- [Overleaf](https://www.overleaf.com/)

Keep the general IEEE conference formatting, including:

- two-column layout,
- fonts,
- margins,
- section formatting,
- figures and tables,
- citations,
- and references.

Your final report should normally be approximately **6–10 pages, excluding references**.

Subsections are encouraged where appropriate.

---

## 1. Title and Team Members

Include:

- Project title
- Names of all team members as authors

For example:

```latex
\title{Project Title}

\author{
\IEEEauthorblockN{Student A}
\IEEEauthorblockA{
\textit{College of Computing} \\
\textit{Grand Valley State University}\\
Allendale, MI, USA \\
studentA@mail.gvsu.edu
}
\and
\IEEEauthorblockN{Student B}
\IEEEauthorblockA{
\textit{College of Computing} \\
\textit{Grand Valley State University}\\
Allendale, MI, USA \\
studentB@mail.gvsu.edu
}
\and
\IEEEauthorblockN{Student C}
\IEEEauthorblockA{
\textit{College of Computing} \\
\textit{Grand Valley State University}\\
Allendale, MI, USA \\
studentC@mail.gvsu.edu
}
}
```

Use the title and author fields provided by the IEEE template.  
Do not create a separate numbered section for the title and authors in the actual paper.

---

## 2. Abstract

Provide a concise summary of the completed project.

The abstract should briefly describe:

- the problem,
- the data or learning environment,
- the main machine learning methods,
- the evaluation strategy,
- the most important results,
- and the main conclusion.

The abstract should summarize the completed work rather than describe what you originally planned to do.

---

## 3. Introduction

Introduce the application or research problem and provide enough context for readers to understand the project.

The introduction should explain:

- What problem are you addressing?
- Why is the problem important or interesting?
- What is the machine learning setting?
- What is the main objective of the project?
- What approach did you take?
- What are the main findings or contributions of the project?

End the introduction with a clear description of what the project accomplished.

---

## 4. Related Work

Discuss prior research relevant to your project.

Your related work section should:

- describe similar machine learning problems,
- discuss methods that have previously been used,
- explain how your project relates to existing work,
- and identify important differences between your work and previous studies.

Include at least **three relevant academic references**.

Academic sources such as [Google Scholar](https://scholar.google.com/) are recommended.

Use the IEEE citation style consistently.

---

## 5. Data or Learning Environment

Describe the data or environment used in the project.

For a data-based project, include:

- the data source,
- the size of the dataset,
- important variables or features,
- the learning target, if applicable,
- missing-data issues,
- preprocessing,
- feature engineering,
- and any important filtering or data-selection decisions.

If you used the **NHTSA CRSS** dataset, clearly describe:

- which years or subsets were used,
- which variables were selected,
- the target or research question,
- and any variables excluded because of potential data leakage.

For reinforcement learning projects, describe:

- the environment,
- observations or states,
- actions,
- reward function,
- and episode or simulation setup.

Include appropriate tables or figures when they help readers understand the data or environment.

---

## 6. Methods

Describe the machine learning methods used in the project.

The methods section should include:

- the baseline method,
- the main machine learning methods,
- important preprocessing steps,
- feature engineering when applicable,
- model architecture when applicable,
- important hyperparameters,
- and software or libraries used.

Explain the methods in enough detail that another person could understand and reproduce your approach.

You do not need to explain standard machine learning algorithms from first principles, but you should explain how they were used in your project.

For example, rather than explaining what a Random Forest is in general, focus on:

- why you selected it,
- how it was configured,
- and how it was evaluated.

---

## 7. Experimental Design

Describe how the experiments were conducted.

Depending on your project, this may include:

- training, validation, and test splits,
- cross-validation,
- chronological or group-based splitting,
- hyperparameter tuning,
- random seeds,
- model-selection criteria,
- evaluation metrics,
- baseline comparisons,
- and computational environment.

For supervised learning projects, clearly distinguish between:

- training data,
- validation data,
- and final test data.

The final test set should not be used repeatedly for model selection.

Also discuss any methodological concerns such as:

- data leakage,
- class imbalance,
- limited labeled data,
- distribution shift,
- or other issues relevant to your project.

For unsupervised, semi-supervised, reinforcement learning, or other projects, describe an evaluation protocol appropriate for the learning setting.

---

## 8. Experiments, Results, and Discussion

This should be the most important section of the report.

Present the experimental results clearly using appropriate:

- tables,
- figures,
- learning curves,
- confusion matrices,
- visualizations,
- or other summaries.

Report results for:

- the baseline,
- the main machine learning methods,
- and any important experimental variations.

Do more than report numbers. Discuss what the results mean.

Consider questions such as:

- Which method performed best?
- How much improvement was achieved over the baseline?
- Why might one method perform better than another?
- Did the model overfit?
- How sensitive were the results to model choices or hyperparameters?
- Were the results stable across different runs or random seeds?
- What types of examples were difficult for the model?
- What important patterns were discovered?
- Did the results support your original expectations?

Where appropriate, include:

- error analysis,
- feature importance,
- SHAP or other interpretation methods,
- subgroup analysis,
- ablation studies,
- sensitivity analysis,
- cluster interpretation,
- or policy analysis.

Figures and tables should be readable, clearly labeled, and discussed in the text.

---

## 9. Conclusion and Limitations

Summarize the most important findings of the project.

Your conclusion should address:

- What did you learn?
- What were the main results?
- Did the project achieve its original goal?
- What are the major limitations?
- What could be improved?
- What future work would be useful?

Avoid simply repeating numerical results from the previous section.

---

## 10. Data and Software Availability

Describe how the work can be reproduced.

Include:

- the source of the dataset,
- instructions for obtaining the data if it cannot be shared directly,
- important software and libraries,
- and information about how to run your code.

If the data cannot be publicly shared, clearly explain the restriction.

Instructions for final project code submission and repository organization will be provided separately.

---

## 11. Team Member Contributions

Briefly describe the contribution of each team member.

For example:

- problem formulation,
- literature review,
- data preparation,
- model implementation,
- experiments,
- evaluation,
- visualization,
- analysis,
- or report writing.

Each team member is expected to contribute meaningfully to the project.

---

## 12. References

List all references using the **IEEE citation style**.

References should include complete citation information, such as:

- authors,
- title,
- publication venue,
- year,
- and DOI or URL when appropriate.

All academic work, datasets, software, code, and external resources used in the project should be properly cited.

---

## Grading

The final report will be graded out of **100 points**.

| Item | Points |
| --- | ---: |
| Abstract and Introduction | 10 |
| Related Work | 10 |
| Data or Learning Environment | 10 |
| Methods | 15 |
| Experimental Design | 10 |
| Experiments, Results, and Discussion | 30 |
| Conclusion and Limitations | 5 |
| Data/Software Availability and Team Contributions | 5 |
| Writing Quality, IEEE Formatting, Figures/Tables, and References | 5 |
| **Total** | **100** |

### Grading Expectations

- **Abstract and Introduction:** Clearly define the problem, motivation, learning objective, approach, and main findings.
- **Related Work:** Demonstrate an understanding of relevant previous research and appropriately cite academic sources.
- **Data or Learning Environment:** Clearly describe the data, environment, preprocessing, and important design decisions.
- **Methods:** Clearly describe the baseline and machine learning approaches used in the project.
- **Experimental Design:** Use a correct and appropriate evaluation methodology.
- **Experiments, Results, and Discussion:** Present meaningful experiments, clearly communicate results, compare methods, and provide thoughtful analysis.
- **Conclusion and Limitations:** Summarize the findings and discuss important limitations and future work.
- **Data/Software Availability and Team Contributions:** Provide sufficient information for reproducibility and clearly describe each member's contribution.
- **Writing Quality and Formatting:** The report should be clear, professional, well organized, and follow the IEEE conference format with publication-quality figures, tables, citations, and references.

The final report should demonstrate a **complete and rigorous machine learning investigation**, not simply the application of several algorithms to a dataset.

---

## Delivery

Submit the final report as a **PDF file to Blackboard**.

The report must be prepared using the **IEEE Conference Template in Overleaf**.

Only **one submission per team** is required.

Additional instructions for submitting project code and other project materials will be provided separately.

---

## Final Project Presentation and Peer Evaluation

### Presentation

Each team will give a final project presentation during the last part of the semester.

The presentation should highlight:

- the problem,
- the machine learning approach,
- the experimental design,
- the main results,
- important findings,
- and major limitations or challenges.

More details about the presentation format will be provided later.

### Peer Evaluation

Each team member will complete a peer evaluation describing the contributions of the other team members.

Peer evaluation may be used to adjust individual project grades when there are substantial differences in team-member contributions.

---

All components of the term project are subject to GVSU and the School of Computing's academic honesty policies.
```