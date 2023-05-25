# InterviewAnalysis
## 🛈 Background Information
Lebron James is unquestionably one of the greatest basketball players to ever live. He entered stardom during his high basketball career when he was deemed, 'The Chosen One'. Then drafted directly out of high school by his hometown team, the Cleveland Cavaliers, the storybook was written for him. Despite unfathomable expectations, James has exceeded them all; in 2023, he became the NBA all-time leading scorer. Categorized as a 'team first' player, Lebron has always been known to make the correct basketball decision. This unselfish behavior is also reflected in his off-court behavior and sentiment in interviews. Lebron James is a class act of a player and human. 

The best interviews occur when the spotlight is brightest and Lebron has been in many of these moments. He has been voted to the NBA All-Star team for 19 consecutive seasons, only missing out on the team his rookie year. James has competed in the NBA Finals 10 times. He has an overall record of 22 wins and 33 losses, resulting in four championship titles. 

## 🎯 Aim
We aim to perform various forms of sentiment analysis on interviews with Lebron James. 

First, we aim to identify themes in James' ASG interviews. The All-Star game is a unique experience which should consist of varying topics and trends of the year. 

Next, we will conduct sentiment analysis of Lebron's tone from interviews during the NBA Finals. These are the big moments; this is where remaining poised and leading the team is most impactful! 

Finally, we test and optimize various ML models for binary classification where we predict Lebron's tone on a test set of data. How well can our models predict tone with limitations to factors and a small sample size? 

## :robot: ChatGPT
Prompt testing was initially performed on openai's website. We found most consistent results when submitting batches of size 5. After a consistent return from our prompt, we integrated ChatGPT into Python and identified the tone of over 2,000 questions and responses. 

Prompt: "Let 1 = positive, 0 = neutral, and -1 = negative. Identify the tone of the 5 questions using the given values. Output the list of values in order of the questions." 

(note: we used loops to change the prompt based on the number of questions submitted, originally an f-string was used to always determine the number of questions-however, this resulted in higher token usage.)

## :mag_right: Interview Source
http://www.asapsports.com/show_player.php?id=13888

## 📁 Datasets
**Raw data**

[Question tones](https://github.com/BryceDecker/InterviewAnalysis/blob/main/Data_sets/Question_tones.csv), [Response tones](https://github.com/BryceDecker/InterviewAnalysis/blob/main/Data_sets/Response_tones.csv), and [Tone ratings](https://github.com/BryceDecker/InterviewAnalysis/blob/main/Data_sets/raw/Interview_Tone_Rating.csv)

**Clean data**

[Interview data](https://github.com/BryceDecker/InterviewAnalysis/blob/main/Data_sets/clean/Interview_analysis_final.csv)

## 📊 Data Visualization
**Word Cloud**

<img src="Data_visuals/Bball_wordcloud.png" width="30%"> 

**Linear Regression**

<img src="Data_visuals/RR_distribution.png" width="30%"> <img src="Data_visuals/lin_reg.png" width="30%">

**Multivariate Regression**

<img src="Data_visuals/Multivariate/Chosen_Variable_analysis.png" height="30%">

<img src="Data_visuals/Multivariate/multivarplot.png" width="33%"> <img src="Data_visuals/Multivariate/multivarresiduals.png" width="33%"> 

<img src="Data_visuals/Multivariate/mvtest_PDF.png" width="33%"> <img src="Data_visuals/Multivariate/testresiduals.png" width="33%"> <img src="Data_visuals/Multivariate/multivarconfusion.png" width="32%">

**ML Accuracy**

<img src="Data_visuals/ML_acc.jpg">

**Confusion Matrices**

<img src="Data_visuals/Confusionmatrices/knn_confusion1.png" width="30%"> <img src="Data_visuals/Confusionmatrices/lr_confusion1.png" width="30%">
 <img src="Data_visuals/Confusionmatrices/svc_confusion1.png" width="30%"> 

## :bookmark_tabs: Results

## :closed_book: Concluding Statements
