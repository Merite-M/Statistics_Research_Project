# Full Marks Report Guide

This guide shows how to turn the notebook analysis into a strong written report for the Statistics and Probability for Business final assessment.

It is written for this project specifically:

- Topic: student perceptions of AI grading vs human grading
- Scope: Year 2 students cohort 2025 only
- Main test: paired t-test for human fairness vs AI fairness
- Second test: chi-square test for academic program vs preferred grading system
- Sample size after cleaning: 91 responses

## 0. Context used to build this guide

This guide is based on the full project context, not only the notebook. The main files and what they contributed are:

- Assessment brief: report length, required sections, appendix expectations, and slide presentation requirement.
- Work template: section-by-section page guidance and the reminder to discuss mean, standard deviation, charts, significance level, and recommendations.
- Chrome research context: the original research topic, survey design, hypothesis language, ethics note, and the survey questions that generate the variables.
- Research notebook: the actual cleaned columns, the final sample size, the charts, and the final test outputs used in the report.

If a detail from any of those files is important for the report, it should appear somewhere in the final write-up.

## 1. What the marker is looking for

To score highly, the report must do more than show results. It must:

- define a clear problem
- explain why the problem matters to the Kepler community
- show that the data was cleaned carefully
- use the right statistical tests
- explain what the numbers mean in plain language
- connect the findings back to the research objective
- make realistic recommendations
- look polished, well structured, and easy to follow

The strongest reports usually have four qualities:

1. Clear logic from problem to conclusion.
2. Correct statistical method choice.
3. Good interpretation, not just copied output.
4. Professional writing and presentation.

## 2. Recommended structure and page plan

For this project, the best target is **about 12 to 14 pages for the main report body**. If you include a title page, references, and appendices, the **full document can reach about 15 to 18 pages**.

That is a better target than guessing 20 pages, because it matches the rubric and the amount of analysis you actually have.

A good balance is below.

- Introduction: 1 to 1.5 pages
- Methodology: 2.5 to 3 pages
- Data Processing: 0.5 to 1 page
- Data Analysis: 3 to 4 pages
- Interpretation and Discussion: 2.5 to 3 pages
- Conclusion and Recommendations: 1.5 to 2 pages
- Appendices: not counted heavily in the word limit

If you want full marks, do not make the report too short. Short reports usually miss explanation and discussion. At the same time, do not add filler just to increase page count.

## 3. Title suggestion

Use a title that is specific and academic.

Example:

**Student Perceptions of AI Grading and Human Grading Among Year 2 Students at Kepler College**

## 4. Introduction: what to write

This section should explain the problem and why it matters.

Include these points:

- AI grading is becoming more common.
- Students may not fully trust AI grading.
- Fairness is important in assessment because it affects confidence, motivation, and acceptance of results.
- This study focuses on Year 2 students cohort 2025
- The study compares perceptions of human grading and AI grading.
- The study also checks whether preferred grading system differs by academic program.

You should clearly state the research objective.

Good objective example:

> The objective of this study is to determine whether Year 2 students rate human grading as fairer than AI grading and whether preferred grading system is associated with academic program.

State the hypotheses clearly.

For the paired t-test:

- H0: There is no difference between the mean fairness rating of human grading and AI grading.
- H1: There is a difference between the mean fairness rating of human grading and AI grading.

For the chi-square test:

- H0: Academic program and preferred grading system are independent.
- H1: Academic program and preferred grading system are associated.

The broader brainstorming in the research context also mentioned correlation and ANOVA. In the final report, only include those if they are still in the notebook and in the final analysis plan. If you have simplified the notebook to two tests, do not force extra tests into the report.

Keep the introduction focused on the challenge, the objective, and the hypotheses. Do not put detailed results here.

## 5. Methodology: what to write

This section should explain exactly how the study was designed.

### 5.1 Variables

Describe the main variables and classify them.

Use this wording style:

- Human_Fairness: quantitative, ordinal rating scale from 1 to 10
- AI_Fairness: quantitative, ordinal rating scale from 1 to 10
- AI_Bias_Concern: quantitative, ordinal rating scale from 1 to 10
- System_Preference: qualitative categorical variable
- Academic_Program: qualitative categorical variable
- Year_of_Study: qualitative categorical variable

