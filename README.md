# MHARD – Mental Health App Reviews Dataset

## Overview  
The Mental Health App Reviews Dataset (MHARD) contains user reviews from 73 mental health apps on the Google Play Store, collected using the SerpAPI tool. The dataset includes **200,972** reviews posted between **March 29, 2011** and **July 11, 2023** from apps with over 100k downloads. It is designed to support research in user experience, sentiment analysis, app evaluation, and human-AI collaboration.

## Data Features  
Each record in the dataset includes original user-written reviews, ratings, developer responses, and AI-generated rating predictions from multiple large language models (LLMs). Below is a summary of key features:

- `UID`: Unique ID for the review  
- `app_name`: Name of the app  
- `rating`(ground truth): User-provided rating (1–5)
- `date`: Review date  
- `review`: Raw user review text  
- `review_cleaned`: Preprocessed version of the review  
- `likes`: Number of likes/upvotes on the review  
- `response_date`: Date of developer response (if any)  
- `response`: Developer's reply to the review (if any)  

### LLM-Based Predictions:
- `pred_gpt3.5instruct`: Prediction from GPT-3.5 Instruct  
- `pred_gpt3.5turbo`: Prediction from GPT-3.5 Turbo  
- `pred_gpt4`: Prediction from GPT-4  
- `pred_gemini1.5flash`: Prediction from Gemini 1.5 Flash  
- `pred_gemini1.5pro`: Prediction from Gemini 1.5 Pro  
- `pred_llama3.1_8b`: Prediction from LLaMA 3.1 (8B)  
- `pred_llama3.3_70b`: Prediction from LLaMA 3.3 (70B)  

## Available Files

### [MHARD_dataset.csv](./MHARD_dataset.csv)  
This is the **full dataset** containing 200,973 user reviews collected from 73 mental health apps on the Google Play Store

### [MHARD_dataset_sample.csv](./MHARD_dataset_sample.csv)  
This is a **random sample of 100 entries** selected from the full dataset. It is intended for quick exploration, testing, or demonstration purposes. The structure and features are identical to the full dataset.

## Citation  
If you use this dataset or it has informed your work, we kindly ask that you cite the corresponding paper to acknowledge and support our research efforts.

> *[Pending]*




## Included Apps

This dataset includes reviews from the following mental health apps:

`amaha`, `anxietyrelief`, `anxietytest`, `bearable`, `besthelp`, `blockapp`, `breathball`, `breeze`, `calm`, `cbtguide`, `cbttools`, `cerebral`, `chiku`, `clarity`, `constant`, `dailybean`, `dare`, `daylio`, `digitalwellbeing`, `evolve`, `fabulous`, `feelbetter`, `finch`, `gratitude`, `happify`, `headspace`, `healthily`, `healthyminds`, `heyy`, `iam`, `ifeel`, `intellect`, `minddiagnostics`, `minddoc`, `mindease`, `mindshift`, `mindshine`, `moodflow`, `moodpress`, `moodspace`, `moodtools`, `moodtracker`, `mypossibleself`, `norbu`, `pixels`, `reflectly`, `reflexio`, `regain`, `remente`, `rootd`, `roubit`, `sanvello`, `sevencups`, `sharecare`, `sparkle`, `stoppanic`, `stressscan`, `talklife`, `talkspace`, `teencounseling`, `thrive`, `tochi`, `twentyninek`, `unwinding`, `up`, `voice`, `voidpet`, `vos`, `welltory`, `whatsup`, `woebot`, `wysa`, `youper`

## Sample Data  

|UID|app\_name|rating|date|review|review\_cleaned|likes|response\_date|response|pred\_gpt3\.5instruct|pred\_gpt3\.5turbo|pred\_gpt4|pred\_gemini1\.5flash|pred\_gemini1\.5pro|pred\_llama3\.1\_8b|pred\_llama3\.3\_70b|
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
|72038|calm|5|October 27, 2018|Excellently designed app\. In this day and age when we are being inundated by information overload,this app gives one many reasons to unwind and get a digital detox, a breath of fresh air :\)|excellently designed app day age inundated information overloadthis app give one many reason unwind get digital detox breath fresh air|1|NaN|NaN|5\.0|5\.0|5\.0|5\.0|5\.0|5\.0|5\.0|
|166769|dare|5|November 16, 2021|I love this app it's great it has helped me better than any app I have used|love app great helped better app used|0|November 17, 2021|Thank you so much for your review,  Please recommend our app to your friends, and don’t hesitate to shoot us a note at  if you have any questions\.|5\.0|5\.0|5\.0|5\.0|5\.0|5\.0|5\.0|
|179492|gratitude|5|May 28, 2019|Simple\. Easy to use\. Customizable\. No ads or monthly fees\. What more could you ask for?|simple easy use customizable ad monthly fee could ask|0|May 29, 2019|Thank you very much for your 5-star review\!\!\!|5\.0|5\.0|5\.0|5\.0|5\.0|5\.0|5\.0|
|45106|headspace|2|June 21, 2023|I thought Headspace would be great\.\.\. But the only thing you can do unless you get a free trial is to wach a two minute video on the basics of headspace\. No sneak preveiw of what you could do with the free trial, no nothing\.|thought headspace would great thing unless get free trial wach two minute video basic headspace sneak preveiw could free trial nothing|1|June 22, 2023|We appreciate your feedback\! We recently updated the Headspace app to allow all new members to unlock the entire Headspace library through our free trial\. We still offer free content outside of the app on social media channels and still offer K-12 organizations free memberships in the US, UK, Australia, and Canada\.|2\.0|2\.0|2\.0|1\.0|2\.0|3\.0|1\.0|
|123464|moodpress|5|December 15, 2022|The app is really good, but I give it only 3 stars as unfortunately their are only few moods option which is so unrealistic days come where I can't even choose from the specific emotions as they only about 8 available, so it would be great if you added more emotions options|app really good give star unfortunately mood option unrealistic day come cant even choose specific emotion available would great added emotion option|0|March 06, 2023|UPDATE: Hi , We finally made it\! \! Please update your Moodpress to the latest version 1\.4\.0\! Now you can choose the emoji you like to add three more moods for free, or try to change the moods name you don't use now :D|3\.0|3\.0|3\.0|3\.0|3\.0|3\.0|3\.0|

## Note

Please note that some LLM predictions are missing due to errors encountered during the experiments. In some cases, the models returned unexpected outputs such as bracketed numbers, lengthy explanations, or error messages.

## License  
This project is licensed under the MIT License - see the [LICENSE.md](./LICENSE)  file for details

## Contact  
For questions, reach out to Kyle Wang at kylewang@udel.edu or Moath Erqsous at merqsous@udel.edu

#api #computer-science #application #machine-learning #supervised-learning #unsupervised-learning #classification #recommendation-system #dataset #mental-health #stress #anxiety #llms #chatgpt
