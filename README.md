# Changelog

- Wed 15/05/2024: Added Final report template in the [Final](Final) folder
- Tue 14/05/2024: **See blackboard announcement for your team ID's and more information about the feedback sessions!**
- Wed 01/05/2024: Fixed typos, added feedback schedule, and added clarification in [Project Proposal description](#3-project-proposal)
- Mon 29/04/2024: Added clarification in [Project Proposal description](#3-project-proposal).
- Fri 26/04/2024: Updated difficulty score description of MERP. More specifically, the case when zero points are awarded.
- Thu 25/04/2024: Updated criteria for maximum bonus point of TIHM. Please read if you are using the TIHM dataset.
- Wed 24/04/2024: Small typos and clarification of the guidelines

# INFOMQNM: The project
All information about the project of INFOMQNM in one repository. 

- [General information](#general-information)
- [Important dates](#important-dates)
- [Main guidelines](#main-guidelines)
- [Questions](#questions)
- [Use of generative AI](#use-of-generative-ai)
- [Phase 1: Project proposal](#phase-1-project-proposal)
    - [1. Choose your dataset and team formation (during first lecture)](#1-choose-your-dataset-and-team-formation-during-first-lecture)
    - [2. Research question](#2-research-question)
    - [3. Project proposal](#3-project-proposal)
    - [4. Project proposal feedback](#4-project-proposal-feedback-and-gono-go)
- [Phase 2: Research and report](#phase-2-research-and-report)
    - [1. Questions](#1-questions)
    - [2. Python notebooks](#2-code-examples)
    - [3. Optional feedback](#3-optional-feedback)
    - [4. Supplementary material](#4-supplementary-material)
    - [5. Final report](#5-final-report)
    - [6. Presentation](#6-presentation)
- [Datasets](#datasets)
    - [Existing datasets](#existing-datasets)
    - [Collecting your own data](#collecting-your-own-data)
- [Grading](#grading)
    - [Criteria](#criteria)
    - [Weights](#weights)
    - [Main guidelines](#main-guidelines-1)

## General information
In the project of INFOMQNM, you are going to perform a quantitative research study on an existing or self-collected dataset. You will work in teams of 2 people. This repository provides you with the templates for the proposal and full report, datasets ready to use, and all information regarding the project.

The project consists of two phases: i) the proposal, and ii) research phase. In the first phase, you and your team will decide on the dataset to use and form a research question. Subsequently, you will present your research idea, describe related work, explain your planned methodology and statistical analyses, and present the schedule in a research proposal. In the second phase, you will use this proposal as a blueprint for the actual research. In case you decided to collect your own data, you conduct your user experiments. In the end, you present the entire research (proposal + results + discussion and conclusion) in a final report and during a 6-minute presentation. 

## Important dates
- Tue. 23/04/2024: Introduction of the project + Team formation + Dataset preferences
- Tue. 30/04/2024 - **Before 11:00**: Email research question and receive approval
- Tue. 14/05/2024 - **Before 11:00**: Hand-in project proposal
- Thu. 16/05/2024: Feedback and Go/No-Go project proposal, check schedule [here](AdditionalInformation/schedules.md)
- Thu. 30/05/2024 - **Before 13:15**: Hand-in a version of the final report if you want me to read it
- Tue. 04/06/2024: Feedback, check schedule [here](AdditionalInformation/schedules.md)
- Thu. 13/06/2024 - **Before 23:00**: Hand-in final report
- Tue. 11/06/2024: Presentations day 1, please email me to reserve a timeslot otherwise you will be assigned a day at random. First come, first serve.
- Thu. 13/06/2024: Presentations day 2, please email me to reserve a timeslot otherwise you will be assigned a day at random. First come, first serve.

## Main guidelines
- Study design should include
    - more than 1 independent variable and
    - either >1 dependent variable or a within subject factor design (both is also fine)
- Check whether assumptions underlying the selected statistical analysis are met. If not, provide a remedy or alternative analysis
- Report on post-hoc analysis or supplementary analysis including an appropiate type of regression analysis or a well-justified alternative

## Questions
We made a lot of changes to this year's project compared to last year. Hence, it could be that we missed some details in our explanation or that some descriptions are not clear. As such, questions and comments during the first and second phases of the project can be sent in by i) raising an issue here on GitHub, ii) by sending me an email, or iii) by tackling me during one of the lab sessions. If I deem your question to be relevant for other teams as well, I will raise an issue about this question myself and/or update this repository. Hence, check the issues page of this repository regularly! 

## Use of generative AI
In this course, the use of generative AI (like ChatGPT, Gemini, and LLama) is allowed when used in the form of a writing coach or brainstorm buddy. Text in the project proposal or final report should not be generated by AI. Keep in mind that I have a trained eye on the use of this technology. If I suspect the use of AI in one of your reports, you'll be invited to discuss this and you have one opportunity to redeem yourself if my suspicion was true. However, if I still suspect the use of AI after this warning, you'll fail the assignment. See more: https://students.uu.nl/en/news/chatgpt-in-the-classroom-what-are-the-current-rules   

**Why?** Generative AI can limit your ability to learn. You learn by making mistakes and tools like ChatGPT and Gemini take away the opportunity to make these mistakes. Of course, there are situations (especially later in life) where errors are less favourable. Fortunately, the university is *the* place where you have the ability to blunder safely and learn accordingly. In this course, for example, you'll get at least two feedback moments before you hand in the final report. Hence, a significant part of your grade will be based on how you handled the feedback I gave you.   

## Phase 1: Project proposal
In the first phase of the project (April 23rd - May 14th), you will form a team, choose a dataset, come up with a research question, and write a project proposal. After submission you'll receive feedback and a Go/No-Go status. Based on this Go/No-Go status, you're allowed to proceed to the research phase or are asked to improve upon several points before you can proceed. 

### 1. Choose your dataset and team formation (during first lecture)
- **It is very important to be present during the first lecture as teams are formed and datasets are assigned during the break.**
- If you cannot make it to the first lecture, please email me in advance but **at least before 11:30** during the first lecture.
- Choose your preferred dataset and form a team with one other person that chose the same dataset.
- Max. 6 teams can work on the same dataset.
- Teams working on the same dataset should have distinct research questions.
- Some datasets are more challenging than others. This is compensated by difficulty points. Please see [Datasets](#datasets) for more information about difficulty points.
- If you choose to collect your own data, please read 'Collecting your own data' in the [Datasets](#datasets) section.
- If you choose to collect your own data, I will ask for more regular updates about your progress to minimize mistakes and time delays in the second project phase.
- **Choose a team name**

### 2. Research question
- Research question should include:
    - more than 1 independent variable and
    - either >1 dependent variable or a within subject factor design (i.e., repeated measures) (both is also fine)
- Come together as a team and brainstorm about research questions. Be creative!
- Examples:
    - Do **eating times** and **sleep quality** affect **heart rate, blood pressure, and weight** when correcting for **age**?
    - Do **genre** and **tempo** affect **valence** and **dancability**? 
    - Do **time of first sunlight** and **the intensity of outdoor activity** affect **smartphone usage** and **mood**? 
    - Do **mood** and **personality traits (neuroticism)** change **the frequency of skin conductance responses** over time?  
- TIP: Try to follow your genuine interest or passion when brainstorming. This will increase your team's motivation tremendously!
- TIP: Make sure that your research question can be supported by literature (i.e., that it makes sense). Otherwise, you'll have a hard time writing the proposal.
- You can send me a main research question with sub-research questions. However, the main questions should adhere to the main guidelines.
- Sent me your research question as soon as possible but at least **before Tue. 30/04/2024 11:00**
- I will reject your research question if it is too similar to the original paper's research question. As such, make sure you have read the paper! You can access them via each dataset's README.md file.
- I will reject your research question if it has too much overlap with a team's research question that was already sent in.
- You will receive approval or rejection within 1 working day.
- TIP: The sooner you sent your research question, the sooner you will receive approval, the sooner you can start writing your project proposal!

### 3. Project proposal
- Study design should include:
    - more than 1 independent variable and
    - either >1 dependent variable or a within subject factor design (i.e., repeated measures) (both is also fine)
- Your research question needs to be answered using one omnibustest (one large statistical test) and (multiple) post-hoc analyses
- Suggest post-hoc analysis or supplementary analysis including an appropriate type of regression analysis or a well-justified alternative 
- Note: You have only 2-2.5 weeks to write!
- A LaTex template is available in [the project proposal folder](Proposal)
- Adhere to the section outline as presented in the template!
- We will send the report back if you fail to adhere to the template or page limit (i.e., max. 6 pages excluding figures, tables, and refs).
- Double check your report when handing it in. It will be send back when obvious errors are still present (e.g., unfinished sentences, copied text, etc.)
- Generative AI is not allowed to write text (see [Use of generative AI](#use-of-generative-ai))
- **Send in your proposal in .PDF format by email before Tue. 14/05/2024 11:00**
- See the project proposal document for more details.

### 4. Project proposal feedback and Go/No-Go
- After handing in the project proposal, you'll receive feedback on **Thu. 16/05/2024 between 13:15 and 18:00**
- Based on the feedback you'll either get a:
    - Go: You can begin working on phase 2 of the project
    - No-Go: Don't worry, you'll have to update the proposal based on the feedback you received before you can proceed :)
- Feedback will be provided during a dedicated 10-minute conversation.
- You'll be assigned a random 10-minute timeslot. To keep things fair, this order will be reversed in the second feedback round. Check schedule [here](AdditionalInformation/schedules.md)
- Prepare your feedback meeting as you only have 10 minutes to ask questions and get feedback (other questions can be sent via email or during the lab sessions)
- I will be very strict on time as the schedule is tight. 10 minutes = 10 minutes
- As there are 26 pairs, the last talks will be between around 18.00.


## Phase 2: Research and report
In the second phase of the project (May 14th - June 13th), you will conduct the quantitative study you have proposed in the first phase and deliver a final report and presentation.

### 1. Questions
- During the second phase, questions regarding the project can be sent in by raising an issue in this repository or by sending me an email.
- Please check [the issues](https://github.com/fastlib/INFOMQNM/issues) before raising an issue or sending me an email. It could be that another team already asked your question.

### 2. Code examples
- Several datasets will have code examples available that demonstrate basic feature extraction techniques.
- You are allowed to use any programming language you like for feature extraction.
- We only offer support for Python, R and SPSS

### 3. Feedback
- Near the end of the second phase, there's a second round of feedback.
- We will talk about progress and your questions.
- Make sure to hand in material you want me to have read, before **Thu. 30/05/2024 13:15**
- Like the first feedback round, feedback will be given during a private 10-minute conversation. Check schedule [here](AdditionalInformation/schedules.md)
- The schedule for the second feedback round will be the reversed schedule of the first round.

### 4. Supplementary material
- In research, it is important that others can check and reproduce your results. Yet many studies can't be reproduced! You should know better!
- In addition to the final report, you are asked to hand in all your data, scripts and notebooks you used to generate the results.
- Add a README.md file or well annotated notebook that explains how to reproduce your results.
- I will do my best to reproduce your results, but if I'm unable to do so, you will get penalized. Instruct me well! Assume I'm one of your parents/little siblings/dog.

### 5. Final report
- A LaTex template is available in the [final report folder](Final)
- Adhere to the section outline as presented in the template!
- We will sent your report back if you fail to adhere to the template or page limit.
- Sent in your **final report in .PDF format** and **your supplementary material as a ZIP file** by email **before Tue. 13/06/2024 23:00**
- See the [final report document](Final) for more details.

### 6. Presentation
- Summerize your research in a short presentation/pitch
- Max. 6 minutes
- Presentations will be a part of your final grade.
- More information about the presentations will be announced [here](AdditionalInformation/presentations.md) in due time.
- Presentations will be divided into two sessions. One on Tuesday and one on Thursday during the regular lecture times. Each session features 13 presentations.
- If you have a preference, email me to reserve your spot in one of the sessions. Otherwise, I will assign you to a random slot.


## Datasets
There are five datasets you can choose. Datasets were chosen to cover a broad spectrum quantitative HCI research domains. However, if you cannot find an appropiate dataset, you can also choose to gather your own data instead. The advantage of collecting your own data is that you circumvent the need for significant preprocessing when using existing datasets. On the other hand, you do have to design your own experimental protocol and run user studies. Due to the limited time frame of the course, it is advised to use one of the existing datasets. Yet, if you are passionate about gathering your own data, we'll support you along the way!

Existing datasets vary in terms of preprocessing and feature extraction difficulty. To incentivize the use of the more difficult datasets and, hence, taking a higher risk, you'll be awarded bonus points based on the dataset's difficulty and the complexity of your processing pipeline. For example, if you intend to use CASE, you can receive a full bonus point if you succesfully preprocess and segment both the joystick and biosignal data and use features from both streams in your statistical analysis. However, when choosing the Spotify Top 50 dataset, no feature extraction is needed and no bonus points can be gained. 

Note: Choosing a more difficult dataset does not automatically gain you the maximal amount of bonus points. Please read the 'For a maximum score' description in each dataset's README.md to get an idea what you need to do to get a maximum bonus score.

### Existing datasets
- [Continuous Annotation Signals of Emotion (CASE)](CASE/README.md): Difficulty score: 1.0
- [K-EmoPhone](K-EmoPhone/README.md): Difficulty score: 1.0
- [MERP: A Music dataset with Emotion Ratings and Raters' Profile information](MERP/README.md) Difficulty score: 0.75 
- [Spotify Top 50](SpotifyTop50/README.md) Difficulty score: 0
- [TIHM: An open dataset for remote healthcare monitoring in dementia](TIHM/README.md) Difficulty score: 0.5

### Collecting your own data
Collecting your own data is also a possibility in the practical assignment. Doing this successfully grants you a 1.0 bonus point. Please read [this](AdditionalInformation/collecting_data.md) for more details.

## Grading
The project will be graded in roughly the same way your master's thesis will be graded. We will assess different aspects of the project as described in the [Weights](#weights) section. In addition to the guidelines and requirements we described throughout this page, we will assess the project on several criteria. 

### Criteria
- Is the contribution new and significant?
- Is overall quality of an acceptable scientific standard?
- Is the general organization/flow acceptable?
- At all moments, is it explained why choices are made? For example, via references, formal proof, empirical proof, or solid reasoning.
- Does the report provide all information (e.g., [Supplementary material](#4-supplementary-material)) to enable full reproduction of the work?
- Do the methods and the treatment of results conform to acceptable scientific standards?
- Are all conclusions firmly based in the data presented?
- Are the references up to date, complete, and in the correct citation style (i.e., [IEEE](https://www.bath.ac.uk/publications/library-guides-to-citing-referencing/attachments/ieee-style-guide.pdf))?

### Weights

1. **Process (20%)**
    - How did you handle the feedback I gave you? 
    - Did you prepare the feedback meetings?
    - Punctuality
    - Correspondence
    - Deadlines
2. **Project proposal (20%)**
    - see [criteria](#criteria)
    - Go/No-Go will be largely based on your methodological section. Hence, receiving a Go will not automatically mean a high Proposal grade. For that, you'll need to score high on the criteria as well.
3. **Final report (30%)**
    - see [criteria](#criteria)
4. **Results and discussion (20%)**
    - Note: We solely assess on presentation, clarity, and discussion. Significance of your results plays no role.
5. **Presentation (10%)**

Furthermore, you can achieve additional bonus points depending on the dataset's difficulty score as explained in section [Datasets](#datasets). You will also automatically gain a full bonus point if you manage to gather your own data successfully. 

Please read all information in this repository carefully. Check all the boxes if you don't want to be surprised by point subtractions in the end. For example, adhere to the templates I give you and do not exceed the maximum number of pages (6 for proposal, 12 for final report). Also, make sure to double check both your proposal and final report before handing it in. We will sent back the report if we notice there are large errors in your document that you could have spotted by checking the document. Please take the effort to hand in a proper report. In turn, we will take the effort of reading and grading it. Make sure your research question(s) and statistical analyses follow the guidelines as said in the template and in section [Main guidelines](#main-guidelines). Also, make sure that I can reproduce all your statistical tests (see [Supplementary Material](#4-supplementary-material)). 

### Main guidelines
- Study design should include
    - more than 1 independent variable and
    - either >1 dependent variable or a within subject factor design (both is also fine)
- Check whether assumptions underlying the selected statistical analysis are met. If not, provide a remedy or alternative analysis
- Report on post-hoc analysis or supplementary analysis including an appropiate type of regression analysis or a well-justified alternative
