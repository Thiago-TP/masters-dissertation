# Chapter health

## Overall diagnosis

The methods and results chapters are quite developed, while discussions and conclusion chapters are empty and the introduction and theory framework chapters are mostly finished with some missing/underdeveloped sections. The table below summarizes the effort required to finish each chapter.

| Chapter          | Total estimated time (h) | Average importance (out of 10) |
| ---------------- | -----------------------: | -----------------------------: |
| Abstract         |                     0.25 |                          10.00 |
| Introduction     |                     7.00 |                           8.00 |
| Theory framework |                     5.00 |                           7.60 |
| Methods          |                     0.33 |                           1.00 |
| Results          |                     0.50 |                          10.00 |
| Discussion       |                     1.30 |                          10.00 |
| Conclusion       |                     3.00 |                          10.00 |
| Appendix A       |                     0.00 |                           0.00 |
| Appendix B       |                     0.00 |                           0.00 |
| Appendix C       |                     0.00 |                           0.00 |

**Total time: 17.38 hours**

Proposed strategy: finish theory, methods, results, discussion and conclusion chapters first, and in that order.
This covers just over 10 hours of the estimated 17.
Then, tackle the literature review and research gap outlining in the introduction, in that order.
Then, finish other tasks in the introduction chapter, and finally write the abstract.

In the worst case where there are tasks to do but not enough time, current progress should be stoppped,
remaining issues addressed as best as possible, the abstract written, and the manuscript delivered.
Pending changes should then be addressed during the period between deliverance and presentation.

Other optional tasks include:

- [X] decide on a pattern for headers (whether each word is capitalized or only the first one).
- [ ] fill in the chapter outline and chapter summary sections of each chapter that has them.

## Chapter-by-chapter analysis

### Abstract

While there is a placeholder text, it should be reviewed once all remaining changes are made.

- importance (out of 10): 10
- estimated time required (in hours): 0.25 (15 minutes)

### Chapter 1 - Introduction

#### Diagnosis summary

This chapter is empty, but should be straightforward to write.

This chapter is well organized with most sections done or mostly done,
but the background context is sorely underdeloped.

- Estimated time necessary for corrections/changes: 7 hours
- Average importance in the corrections/changes: 8/10

#### 1.1 Work overview