Explain why these variables matter.

For example:

- Human_Fairness and AI_Fairness directly measure the main research question.
- System_Preference shows the grading approach students prefer.
- Academic_Program allows a comparison between groups of students.

### 5.2 Population and sample

State the population and sample clearly.

Example:

> The target population was Kepler students who responded to the survey. After cleaning, the final sample used for analysis contained 91 Year 2 responses.

If you do not know the full population size, say so honestly. Do not invent it.

### 5.3 Sampling approach

Explain the sample selection method as it fits the project.

You can write that the study used survey responses from available participants, which is a form of non-probability convenience sampling unless your team used a different method.

### 5.4 Data collection method

State that this was primary data collected through a survey.

Mention that the questionnaire captured fairness perceptions, bias concern, grading preferences, program, and year of study.

For completeness, mention the actual question groups from the Google Form:

- Human_Fairness
- AI_Fairness
- AI_Bias_Concern
- System_Preference
- AI_Objectivity_Belief
- Comfortable_AI_Grading_Aspects
- Gender
- Academic_Program
- Year_of_Study

These are important because they give you both the main hypothesis variables and the demographic variables needed for description and comparison.

### 5.5 Ethics

Include a short ethics paragraph.

Mention:

- permission was requested before data collection 
- responses were used for academic purposes only
- participant identity was protected
- data was reported in summary form

This section should sound careful and responsible.

## 6. Data Processing: what to write

This section should show that you handled the data properly.

Write about the raw data issues you found:

- timestamp column not needed for analysis
- duplicate responses
- missing values in Academic_Program and AI_Objectivity_Belief
- inconsistent formatting in Academic_Program labels

Then explain how you fixed them:

- removed the timestamp column
- removed duplicate rows
- standardized Academic_Program text using consistent capitalization
- filled missing Academic_Program values with the mode
- kept the raw and clean data separate for transparency

Do not just list actions. Explain why they mattered.

Example:

> Standardizing the academic program labels was necessary because the same category appeared in slightly different forms. Without this step, the summary counts would be misleading.

Also mention that the final cleaned analysis used a Year 2-only sample, which is why the working sample size became 91 responses.

## 7. Data Analysis: how to write it well

This is one of the most important sections.

### 7.1 Start with descriptive statistics

Include the mean and spread for the main rating variables.

For this project, report:

- Human_Fairness
- AI_Fairness
- AI_Bias_Concern

Use the numbers from the notebook.

You can say:

> Human grading received a higher average fairness score than AI grading, suggesting that students viewed human grading more positively.

### 7.2 Include charts

You should discuss the charts, not only paste them.

Recommended charts:

- boxplot comparing Human_Fairness and AI_Fairness
- bar chart for System_Preference
- bar chart for AI comfort areas

For each chart, explain what the reader should notice.

Example:

> The boxplot shows that the human fairness ratings are generally higher than the AI fairness ratings, although there is some overlap between the two distributions.

### 7.3 Explain the paired t-test

This is the main test for the first hypothesis.

Write the test purpose in plain language:

> A paired t-test was used because the same students rated both human and AI grading.

Report the results clearly:

- t = 2.615
- p = 0.010461
- decision: reject H0 at 0.05

Do not stop at the numbers. Explain them.

Example:

> Since the p-value is below 0.05, the difference is statistically significant. This means Year 2 students rated human grading as significantly fairer than AI grading.

If you include the confidence interval, explain it briefly.

### 7.4 Explain the chi-square test

This is the second test and should be described simply.

Write why it was used:

> A chi-square test of independence was used to check whether preferred grading system is related to academic program.

Report the result:

- chi2 = 0.1883
- p = 0.910136
- decision: fail to reject H0

Interpret it:

> The result shows no evidence that preferred grading system differs by academic program in this sample.

### 7.5 Keep the analysis section balanced

Do not spend too long repeating output values.

The best structure is:

- 1 short paragraph for descriptive statistics
- 1 short paragraph for charts
- 1 paragraph for paired t-test
- 1 paragraph for chi-square test
- 1 short paragraph summarizing the main statistical message

