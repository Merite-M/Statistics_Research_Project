Research Context: AI vs. Human Grading Analysis
Project: Business Statistics & Probability Final Assessment
1. Research Topic
"A Comparative Statistical Analysis of Student Perceived Fairness: Human vs. Algorithmic (AI) Grading Systems at Kepler College."
2. Research Goals
Analyze student trust in AI grading vs. traditional human grading.
Determine if there is a statistically significant difference in perceived fairness.
Identify correlations between demographic factors (Major, Year) and AI trust.
Provide data-driven recommendations for university grading policy.
3. Research Variables
Independent Variable (IV): Grading Method (Categorical: AI vs. Human).
Dependent Variable (DV): Perceived Fairness Score (Numerical: 1–10 Likert scale).
Population: 

 students (Gender, Program, Year of Study).
4. Hypothesis Statements
Null Hypothesis (
): 

 (No significant difference in perceived fairness).
Alternative Hypothesis (
): 

 (A significant difference exists).
Confidence Level: 95% (

).
5. Technical Rules & Requirements
Library Preference: Use pandas, numpy, scipy.stats, and matplotlib for all visualizations (avoid Seaborn).
Statistical Tests: Use Paired-Sample t-Test (Primary), ANOVA (for major-based comparison), and Pearson’s 
 (for correlation).
Formatting: Final output must be compatible with Times New Roman, 12pt, 1.5 spacing.
6. Data Handling & Ethics
Approval: Research approved by research@keplercollege.ac.rw.
Anonymity: Remove Timestamp columns immediately.
Cleaning: Check for outliers and ensure 

 before running inferential tests.


These are the questions I asked in google forms:

Student Perceptions of AI vs. Human Grading
A research survey exploring student attitudes, fairness perceptions, and concerns regarding traditional human grading compared to automated AI grading systems at Kepler college.
On a scale of 1 to 10, how FAIR do you typically find traditional Human (Teacher) grading?
Not at all fair
1
2
3
4
5
6
7
8
9
10
Perfectly fair
On a scale of 1 to 10, how FAIR do you anticipate Automated (AI) grading to be?
Not at all fair
1
2
3
4
5
6
7
8
9
10
Perfectly fair
On a scale of 1 to 10, how concerned are you about Algorithmic Bias (AI being potentially unfair to certain demographic or academic groups)?
Not concerned
1
2
3
4
5
6
7
8
9
10
Very concerned
Which grading system would you prefer for a high-stakes assessment, such as a final exam?
100% Human Grading (Traditional Teacher/Professor)
100% AI Grading (Fully Automated)
Hybrid/AI Grading with Human Review (AI scores, human validates)
Do you believe AI grading is inherently more objective (less subject to personal bias) than human grading?
Yes, AI is generally more objective
No, human grading is better or AI has new forms of bias
Unsure
Which aspects of a course are you most comfortable having graded by an AI system? (Select all that apply)
Multiple-choice quizzes
Short answer questions (factual recall)
Coding assignments
Essays/Long-form written papers
Presentations/Oral assessments
Other:
What is your gender?
Male
Female
Please specify your current Academic Program/Major (e.g., Business Analytics, Project Management, etc):
What is your current Year of Study?
Year 1
Year 2
Year 3
This is a perfect list of questions. It gives you a mix of Continuous data (the 1-10 scales) for your T-Tests and Categorical data (Gender, Major, Preferences) for your Descriptive stats and ANOVA.
To make this work seamlessly in your Jupyter Notebook with GitHub Copilot, you should add this "Data Schema" to your reference cell. This tells Copilot exactly which columns to look for and how to handle the "Select all that apply" question (which is always the hardest to code).
Updated "Data Schema" for your Notebook
Paste this below your Research Context so Copilot knows your column headers:
8. Data Dictionary (Form Questions)
Human_Fairness: (Scale 1-10) - How fair is teacher grading?
AI_Fairness: (Scale 1-10) - How fair is AI grading?
Bias_Concern: (Scale 1-10) - Concern about algorithmic bias.
System_Preference: (Multiple Choice) - Preferred grading system for finals.
Objectivity_Belief: (Multiple Choice) - Is AI more objective?
AI_Comfort_Areas: (Checkboxes) - Which tasks are okay for AI? (Note: This will require string splitting/one-hot encoding).
Gender: (Male/Female).
Major: (Short Answer).
Year: (Year 1, 2, or 3).
Pro-Tip: Handling the "Select all that apply" Question
Question 6 (AI Comfort Areas) will come out of Google Forms as a single cell with items separated by commas (e.g., "Coding assignments, Multiple-choice quizzes").
Tell Copilot this:
"Copilot, column 'AI_Comfort_Areas' contains comma-separated values. Please write a script to count the frequency of each individual choice so I can plot a Bar Chart of what students trust AI to grade most."
Next Step for your Team:
Since you mentioned Business Analytics and Project Management as examples, you can use an Independent Samples T-Test to compare these two specific majors once you have your 100 responses.