- what's left to do/change:
  - [ ] include citations at "Kalman-based ensemble method" that will be referenced again in the literature review (they should all be in Emerick's book, chapters 4 and 5)
  - [ ] include citation at "Ensemble Smoother with Multiple Data Assimilation (ES-MDA)"
- importance (out of 10): 5
- estimated time required (in hours): 0.25 (15 minutes)

#### 1.2 Background context

- what's left to do/change:
  - [X] expound contextualization with a paragraph saying models are 3d grids of physical parameters, and list the most important parameters (check Emerick's book, most likely chapter 1)
  - [X] expound contextualization with a paragraph with general description of subsurface simulators, and list commonly used simulators. Also should introduce the concept of reservoir states, listing the most important ones.
  - [ ] expound contextualization with a literature review subsection describing and comparing, in order: KF, EKF, EnKF, ES, ES-MDA, PFA, DSI, DSI-ESMDA. The first five are "history match" methods, and the last "data-space inversion methods". Comparisons should be group-focused. Include a timeline of the cited works.
  - [X] expound contextualization with a scope subsection describing the aims of Gated DSI-ESMDA and where it can be applied.
  - [ ] expound contextualization with a figure comparing data-space and model-space inversion (possibly added in the literature review subsection).
- importance (out of 10): 10
- estimated time required (in hours): 6

#### 1.3 Research problem

- what's left to do/change:
  - [ ] a paragraph highlighting the gap the work fills in each of the aforementioned data-space methods in the literature review subsection.
- importance (out of 10): 10
- estimated time required (in hours): 0.5

#### 1.4 Research questions

- what's left to do/change: the section seems fine.
- importance (out of 10): 0
- estimated time required (in hours): 0

#### 1.5 Significance

- what's left to do/change:
  - [ ] current text is fine, but should be reviewed once the specific gap the work fills is outlined in the research problem section.
- importance (out of 10): 5
- estimated time required (in hours): 0.25 (15 minutes)

#### 1.6 Methodology overview

- what's left to do/change: the section seems fine.
- importance (out of 10): 0
- estimated time required (in hours): 0

#### 1.7 Dissertation outline

- what's left to do/change:
  - [X] current text is fine, but should be reviewed if chapter 2, which originally was the literature review, be dropped
- importance (out of 10): 10
- estimated time required (in hours): 0.05 (5 minutes)

### Chapter 2 - Literature Review

This chapter is planned to become a subsection in the Introduction chapter (under background context section).

### Chapter 3 - Theory Framework

#### Diagnosis summary

This chapter is empty, but should be straightforward to write.

The development of the key contents in this chapter are either advanced or completed,
but supporting/context concepts have not been addressed.

- Estimated time necessary for corrections/changes: 5 hours
- Average importance in the corrections/changes: 7.6/10

#### 3.2 Elements of reservoir engineering

- what's left to do/change:
  - [X] A paragraph at the start of the section stating its contents: general characterization of a reservoir and of subsurface simulation.
  - [X] Reservoir formation subsection: a paragraph or two on how a reservoir is formed and what it can store. Important concepts like facies and faults must be introduced here  (see Emerick's book, then Emanuel's thesis).
  - [X] Subsurface simulation subsection: a paragraph briefly describing the role of wells in reservoir production. The types of well (producer, injector) and their geometry (vertical, horizontal) should be described here (see Emerick's book).
  - [X] Subsurface simulation subsection: a paragraph on what reservoir states are and how they evolve during oil production (see Emerick's book, then Emanuel's thesis). Reservoir control should be briefly mentioned here.
  - [X] Subsurface simulation subsection: a paragraph on the general workings of a subsurface simulator. The main equations employed should be presented here (see Emerick's book, then Emanuel's thesis).
  - [X] Subsurface simulation subsection: a paragraph on the forward model and the prediction forward model. The most important features of this work, i.e., OPR, WPR, WIR, WCTP, FOPT and BHP should be highlighted here (see Emerick's book, and Eclipse's manual).
- importance (out of 10): 10
- estimated time required (in hours): 3

#### 3.3 DSI-ESMDA

- what's left to do/change:
  - [X] subsubsection on a quick review of probability theory (see appendix C of Emerick's book). Definition of probability, Kolmogorov axioms, and Bayes' theorem should be included here, as well as a picture of the classical Vein diagram.
  - [X] review notation: sometimes d appears where d_h should be.
  - [X] review notation: swap k for l in the update equation.
  - [X] finish the derivation of the base update equation (d_map).
  - [X] after presentation of the base equation, comment on the "ensemble smoother" portion of DSI-ESMDA.
  - [X] covariance localization subsection: adapt comentary from Emerick's book (sections 7.1 and 7.3).
- importance (out of 10): 10
- estimated time required (in hours): 2

#### 3.4 Gated DSI-ESMDA

- what's left to do/change:
  - [X] a paragraph commenting on figure 2.6, possibly also absorbing some of the figure's caption text.
- importance (out of 10): 3
- estimated time required (in hours): 0.1 (5 minutes)

### Chapter 4 - Methods

#### Diagnosis summary

This chapter is empty, but should be straightforward to write.

This section is effectively complete, but there might be a table missing.

- Estimated time necessary for corrections/changes: 20 minutes
- Average importance in the corrections/changes: 1/10

#### 4.2 Reservoir case studies

- what's left to do/change:
  - [X] there might be a table of fluid properties missing for the Egg ensemble. Check Emanuel's thesis or the SPE paper.
- importance (out of 10): 1
- estimated time required (in hours): 0.2 (10 minutes)

#### 4.3 Evaluation workflow and parameters

- what's left to do/change:
  - [X] comment on the computational specs used.
  - [X] move the parameters subsection into its own section
  - [X] table which features were used per case study (this could be in the results section instead)
- importance (out of 10): 1
- estimated time required (in hours): 0.2 (10 minutes)

### Chapter 5 - Results

Figures and tables are well curated, but not contextualized.

- Estimated time necessary for corrections/changes: 30 minutes
- Average importance in the corrections/changes: 10/10

#### 5.2 Egg ensemble

- what's left to do/change:
  - [X] paragraph describing what the tables and figures presented are.
  - [X] comment on the trend of results and possible outliers.
- importance (out of 10): 10
- estimated time required (in hours): 0.2 (10 minutes)

#### 5.3 Olympus ensemble

- what's left to do/change:
  - [X] paragraph describing what the tables and figures presented are.
  - [X] comment on the trend of results and possible outliers.
- importance (out of 10): 10
- estimated time required (in hours): 0.2 (10 minutes)

#### 5.4 Brazilian Post-salt Field

- what's left to do/change:
  - [X] move analytical text into the discussion chapter
  - [X] paragraph describing what the tables and figures presented are.
  - [X] comment on the trend of results and possible outliers.
- importance (out of 10): 10
- estimated time required (in hours): 0.2 (10 minutes)

### Chapter 6 - Discussion

#### Diagnosis summary

This chapter is empty, but should be straightforward to write.

- Estimated time necessary for corrections/changes: 1.3 hours
- Average importance in the corrections/changes: 10/10

#### 6.2 Summary of Key Findings

- what's left to do/change:
  - [ ] a paragraph or two summarizing the comments made in the results chapter.
- importance (out of 10): 10
- estimated time required (in hours): 0.2 (10 minutes)

#### 6.3 Interpretation of Findings

- what's left to do/change:
  - [ ] one or two paragraphs per case study analyzing the results on each case (see ECMOR paper)
- importance (out of 10): 10
- estimated time required (in hours): 0.3 (20 minutes)

#### 6.4 Evaluation of Existing Theories and Models

- what's left to do/change:
  - [ ] a paragraph explaining why the proposal performed better/worse than DSI-ESMDA on each case study.
- importance (out of 10): 10
- estimated time required (in hours): 0.3 (20 minutes)

#### 6.5 Limitations and Future Research

- what's left to do/change:
  - [ ] a paragraph commenting the lack of method in localization tuning and lack of spacial element in the real field localization.
  - [ ] a paragraph commenting on future comparisons with EnKF (specially in cases like I3 BHP) and other data assimilation methods.
- importance (out of 10): 10
- estimated time required (in hours): 0.5 (30 minutes)

### Chapter 7 - Conclusion

#### Diagnosis summary

As with the discussion chapter, this chapter is empty, but should be straightforward to write.

- Estimated time necessary for corrections/changes: 3 hours
- Average importance in the corrections/changes: 10/10

#### 7.1 Summary of Findings

- what's left to do/change:
  - [ ] move research questions to closing statement section.
  - [ ] adapt the text in the dicussion chapter summary of key findings section into here.
- importance (out of 10): 10
- estimated time required (in hours): 0.5 (30 minutes)

#### 7.2 Contribution to Knowledge

- what's left to do/change:
  - [ ] a paragraph restating the novelty in the proposal, i.e., a straightforward method for covariance recovery.
- importance (out of 10): 10
- estimated time required (in hours): 0.5 (30 minutes)

#### 7.3 Practical Implications

- what's left to do/change:
  - [ ] a paragraph commenting the ease of implementation of the gating mechanism in both model- and data-space based methods.
- importance (out of 10): 10
- estimated time required (in hours): 0.2 (10 minutes)

#### 7.4 Limitations

- what's left to do/change:
  - [ ] a paragraph commenting the importance of prior representation in cases like I3 BHP
- importance (out of 10): 10
- estimated time required (in hours): 0.5 (30 minutes)

#### 7.5 Future Research

- what's left to do/change:
  - [ ] adapt the text in the dicussion chapter future research section into here.
- importance (out of 10): 10
- estimated time required (in hours): 0.2 (10 minutes)

#### 7.6 Closing Statement

- what's left to do/change:
  - [ ] answers to each research question
- importance (out of 10): 10
- estimated time required (in hours): 1

### Appendix A - Academic Productions

#### Diagnosis summary

This chapter seems fine.

- Estimated time necessary for corrections/changes: 0 hours
- Average importance in the corrections/changes: 0/10

#### A.1 Disciplines Completed

- what's left to do/change: this section seems fine
- importance (out of 10): 0
- estimated time required (in hours): 0

#### A.2 Publications

- what's left to do/change: this section seems fine
- importance (out of 10): 0
- estimated time required (in hours): 0

#### A.3 Software

- what's left to do/change: this section seems fine
- importance (out of 10): 0
- estimated time required (in hours): 0

### Appendix B - Deriving the Innovation Gating Parameter

#### Diagnosis summary

This chapter seems fine.

- Estimated time necessary for corrections/changes: 0 hours
- Average importance in the corrections/changes: 0/10

### Appendix C - Detailed Results

#### Diagnosis summary

This chapter seems fine.

- Estimated time necessary for corrections/changes: 0 hours
- Average importance in the corrections/changes: 0/10

#### C.1 Egg ensemble

- what's left to do/change: this section seems fine
- importance (out of 10): 0
- estimated time required (in hours): 0

#### C.2 Olympus ensemble

- what's left to do/change: this section seems fine
- importance (out of 10): 0
- estimated time required (in hours): 0

#### C.3 Real field

- what's left to do/change: this section seems fine
- importance (out of 10): 0
- estimated time required (in hours): 0