If you want to show full use of the project context, you can briefly mention the AI comfort areas chart and the AI objectivity belief question as descriptive findings, but keep them out of the inferential focus unless they are directly tested.

## 8. Interpretation and discussion: what to write

This section should answer the question: so what?

Discuss these points:

- why students may trust human grading more than AI grading
- what this means for grading systems at Kepler
- whether the result matches the research objective
- whether academic program seems to matter for grading preference

You can also mention that the chi-square result suggests program type does not explain grading preference in this sample.

You may also note that the survey responses suggest mixed feelings about AI objectivity, which supports the broader discussion about trust and bias even if it is not a formal hypothesis test in the final version.

### Limitations to mention

Include at least 2 or 3 honest limitations:

- the sample is limited to Year 2 students
- the study is based on survey responses, so it depends on perception
- the sample size is modest
- the results may not generalize to all students

Do not make limitations sound like excuses. Make them sound thoughtful and professional.

## 9. Conclusion and recommendations

This section should be direct and practical.

### Conclusion

Summarize the main findings in one short paragraph:

- human grading was rated significantly fairer than AI grading
- preferred grading system was not significantly associated with academic program
- the main hypothesis was supported by the paired t-test

### Recommendations

Give realistic actions based on the findings.

Good recommendations:

- if AI grading is used, keep human review in the process
- explain grading criteria clearly to students
- provide communication about how AI-based grading works
- do more student feedback studies before wider AI adoption

The recommendations should connect directly to the results.

## 10. Appendices

Include supporting material here:

- raw data file
- cleaned data file if available
- survey or response form
- approval email
- relevant notebook screenshots or summary tables

If your instructor wants evidence, appendices are where it belongs.

For this project, the appendices should ideally include:

- raw survey responses export
- cleaned Excel or CSV version of the data
- screenshot or copy of the Google Form questions
- research approval email to research@keplercollege.ac.rw with the instructor copied
- any response summaries or charts you want to preserve

## 11. Slide presentation requirement

The assessment brief also asks for a slide presentation of about 7 to 10 slides. Keep it short and direct.

Recommended slide flow:

- Slide 1: Title and team members
- Slide 2: Research problem and objective
- Slide 3: Hypotheses and variables
- Slide 4: Data collection and sample
- Slide 5: Cleaning and descriptive statistics
- Slide 6: Paired t-test results
- Slide 7: Chi-square result
- Slide 8: Interpretation and limitations
- Slide 9: Recommendations
- Slide 10: Conclusion and thank you

If you only have 7 to 8 slides, combine closely related sections.

## 12. How to make it look like a full-mark report

Presentation matters.

Use these formatting rules:

- Times New Roman, 12 pt
- 1.5 line spacing
- consistent headings
- numbered sections
- aligned tables and figures
- figure captions
- page numbers if possible

Also use strong academic writing:

- avoid casual wording
- avoid repeating the same sentence structure
- explain each result in plain language
- use the first-person plural only if your class style allows it

## 13. A strong writing formula for each section

Use this pattern repeatedly:

1. State the point.
2. Show the number or evidence.
3. Explain what it means.
4. Connect it to the research objective.

Example:

> Human fairness scores were higher than AI fairness scores. The paired t-test showed a significant difference, with p = 0.010461. This suggests that Year 2 students currently view human grading as fairer, which directly supports the main research objective.

## 14. Common mistakes to avoid

- writing too little in the discussion section
- listing results without interpretation
- using the wrong statistical test
- forgetting to explain why a test was chosen
- ignoring data cleaning issues
- mixing up hypotheses and conclusions
- making recommendations that do not follow from the results
- leaving out appendices or evidence

## 15. Submission checklist

Before submitting, confirm that your report has:

- a clear title
- introduction with objective and hypotheses
- methodology with variables, sample, and ethics
- data processing with cleaning steps
- descriptive statistics and charts
- paired t-test result
- chi-square result
- interpretation and limitations
- recommendations
- appendices
- slide presentation ready
- correct formatting and page count

## 16. Final short version of the story

If you need one sentence to keep the whole report focused, use this idea:

> Year 2 students rated human grading as significantly fairer than AI grading, while academic program did not show a significant relationship with preferred grading system.

That sentence can guide your whole report.
