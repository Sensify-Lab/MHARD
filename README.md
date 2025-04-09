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
- `pred_gpt35turbo`: Prediction from GPT-3.5 Turbo  
- `pred_gpt4`: Prediction from GPT-4  
- `pred_gemini15flash`: Prediction from Gemini 1.5 Flash  
- `pred_gemini15pro`: Prediction from Gemini 1.5 Pro  
- `pred_llama31_8b`: Prediction from LLaMA 3.1 (8B)  
- `pred_llama33_70b`: Prediction from LLaMA 3.3 (70B)  

## Citation  
If you use this dataset, please cite the corresponding paper:

> *[Pending]*




## Included Apps

This dataset includes reviews from the following mental health apps:

`amaha`, `anxietyrelief`, `anxietytest`, `bearable`, `besthelp`, `blockapp`, `breathball`, `breeze`, `calm`, `cbtguide`, `cbttools`, `cerebral`, `chiku`, `clarity`, `constant`, `dailybean`, `dare`, `daylio`, `digitalwellbeing`, `evolve`, `fabulous`, `feelbetter`, `finch`, `gratitude`, `happify`, `headspace`, `healthily`, `healthyminds`, `heyy`, `iam`, `ifeel`, `intellect`, `minddiagnostics`, `minddoc`, `mindease`, `mindshift`, `mindshine`, `moodflow`, `moodpress`, `moodspace`, `moodtools`, `moodtracker`, `mypossibleself`, `norbu`, `pixels`, `reflectly`, `reflexio`, `regain`, `remente`, `rootd`, `roubit`, `sanvello`, `sevencups`, `sharecare`, `sparkle`, `stoppanic`, `stressscan`, `talklife`, `talkspace`, `teencounseling`, `thrive`, `tochi`, `twentyninek`, `unwinding`, `up`, `voice`, `voidpet`, `vos`, `welltory`, `whatsup`, `woebot`, `wysa`, `youper`

## Sample Data  
|index|UID|app\_name|rating|date|review|review\_cleaned|likes|response\_date|response|pred\_gpt3\.5instruct|pred\_gpt35turbo|pred\_gpt4|pred\_gemini15flash|pred\_gemini15pro|pred\_llama31\_8b|pred\_llama33\_70b|
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
|0|74492|calm|5|July 22, 2020|I use this for my children and myself\. They love to listen to the stories while they go to bed\. And I love the constant reminders throughout the day to just simply breath\!|use child love listen story go bed love constant reminder throughout day simply breath|0|NaN|NaN|5|5|5|4|5|5|5|
|1|168281|dare|5|August 02, 2021|I felt an upcoming anxiety attack rising and I wasn't near anyone who I'm close/comfortable with or understands what I deal with in my head\. I downloaded this app and pressed on the anxiety button and all I needed was the speakers voice to help me feel better and human again\. He explained what I feel so well and then reassuring me that I was safe and completely normal made me feel whole, like a person\. Anyone out there dealing with this, you are so very strong, keep your head up\! 💕🙌|felt upcoming anxiety attack rising wasnt near anyone im closecomfortable understands deal head downloaded app pressed anxiety button needed speaker voice help feel better human explained feel well reassuring safe completely normal made feel whole like person anyone dealing strong keep head|8|August 02, 2021|Thank you so much for your review, Diana\! It really helps us to keep going and delivering the best\. Please recommend our app to your friends, and don’t hesitate to shoot us a note at support@dareresponse\.com if you have any questions\. We would love to hear from you\!|5|5|5|5|5|5|5|
|2|176561|gratitude|5|November 21, 2020|I've definitely enjoyed the mindset change and positive impact journaling about what I'm grateful for has had\. The new challenges have helped keep things fresh and opened my eyes to topics I've never considered before\.|ive definitely enjoyed mindset change positive impact journaling im grateful new challenge helped keep thing fresh opened eye topic ive never considered|0|December 29, 2020|Hey Erin, thank you for the 5 stars\! We're happy to know that you love the app :\) So glad that Gratitude brings a pleasant experience to you\. Thank you for being a part of this\. We send our best wishes\. Have a great day\!|5|5|5|5|5|5|5|
|3|43238|headspace|4|July 27, 2021|I like that it gives you new meditates daily and a 'wakeup' feature for better wellbeing\. I dont love that you have to subscribe for the app, though, as I'm a poor college student\. Other than that, I like that all your daily meditations are in one place\.|like give new meditates daily wakeup feature better wellbeing dont love subscribe app though im poor college student like daily meditation one place|1|NaN|NaN|4|4|4|4|4|4|4|
|4|123823|moodpress|5|January 03, 2023|Nice 👍 I'm going to use it every day for my mood tacker for 2023|nice im going use every day mood tacker|0|NaN|NaN|5|5|5|4|5|5|5|



## Note

Please note that some LLM predictions are missing due to errors encountered during the experiments. In some cases, the models returned unexpected outputs such as bracketed numbers, lengthy explanations, or error messages.

## License  
This project is licensed under the MIT License - see the LICENSE.md file for details

## Contact  
For questions, reach out to Kyle Wang at kylewang@udel.edu