Ah, got it! You're looking for a research topic for a Statistics and Probability assessment and want to tie it back to AI grading bias.
That is a great move—professors love it when you apply class concepts to "hot" real-world problems. Since you need to show off your stats skills, here are three ways to frame an assessment project:
1. The "Null Hypothesis" Approach (Testing for Fairness)
The Goal: Prove whether a grading algorithm is "fair" or "biased" toward a specific group.
The Stats: Use Hypothesis Testing.
Null Hypothesis (
): There is no significant difference between the mean AI-assigned grades of Group A and Group B.
Alternative Hypothesis (
): There is a statistically significant difference.
Test: Use a Two-Sample t-Test or ANOVA (if comparing more than two groups).
2. The "Correlation vs. Causation" Approach (Identifying Proxies)
The Goal: See if the AI is accidentally using "proxy variables" (like word count or zip code) to guess a student's background and grade them accordingly.
The Stats: Use Linear Regression and Correlation Coefficients (
).
Calculate the 
 value to see how much of the grade variance is explained by "neutral" factors (like grammar) versus "biased" factors (like vocabulary complexity associated with high-income schools).
3. The "Error Rate" Approach (Confusion Matrices)
The Goal: Analyze if the AI makes more "False Negatives" (failing someone who should have passed) for one group than another.
The Stats: Use Conditional Probability and Confusion Matrices.
Compare 




 across different demographics.
