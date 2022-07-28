# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 1: Standardized Test Analysis

### Project Objectives:

Identify the states in the United States that has the most potential to increase the SAT participation rate and make recommendations to the College Board on where the efforts should be focused on. Give some recommendations on what could be done.

---

### Data used:

The aggregate SAT and ACT scores and participation rates by states from 2017 to 2019.

---

### Data Dictionary:

Three main datasets were used in this project. The data dictionaries of the datasets can be found below.

<br>**Dataset name: `act_2017_to_2019`**
<br>This dataset contains the aggregate ACT scores and participation rates by states from 2017 to 2019.

| Feature | Type | Dataset | Description |
|:--|:-:|:-:|:--|
|state|string|act_2017_to_2019|States found in the United States.|
|participation_act|float|act_2017_to_2019|Percentage of the population taking ACT. Percentage is shown in decimal form.|
|total_ACT|float|act_2017_to_2019|Overall score obtained by summing the scores of all the ACT sections.|
|year|int|act_2017_to_2019|The year the data pertains to.|

<br>**Dataset name: `sat_2017_to_2019`**
<br>This dataset contains the aggregate SAT scores and participation rates by states from 2017 to 2019.

| Feature | Type | Dataset | Description |
|:--|:-:|:-:|:--|
|state|string|sat_2017_to_2019|States found in the United States.|
|participation_sat|float|sat_2017_to_2019|Percentage of the population taking SAT. Percentage is shown in decimal form.|
|ebrw_sat|int|sat_2017_to_2019|Score for the Evidence-Based Reading and Writing section.|
|math_sat|int|sat_2017_to_2019|Score for the Math section.|
|total_sat|int|sat_2017_to_2019|Overall score obtained by summing the scores of all the SAT sections.|
|year|int|sat_2017_to_2019|The year the data pertains to.|

<br>**Dataset name: `combined`**
<br>This dataset contains the aggregate ACT and SAT scores and participation rates by states from 2017 to 2019.
| Feature | Type | Dataset | Description |
|:--|:-:|:-:|:--|
|state|string|combined|States found in the United States.|
|participation_act|float|combined|Percentage of the population taking ACT. Percentage is shown in decimal form.|
|total_ACT|float|combined|Overall score obtained by summing the scores of all the ACT sections.|
|year|int|combined|The year the data pertains to.|
|state|string|combined|States found in the United States.|
|participation_sat|float|combined|Percentage of the population taking SAT. Percentage is shown in decimal form.|
|ebrw_sat|int|combined|Score for the Evidence-Based Reading and Writing section.|
|math_sat|int|combined|Score for the Math section.|
|total_sat|int|combined|Overall score obtained by summing the scores of all the SAT sections.|
|year|int|combined|The year the data pertains to.|

---

### Key takeaways from the analysis:
1. SAT and ACT participation rates are inversely related to each other. Most students would choose either SAT or ACT. However, there are students who take both SAT and ACT. This is because they can use the higher of the tests in their college/ university applications.

2. Both ACT and SAT total scores are inversely related to their participation rates because if given a choice, students are more likely to take the test that best fits them.

---

### Recommendations:
1. Based on the fact that Oklahoma has an increasing participation rate despite the lower mean scores and mandatory ACT test, more efforts should be spent in Oklahoma.

2. To further encourage the participation rate in SAT, free/subsidised tuition/preparation classes should be introduced. Since students are more inclined to take the tests they are confident in, having these classes would definitely increase the participation rates.