If the probability of a "False Negative" is significantly higher for one group, you’ve statistically proven algorithmic bias.
Which of these statistical methods have you covered most in class so far? (I can help you outline the specific steps for the one you're most comfortable with!)





you know what I was meaning is that we have an assessment in first statistics and probability for business it's you know it's a final assessment and we have been given some have been given a task to research a research topic and then work on it using all of the concept we have started you know everything that is an Aesthetics and probability you know inferential statistics descriptive statistics whatever and you have started all of that at the test is detest another test whatever and the other stuff in you know I thinkour University have been trying to use AI systems to grade us instead of being a graded by teacher and students have different thoughts about it and I want a hypothesis statement about that because the Hot Topic in our University. you know some prefer being a graded by AI other prefer being degraded by teacher I don't know if that AI is biased or not you know things like that after our University and we have an assessment as you know and I think to be like a huge topic to discuss and I need a research topic of course which is related to that which have a dependent variable and an independent variable. so I plan to use Google phones to you know survey Google phones you know I Google phones phones forms you know I have to research about the students you know you know the students at the data I have the individuals to be tested on you know I need all of those steps and you never have been studying statistics and probability for business and
4 April 2026
That is a brilliant idea for a final project. It’s timely, personal to your campus, and perfectly fits a Business Statistics framework because you can treat "grading" like a "quality control" process in a business.
Since you need to use descriptive and inferential statistics (t-tests, ANOVA, etc.) and a Google Form, here is a solid research structure for you:
Research Topic
"Student Perceptions of Algorithmic Fairness: A Comparative Statistical Analysis of AI vs. Human Grading at [Your University Name]."
1. Variables for your Statistics
To make your math work, you need clear variables:
Independent Variable (IV): Grading Method (AI-based vs. Human-based).
Alternative IV for your survey: Student Demographic (e.g., Year of Study or Major) to see if different groups trust AI differently.
Dependent Variable (DV): Perceived Fairness Score (Measured on a Likert scale of 1–10 in your Google Form).
2. The Hypothesis Statements
Since this is a final assessment, you need a Null (
) and an Alternative (
) hypothesis:

 (Null): There is no significant difference in the mean fairness rating between AI grading and human grading among students. (

)

 (Alternative): There is a significant difference in the mean fairness rating between AI grading and human grading. (

)
3. Your Google Form "Data Collection" Plan
To get the data for your Inferential Statistics, your form should ask:
Demographics: Major, Year (to use for Descriptive Stats like Pie Charts).
The Core Question (Likert Scale): "On a scale of 1–10, how much do you trust the fairness of AI grading?"
The Control Question (Likert Scale): "On a scale of 1–10, how much do you trust the fairness of Human (Teacher) grading?"
4. How to use your Stats Concepts:
Descriptive Statistics: Calculate the Mean, Median, and Standard Deviation of the trust scores. Create Histograms to see the distribution (is it "Normal" or skewed?).
Inferential Statistics (The "Test"): Run a Paired Sample t-Test. Since the same student is rating both AI and Humans, this test will tell you if the difference in their scores is "statistically significant" or just due to chance.
Correlation: See if there is a correlation between "Tech Savviness" (if you ask that) and "Trust in AI."
Does this structure feel manageable for your final, or should we narrow it down to one specific major?





wow I like those hypothesis statements, and I would like to double down (focus) on them
4 April 2026
That’s a great call. Focusing on those specific hypothesis statements gives your project a professional, academic "spine." In a business statistics final, you get the most marks for showing you understand the relationship between your data and these formal claims.
To "double down," let’s refine them into the exact language your professor will look for, and I'll show you how to connect them to your Google Forms data.
1. The Formal Statistical Hypotheses
Since you are comparing two specific means (AI Trust vs. Teacher Trust) from the same group of students, you should use a Paired-Sample T-Test approach.
Null Hypothesis (
): 


(Translation: The mean difference between AI trust scores and Teacher trust scores is zero. Students perceive them as equally fair.)
Alternative Hypothesis (
): 


(Translation: There is a statistically significant difference in perceived fairness between the two methods.)
2. Adding a "Business" Layer (Sub-Hypothesis)
Since this is for a Business stats class, you can add a second test to see if "Risk Appetite" or "Major" changes the opinion.

: There is no correlation between a student’s Year of Study and their Trust in AI grading.

: There is a significant correlation (e.g., Seniors might trust AI less than Freshmen).
3. Setting up your Google Form for these Hypotheses
To test these, your form needs two specific "Scale" questions:
"On a scale of 1-10, how fair do you find traditional Human/Teacher grading?" (This is Variable 
)
"On a scale of 1-10, how fair do you find Automated/AI grading?" (This is Variable 
)
4. What to do with the "You Know" (The Math)
Once you get your responses (aim for at least 30-50 students), you will:
Calculate the Mean (
): Which one has a higher average?
Calculate the Standard Deviation (
): Are student opinions "spread out" (disagreement) or "tight" (everyone agrees)?
Find the P-Value: If your P-value is less than 0.05, you get to Reject the Null Hypothesis and "prove" that your university's students officially feel differently about AI vs. Teachers.
Should we draft the 5-6 exact questions for your Google Form next so you can start collecting data right away?





yes let's do that
4 April 2026
Perfect! To make your Statistics for Business project professional, we need questions that give you "Quantitative Data" (numbers you can run tests on) and "Categorical Data" (groups like Major or Year).
Here are 6 targeted questions for your Google Form:
1. What is your current Year of Study? (Categorical/Ordinal)
Options: Freshman, Sophomore, Junior, Senior, Postgraduate.
Why? This lets you use Descriptive Stats (Pie Charts) and see if older students trust AI more or less.
2. Which Faculty/Major are you in? (Categorical)
Options: Business, Engineering, Arts/Humanities, Science, Other.
Why? In Business stats, we often look for Correlation between "Subject Area" and "Tech Trust."
3. On a scale of 1 to 10, how fair do you believe Human (Teacher) grading is? (Numerical/Interval)
(1 = Very Unfair, 10 = Perfectly Fair)
Why? This is your Control Variable. It’s the "benchmark" for your hypothesis.
4. On a scale of 1 to 10, how fair do you believe AI/Automated grading is? (Numerical/Interval)
(1 = Very Unfair, 10 = Perfectly Fair)
Why? This is your Independent Variable. You will compare this mean to the Human mean in your t-test.
5. What is your biggest concern regarding AI grading? (Categorical)
Options: Lack of nuance/context, Algorithmic bias, Technical errors/glitches, Lack of feedback, I have no concerns.
Why? This gives you a Mode (the most common answer) to discuss in your final report.
6. If you could choose, which system would you prefer for your Final Exams? (Categorical/Binary)
Options: 100% Human, 100% AI, a Hybrid (AI grades, Human checks).
Why? This is a "Business Decision" metric. It shows the Market Preference of the students.
Pro-Tip for your Statistics:
When you get your data into Excel or SPSS, you are going to calculate the Mean (
) for Question #3 and Question #4.
If the Mean for AI is 4.5 and the Mean for Human is 7.2, you have a Mean Difference of 2.7.
Your job in the final paper is to use a Paired t-test to prove that 2.7 didn't just happen by "luck" (sampling error).
Would you like me to show you how to write the "Data Analysis Plan" section for your assignment once you have these responses?





can you formula the research topic again clearly indicating the variables, to give it to my team and teacher for agreeing
4 April 2026
Here is a formal and clear version of the research topic, structured specifically for a Business Statistics and Probability final assessment. You can copy and paste this directly for your team and professor.
Research Project Proposal
Topic:
"A Comparative Statistical Analysis of Student Perceived Fairness: Human vs. Algorithmic (AI) Grading Systems at [Insert University Name]"
1. Research Variables
To ensure we can apply both Descriptive and Inferential Statistics, the study identifies:
Independent Variable (IV): The Grading Method (Categorical: Human-based vs. AI-based).
Dependent Variable (DV): Perceived Fairness Score (Numerical/Interval: Measured on a 1–10 Likert scale).
Grouping/Control Variables: Student Major (Business vs. Non-Business) and Year of Study (Freshman to Senior).
2. Formal Hypothesis Statements
We will test the following to determine if the university should move forward with AI systems:
Null Hypothesis (
): There is no statistically significant difference in the mean fairness scores between human grading and AI grading (

).
Alternative Hypothesis (
): There is a statistically significant difference in the mean fairness scores between human grading and AI grading (

).
3. Statistical Methodology Plan
Our team will use the following concepts from our syllabus:
Descriptive Statistics: We will use Mean, Median, and Standard Deviation to summarize student trust levels and Pie Charts/Histograms to show the distribution of opinions.
Inferential Statistics (The Test): We will perform a Paired-Sample t-Test (at a 95% Confidence Interval) to see if the difference in trust scores is statistically significant (

).
Correlation Analysis: We will use Pearson’s 
 to see if "Year of Study" or "Tech Comfort" correlates with "Trust in AI."
4. Data Collection Tool
Method: Quantitative Survey via Google Forms.
Target Population: Random sample of 

 students from various faculties.
Does this look like a solid plan to present to your teacher, or should we add a section on "Potential Business Impact"?





I have gemini in google forms, Can you give me ready to paste questions so I can paste them there and it makes me ready-to-send form (in the questions to use, remember to add questions that collect data related to the population such as gender, program, year of study)(In addition make sure you have questions that will generate hypothesis data)
7 April 2026
Here is a prompt for use with AI on Google Search to create a Google Form. The prompt includes demographic and hypothesis-generating questions:
Copy and paste the following prompt into the "Help me create a form" box:
Prompt: Create a research survey titled "Student Perceptions of AI vs. Human Grading" with the following 8 questions:
Gender (Multiple Choice: Male, Female, Non-binary, Prefer not to say)
Current Academic Program/Major (Short Answer - e.g., Business, Engineering, Arts)
Year of Study (Multiple Choice: Year 1, Year 2, Year 3, Year 4, Postgraduate)
On a scale of 1 to 10, how FAIR do you find traditional Human (Teacher) grading? (Linear Scale: 1 = Not at all fair, 10 = Perfectly fair)
On a scale of 1 to 10, how FAIR do you find Automated (AI) grading? (Linear Scale: 1 = Not at all fair, 10 = Perfectly fair)
On a scale of 1 to 10, how concerned are you about "Algorithmic Bias" (AI being unfair to certain groups)? (Linear Scale: 1 = Not concerned, 10 = Very concerned)
Which system would you prefer for a high-stakes final exam? (Multiple Choice: 100% Human Grading, 100% AI Grading, Hybrid/AI with Human Review)
Do you believe AI grading is more objective (less biased) than human grading? (Multiple Choice: Yes, No, Unsure)
The first three questions collect population data. Questions 4 and 5 provide numerical data for a paired t-test. Question 6 allows a correlation test. Questions 7 and 8 provide categorical data for Chi-Square tests.
The data can be exported to Excel or Google Sheets.





Did you include the questions you gave me before. Will those questions give enough factors(data), tell me if everything is good
7 April 2026
Yes, I included all the core questions from our previous talk, but I refined them to make sure they work perfectly for a Business Statistics final.
This set of questions gives you more than enough data to hit every requirement of your assessment. Here is why this data is "enough":
1. You have Quantitative Data (for T-Tests & ANOVA)
Questions 4, 5, and 6 use a 1–10 scale. This is "Interval Data."
Why it’s enough: You can calculate the Mean and Standard Deviation. You can run the Paired T-Test to compare the AI mean vs. the Human mean. This is the "meat" of your hypothesis.
2. You have Categorical Data (for Descriptive Stats & Chi-Square)
Gender, Program, and Year of Study are "Nominal/Ordinal Data."
Why it’s enough: You can create Pie Charts and Bar Graphs to describe your population. You can also see if "Business Students" have a different opinion than "Engineering Students" (this is called a Sub-group analysis).
3. You have Correlation Data
Question 6 (Concern about Bias) vs. Question 5 (Trust in AI).
Why it’s enough: You can run a Correlation (
) test. You’ll likely find a "Negative Correlation"—meaning as concern about bias goes up, trust in AI goes down. Professors love seeing this in a final paper.
4. You have "Business Decision" Data
Question 7 (Preference) and Question 8 (Objectivity).
Why it’s enough: This allows you to conclude your paper with a recommendation. For example: "Even though students find AI less 'fair' (p < .05), 60% still prefer a Hybrid model for efficiency."
Is everything ready?
Yes. This setup is "bulletproof" for a university-level stats project. It moves from describing who the students are (Demographics) to what they think (Descriptive) to why it matters (Inferential/Hypothesis testing).
Do you want an explanation of how to interpret the results after the first few student responses are received?





is it better to start with gender, program or year of study or putting them at the end
7 April 2026
In survey design for Business Research, it is almost always better to put demographic questions (Gender, Program, Year of Study) at the end.
Here is why, based on research best practices:
1. The "Hook" Strategy
You want students to engage with the most interesting questions first. If they open the form and immediately see "What is your gender?" and "What is your major?", it feels like a boring administrative task. If they see "How fair is AI grading?", they are more likely to finish the survey.
2. Reducing "Stereotype Threat"
In statistics and psychology, asking for demographics at the start can actually bias the results.
Example: If a student is asked their gender or major first, they might subconsciously answer the "Fairness" questions based on how they think a "Business student" or a "Female student" should answer. Putting them at the end ensures their opinions on AI are pure and unbiased.
3. Survey Fatigue
If a student gets tired halfway through, they are more likely to quit. You want to make sure you've already captured your Primary Hypothesis Data (Questions 4 and 5) before they lose interest.
Recommended Order for your Google Form:
The "Hook": Perceived Fairness of AI vs. Human (The core of your study).
The Details: Concerns about bias and preferences.
The Demographics (The "About You" section): Gender, Program, and Year of Study.
Pro-Tip for your Paper: In your final report, you can actually mention that you put demographics at the end to "minimize response bias and stereotype threat." This will impress your professor because it shows you thought about the quality of your data collection!
Would you like me to help you write a brief Introductory Paragraph for the top of your Google Form to explain the study to your classmates?





Ensure ethical and accurate data handling: Request approval to conduct research from Kepler Community. Send the email to research@keplercollege.ac.rw and copy your instructor(s). (this is also a part of the assessment directions)
7 April 2026
To ensure your project is officially approved, you need to send a professional "Request for Research Approval" email. This is a standard ethical step in Business Research to ensure you aren't violating student privacy.
Here is a ready-to-use template. Make sure to fill in the bracketed information like [Your Name] and [Instructor Name].
Subject: Research Approval Request: Student Perceptions of AI vs. Human Grading
To: research@keplercollege.ac.rw
Cc: [Instructor Email Address]
Dear Kepler Research Committee,
My name is [Your Name], and I am a student in the Statistics and Probability for Business course. As part of my final assessment, my team and I are conducting a study titled: "A Comparative Statistical Analysis of Student Perceived Fairness: Human vs. Algorithmic (AI) Grading Systems at Kepler."
The goal of this research is to apply inferential statistics (Paired-Sample t-Tests and Correlation) to understand how the student body perceives the fairness of AI-based grading compared to traditional methods.
Research Details:
Target Population: Current Kepler students.
Methodology: An anonymous 8-question survey via Google Forms.
Data Handling: All data collected will be strictly anonymous, used only for academic purposes, and stored securely. No personally identifiable information (PII) beyond general demographics (Major, Year, Gender) will be collected.
Variables: The primary dependent variable is a "Fairness Score" measured on a 1–10 Likert scale.
We are requesting your formal approval to distribute this survey to the Kepler community. My instructor, [Instructor Name], is copied on this email for reference.
Thank you for your time and for supporting student research.
Best regards,
[Your Name]
[Your Student ID, if applicable]
Kepler College
A few tips before you hit send:
Wait for the "Yes": Don't send your Google Form link to students until the Research Committee or your instructor gives you the green light.
The "Ethics" Section: In your final paper, you should include a small section titled "Ethical Considerations" where you mention that you sought and received approval from research@keplercollege.ac.rw. This usually earns you extra marks!
Would you like me to help you write the Consent Statement that should go at the very top of your Google Form?





so I have 100 student and would like to use those
17 April 2026
With a sample size of 

, you have hit the "gold standard" for an introductory statistics project! In statistics, once you pass 

, the Central Limit Theorem kicks in, meaning your data distribution will likely be normal enough to run powerful tests.
Since you have 100 students, here is how you should handle that data to get the best grade:
1. Descriptive Statistics (The "Snapshot")
With 100 responses, your charts will look very professional.
Frequency Tables: Show how many students are from each program (e.g., 40 Business, 30 IT, 30 Arts).
Measures of Central Tendency: Calculate the Mean trust score for AI vs. Humans.
Standard Deviation: With 100 people, you can see if opinions are "clustered" (everyone feels the same) or "polarized" (some love AI, some hate it).
2. Inferential Statistics (The "Proof")
This is where the 100 students make your life easy:
Paired-Sample t-Test: You will compare the 100 "Human" scores against the 100 "AI" scores. Because your 
 is large (100), your Standard Error will be low, making it much easier to find a statistically significant p-value (

).
Confidence Intervals: You can state with 95% confidence exactly where the "true" student opinion lies.
3. The "Power" of 100
In your paper, you should mention that your Sample Size (

) provides high Statistical Power. This means your study is strong enough to actually detect a difference in fairness perceptions if one exists. Smaller samples (like 10 or 15) are often dismissed as "anecdotal," but 100 is a legitimate representative sample for a college campus.
4. Group Comparison (Bonus Marks)
With 100 students, you have enough data to do an Independent Samples t-Test or ANOVA between groups. For example:
Does the Business program (

) trust AI more than the Arts program (

)?
Do Year 1 students trust it more than Year 4 students?
Quick Checklist for your Team:
Clean the Data: If you have 100 responses, check for "trolls" (e.g., someone who answered "10" for everything or "1" for everything in 2 seconds).
Coding: In Google Sheets, "Male" becomes 1 and "Female" becomes 2 so you can run the math.
Are you planning to use Google Sheets or a specific software like SPSS or Excel to run your t-test on these 100 students?





I am planning to use Jupiter notebooks you know python in a person
17 April 2026
Using Jupyter Notebooks (Python) is a pro move for a business stats final. It shows your teacher that you can handle "Data Science" workflows, not just basic spreadsheets.
Since you have 100 students, you can use the scipy.stats and pandas libraries to automate all your calculations.
Your "Python Stats Toolkit"
Here is the specific code logic you will need to test your hypotheses:
1. The Paired T-Test (Hypothesis Testing)
This compares the "Human" score column to the "AI" score column for the same 100 students.
python
import pandas as pd
from scipy import stats

# Load your Google Form data (CSV)
df = pd.read_csv('survey_results.csv')

# Run the Paired T-Test
t_stat, p_val = stats.ttest_rel(df['Human_Score'], df['AI_Score'])

print(f"T-statistic: {t_stat}")
print(f"P-value: {p_val}")

if p_val < 0.05:
    print("Reject the Null Hypothesis: Students perceive a significant difference in fairness.")
else:
    print("Fail to Reject the Null: No significant difference found.")
Use code with caution.
2. Visualizing the Distribution
To show the "Business" side of the data, a boxplot is best to see the spread of opinions.
python
import seaborn as sns
import matplotlib.pyplot as plt

# Compare the two distributions visually
sns.boxplot(data=df[['Human_Score', 'AI_Score']])
plt.title('Comparison of Fairness Ratings: Human vs. AI')
plt.ylabel('Score (1-10)')
plt.show()
Use code with caution.
3. Correlation (Bonus Stats)
Check if "Concern about Bias" (Question 6) actually predicts "AI Trust" (Question 5).
python
correlation = df['Bias_Concern'].corr(df['AI_Score'])
print(f"Correlation coefficient (r): {correlation}")
Use code with caution.
Why Python is better for your 

:
Reproducibility: If you get 10 more responses later, you just re-run the cells and the whole report updates.
Data Cleaning: You can easily drop "empty" rows or fix typos in the "Major" column using df.dropna() or df.replace().
Professionalism: You can export your Notebook as a PDF to submit as your technical appendix.
Would you like me to help you write a "Data Cleaning" script to prepare your Google Form CSV for these tests?





So you
17 April 2026
Since you're using Jupyter Notebooks, you're perfectly set up to handle those 100 responses. Python makes it very easy to turn "subjective" opinions into "objective" business insights.
To make sure your project is "A-grade" quality, here is how you should organize your Notebook:
1. Data Preparation (The "Cleaning" Phase)
When you export your Google Form to a CSV, the column names are usually the full questions (e.g., "On a scale of 1-10..."). Your first step in Python should be renaming them for easier coding:
python
import pandas as pd

# Load your data
df = pd.read_csv('your_form_responses.csv')

# Rename columns to short variables for your math
df.columns = ['Timestamp', 'Gender', 'Program', 'Year', 'Human_Score', 'AI_Score', 'Bias_Concern', 'Preference', 'Objectivity']
Use code with caution.
2. Descriptive Statistics (The "Business Overview")
Use .describe() to get a quick summary. This satisfies the "Descriptive Statistics" part of your assessment requirements:
python
# This gives you Mean, Median, Std Dev, Min, and Max for all your 1-10 scores
print(df[['Human_Score', 'AI_Score', 'Bias_Concern']].describe())

# See how many students are in each program
print(df['Program'].value_counts())
Use code with caution.
3. The Hypothesis Test (The "Core")
Since you are comparing two scores from the same student, you must use the Paired T-Test (ttest_rel). This is the most critical part of your final assessment:
python
from scipy.stats import ttest_rel

# Running the test for your Hypothesis
t_stat, p_value = ttest_rel(df['Human_Score'], df['AI_Score'])

print(f"P-Value: {p_value}")
# If p_value < 0.05, you've officially proven a difference in perception!
Use code with caution.
4. Visualizing for the Team/Teacher
A Boxplot or Violin Plot is perfect here. It shows the "spread" of trust—it will visually reveal if students are "scared" of AI or actually prefer it.
Pro-Tip for your "Ethics" section:
Since you're using Python, you can explicitly show your teacher how you protected student privacy by "anonymizing" the data:
Mention that you deleted the Timestamp and Email columns immediately after importing.
How is the team feeling about the Python part? If anyone is nervous about the code, I can give you a full boilerplate script that you can just paste into Jupyter and run.





You know what I wanted it to say is that you have given me an idea you have helped me like create a Google formula the people have filled it and I
17 April 2026
This is the most exciting part! You have gone from an idea to a dataset of 100 individuals, and now you are ready to use Python to "listen" to what that data is telling you about AI at your university.
Since you are using Jupyter Notebooks, here is how you translate those 100 responses into the "A-grade" results for your business statistics final.
1. Descriptive Statistics (The "Snapshot")
In your notebook, your first goal is to describe the 100 students.
Central Tendency: Calculate the average trust score for AI vs. Humans.
Dispersion: Use the Standard Deviation to see if students are divided in their opinions or if they mostly agree.
python
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt

# Assuming your data is loaded into df
print("Average Trust in Human Grading:", df['Human_Score'].mean())
print("Average Trust in AI Grading:", df['AI_Score'].mean())

# Visualize the comparison
df[['Human_Score', 'AI_Score']].plot(kind='box', title='Distribution of Trust Scores')
plt.show()
Use code with caution.
2. Inferential Statistics (Testing the Hypothesis)
This is where you answer your Hypothesis Statement. You will use a Paired-Sample t-Test because each of your 100 students gave two related scores (one for AI, one for Human).
Goal: Find the p-value.
Rule: If 

, you Reject the Null Hypothesis. You can officially tell your teacher: "There is a statistically significant difference in how students perceive AI vs. Human fairness."
python
from scipy.stats import ttest_rel

t_stat, p_val = ttest_rel(df['Human_Score'], df['AI_Score'])
print(f"Statistically Significant? {'Yes' if p_val < 0.05 else 'No'} (p = {p_val:.4f})")
Use code with caution.
3. Business Analysis (Correlation)
In business, we care about why. You can check if "Concern about Bias" is what's driving the low AI scores.
Pearson Correlation (
): Check the relationship between Bias_Concern and AI_Score. If 
 is close to 
, it means that as bias fear goes up, AI trust goes down.
4. Categorical Insights (ANOVA)
Do Business students trust AI more than Arts students?
Since you have 

, you can group your data by Program and run an f-test (ANOVA) to see if the major affects the opinion.
Would you like me to help you write the "Interpretation" section? This is where you explain in plain English what the Python results mean for your university's grading policy.





Work.pdf
In addition, please remember the required text formatting and structure for your report:Font type: Times New RomanFont size: 12Line spacing: 1.5Include a Cover Page (with title, group members, course, instructor, and date)Include a Table of Contents (clearly showing all sections and page numbers)Make sure your report is clearly structured and professionally presented according to these formatting guidelines.These are a small part of the rules that we will have to follow
12:23
Something went wrong and an AI response wasn't generated.
Work.pdf
I am planning to make a gem in gemini that I will be using to writing the whole report and now gems also appear in google sheets gemini which I also want to harness, you can tell me how to harness it well and craft its name, description, and instructions. I have also attached a template. In addition, please remember the required text formatting and structure for your report:Font type: Times New RomanFont size: 12Line spacing: 1.5Include a Cover Page (with title, group members, course, instructor, and date)Include a Table of Contents (clearly showing all sections and page numbers)Make sure your report is clearly structured and professionally presented according to these formatting guidelines.These are a small part of the rules that we will have to follow perhaps these information can help you know what to also include in our report that are not a part of that template
12:38
Something went wrong and an AI response wasn't generated.
come give that instructions for the gemini gems
12:39
To set up your custom Gem effectively, you need to provide it with a "persona" that understands both the rigorous statistics required for a business course and the specific formatting required by Kepler College.
Here is the setup for your Gem. You can copy and paste these directly into the Gem creation window.
Gem Name:
Kepler Business Stats Research Assistant
Gem Description:
An expert in Business Statistics, Python (Jupyter), and academic reporting. Designed to help Kepler College students transform survey data into professional, research-based reports following specific formatting and ethical guidelines.
Instructions for the Gem:
(Role & Persona)
You are the Kepler Business Stats Research Assistant. You are an expert data scientist and academic writer specializing in Business Statistics. Your goal is to help me write a 15-20 page research report on "Student Perceptions of AI vs. Human Grading" using my 

 survey dataset.
(Core Task: Structure & Content)
You must strictly follow the Kepler Research Template provided in the attached PDF. You will help me write each of the 7 sections:
Introduction: Formulate the problem statement, research objective, 
, and 
.
Methodology: Describe our variables (Independent: Grading Method; Dependent: Fairness Score), the 

 population, and ethical approval (research@keplercollege.ac.rw).
Data Processing: Provide Python code for cleaning raw Google Forms data, handling missing values, and anonymizing data.
Data Analysis: Generate and explain Descriptive Statistics (mean, std dev) and Inferential Statistics (Paired T-Tests, p-values).
Interpretation: Discuss trends and identify study limitations.
Conclusion: Provide data-driven recommendations for the Kepler community.
Appendices: Format the raw data, survey questions, and ethics approval for inclusion.
(Core Task: Statistical Rigor)
Always check for Normal Distribution before suggesting a t-test.
Always use a 95% Confidence Interval (

).
When I provide Python output from my Jupyter Notebook, explain the results in professional academic language.
(Formatting Rules)
Every draft you generate must be ready to be pasted into a document with these settings:
Font: Times New Roman, Size 12.
Spacing: 1.5 Line Spacing.
Structure: Must include a professional Cover Page and a detailed Table of Contents.
(Google Sheets Integration)
When I use you inside Google Sheets:
Help me write formulas to clean data (e.g., =IFERROR, =VLOOKUP).
Summarize my columns to check for data quality before I export to CSV for Jupyter.
Generate "Data Summaries" that I can turn into Bar Charts or Pie Charts.
Using the Gem in Google Sheets:
The Gemini family of models is available in the Google Sheets side panel. It can help you prepare data before using Python:
Data Cleaning: Request a formula to group specific responses. For example, "Look at my 'Program' column. Give me a formula to group all 'Business Administration' and 'Business Management' responses into one category named 'Business'."
Data Quality Check: Ask questions about data. For example, "I have 100 responses. Based on my 'AI_Score' column, does it look like I have any outliers or trolls that I should delete before running my t-test in Python?"
Drafting Descriptions: Request a summary of the data. For example, "Write a 1-paragraph Descriptive Statistics summary of this trust-score data that I can use for Section 4 of my report."





As I am going to use jupyter notebook inside vs code with github copilot. I want it to help me end-to-end with all the work in jupyter notebook.
Using GitHub Copilot within VS Code for your Jupyter Notebook project will turn your 100-student dataset into a professional academic report with high efficiency. Copilot serves as an "AI pair programmer" that can generate code for analysis, write markdown text for your report, and troubleshoot errors in real-time. 
YouTube
YouTube
 +4
End-to-End Workflow with GitHub Copilot
Project Scaffolding:
Open VS Code, install the GitHub Copilot and Jupyter extensions.
Use the Copilot Chat pane or the /newNotebook command to generate an initial structure based on your research topic.
Data Exploration & Cleaning:
Place your responses.csv in your workspace.
Use the @workspace or @data command in Copilot Chat to ask, "Clean this dataset and rename columns for my AI vs. Human grading study".
Statistical Analysis:
Type a comment like # Run a paired t-test comparing AI_Score and Human_Score and let Copilot suggest the scipy.stats code.
Ask Copilot to /explain the resulting p-value to ensure it aligns with your 
 and 
.
Visualizations:
Request specific plots: "Generate a Seaborn boxplot comparing perceived fairness of AI vs. teachers".
Copilot can automatically suggest titles, labels, and color palettes that fit a professional business report.
Drafting the Report:
Switch to Markdown cells for the text sections. Use Copilot to "ghost write" paragraphs for your Introduction or Interpretation.
Provide context by adding files like your project template to the chat using the "Add context" button so Copilot follows your specific structure. 
YouTube
YouTube
 +11
Best Prompts for your Business Stats Project
Task 	Prompt for Copilot Chat
Data Summary	"Show descriptive statistics for all 1-10 scale variables in my dataframe."
Hypothesis Test	"Write a script to perform a paired t-test for my fairness scores and check for normality using the Shapiro-Wilk test."
Formatting	"Help me write a professional Conclusion for this report based on the t-test results I just calculated."
Cleaning	"Identify and remove any outlier responses from the 100-student sample that might bias the mean."
Harnessing "Autopilot" for the Final Draft
In the latest 2026 releases, you can use Autopilot (autonomous agent sessions) to have Copilot implement multiple cells of analysis at once. This is particularly useful for building the entire "Data Analysis" section of your report in one go by simply providing your research goals and the CSV file. 
