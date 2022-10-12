# OPELA

>OPELA [O:pæ:la] stands for **O**pen-domain conversations by **P**ersonas with **E**mpathy, **L**ong-term memory, and **A**ttractive personality.

>This data is a conversation playing two roles. 
 One person acts as a persona with a fictional character (or "concept"), and the other acts as a normal user. 
 This is similar to typical conversation between a chatbot (persona) and a person (user), which assumes a situation of interacting with the chatbot that reacts to the user with empathy and an active attitude. 
 The conversations range from as short as 15 turns to as long as 80 turns on a variety of everyday topics.

## This data is a joint collaboration project between Smilegate AI and Seoul National University.

# Researchers

- [Yoon Kyung Lee](https://yoonkyunglee.com)<sup>1</sup>, [Won Ik Cho](https://sites.google.com/site/warnikchow)<sup>2</sup>,Seoyeon Bae<sup>1</sup>, Jihwan Kim<sup>2</sup>, Jisang Park<sup>1</sup>, Nam Soo Kim<sup>2</sup>, Sowon Hahn<sup>1</sup>

- Hyunwoo Choi<sup>3</sup>, Joonsun Hwang<sup>3</sup>, Moosung Kim<sup>3</sup>

<sup>1</sup>[Human Factors Psychology Lab](https://hfpsych.snu.ac.kr/), Department of Psychology, Seoul National University <br>
<sup>2</sup>[Human Interface Lab](https://hi.snu.ac.kr/), Department of Electrical and Computer Engineering, Seoul National University <br>
<sup>3</sup>[Smilegate AI](https://smilegate.ai/)


# Purpose of Data Collection
- Many conversation data using personas were presented in a variety of languages, the majority of which were English and Chinese. Persona, on the other hand, was primarily determined by a number of circumstances in specific situations. 
- We looked into how conversations go and which personas people find engaging (e.g., a game NPC with a human-like attractive personality). 
- We were also interested in what aspects or phrases people find engaging, empathetic, and fun in the conversational agent with persona.

# Data characteristics

- **Data created by real conversations between persona-role and user-role crowdworkers.**
    - The conversation takes place between a small group of persona participants who have a fixed persona concept and an unspecified number of general participants.
    - We provided distinct guidelines for persona participants and general participants, and we held discussions following training and testing.
    - We developed guidelines for collecting Korean dialogue data, which is more relevant than existing dialogue data that are made up of translations from non-Korean data.
    - We also gathered self-labeled ground truth in psychological attributes (e.g., empathy, connectedness, fun, and engaging) in which persona and user evaluated conversations with each other while building conversation data.

- **Data annotated by third-party labelers with empathy, self-disclosure, engaging, uneasiness, strangeness, and activeness**.
<br>
Labels can be used :
    1) to predict the conversation that a specific persona will have using ML/DL training, 
    2) to discover the specific direction where the conversation leads using a supervised learning method, 
    3) to determine which factors positively or negatively affect thoughts about each other not only in human-bot conversations but also in human-human conversations, and 
    4) to identify which factors positively or negatively affect thoughts about the conversation partner (both human and machine)
    5) or many other creative directions.

# Methods
The conversation in this dataset was collected based on the persona-user conversation guideline jointly developed by Human Factors Psychology Lab and Human Interface Lab, and Smilegate AI Center. The data collection process includes additional vocational training of crowdworkers recruited by DeepNatural AI (Seoul, Korea). 

<img src="https://deepnatural.notion.site/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F320cf5a7-583c-45f3-b7c1-770e99d99fdf%2F%E1%84%85%E1%85%A6%E1%84%8B%E1%85%B5%E1%84%87%E1%85%B3%E1%86%AF%E1%84%85%E1%85%A5_%E1%84%8C%E1%85%A1%E1%84%8B%E1%85%B2%E1%84%83%E1%85%A2%E1%84%92%E1%85%AA_%E1%84%91%E1%85%B3%E1%84%85%E1%85%A9%E1%84%8C%E1%85%A6%E1%86%A8%E1%84%90%E1%85%B3A2(01).png?table=block&id=b2b8a23d-7667-422c-89d5-9887d1e0c53b&spaceId=04a9e1fc-cc2a-4e1c-8b27-dd1dc75a88f9&width=2000&userId=&cache=v2" width="500"/>

### Recruitment of persona participants

    - Announcement on how to set up a persona
    - Persona interview of research facilitator and project manager (conversation and dialogue evaluation)
    - Recruitment of persona participants with as many different profiles as possible

        - Example: "Little Donut"
            - "A power housekeeper who likes movies and dramas (especially family sitcoms) and likes to listen to music (especially Ariana Grande)”.

        - Example: "Hungry Jambo"
            - "A fan of fantasy novels who has been reading continuously for nearly 30 years, from the exorcism to the point of omniscient readership. Comics, webtoons, movies, music, and performances are all enjoyable, and omnivorous, regardless of genre. Being an owl, having to do something early in the morning is unfavorable. Even in midsummer Even on a sick or hot day, you have to turn it on. The person who gives you food is unconditionally considered a good person. Sometimes, you are in a depressing mode out of control, but mainly when you are hungry, in everyday life, you are super-positive and optimistic."
    - Training on how to maintain conversation context, how to speak first, and how to use the messenger interface according to the settings in the persona guidelines

<img src="https://deepnatural.notion.site/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2Fb2262017-70f5-4089-8bc3-76cb8fd5d124%2F%EB%A0%88%EC%9D%B4%EB%B8%94%EB%9F%AC_1230%EC%9E%90%EC%9C%A0%EB%8C%80%ED%99%94_%EC%9E%91%EC%97%85%EC%9E%90(04).png?table=block&id=1ef723d9-58b0-41b3-bae3-9747a675f700&spaceId=04a9e1fc-cc2a-4e1c-8b27-dd1dc75a88f9&width=2000&userId=&cache=v2" width="500"/>

### User-role crowdworker recruitment

    - Project title: 'Free conversation with someone with a concept' on a crowdsourcing platform
    - Crowdworkers who want to participate must pass a test based on user guidelines to participate in the project
    - Each worker could freely initiate a conversation with the persona they want
    - Be aware of the precautions during the conversation (ethics rules, avoid using photos/emoticons, allow inscriptions, etc.)
    - Workers receive a basic reward for participating in conversations over a certain level (15 turns), and after that, they can receive more rewards for additional conversations.

### Conversation progress and survey
- Conducted actual conversations using the conversation tools provided by the crowdsourcing platform
- [Dialogue tool usage guide](https://deepnatural.notion.site/07557d83a7b1487a9da156a33c7ce282)

 - At the end of each conversation, the persona and the user conducted a survey about the conversation they had.
- The contents of the survey are provided in the data evaluation and data description below.

### Conversation evaluation
- After collecting the entire conversation, third-party annotators evaluated each sentence for six factors, including self-opening and empathy.
- Evaluation details are provided in the data evaluation and data description below.


## Data Evaluation
***

Conversation partners and engaging were evaluated using survey and third-party annotations.

**Evaluation of conversation participants (self-annotating)**

- The survey includes demographic information about conversation participants, satisfaction with the conversation, and their feelings about the conversation, such as connection, engaging, and fun.

**Evaluation of the labelers (third-party annotating)**

- In the third-party evaluation, six psychological attributes are tagged for each sentence: strange, uneasy, active, engaging (attractive personality), self-disclosure, and empathy.



## Data Description
***

### Survey data

The components for labelerX are provided as an array of sentence arrays, the same as the final label in the annotated data.

**doc_id** - Persona name_worker name and number_total turns_total sentences

**persona_name_original** - The full name of the persona used in the actual conversation, such as 'Professor A', 'Careful Ferret', 'Little Donut', etc.

**user_id** - The unique id of the user (randomly generated key)

**total_turn** - Total number of turns in conversation (same as 'Total Turns' in doc_id)

**total_sent** - Total sentences in conversation (number of rows in conversation dataset, same as 'total sentences' in doc_id)

**total_minutes** - Actual time spent in real persona-to-user conversations (considering virtual time X)

**pause_count** - The number of virtual time intervals the persona used per conversation

**total_pause** - Total time using virtual time intervals within the conversation

**pause_hour** - The (hypothetical) n time interval used within the conversation (Python list format). Each order in the list is the same as the virtual time interval order used in the real conversation. The length of the list is equal to the value of ‘pause_count’

**age** - The age of the user

**gender** - The reported gender of the user: 1 = female, 2 = male, 3 = other

**edu** - User’s reported education level: 1 = Elementary school graduate, 2 = Middle school graduate, 3 = High school graduate, 4 = University graduate, 5 = Graduate or higher

**income** - User’s reported income level: 1 = less than 1 million won, 2 = more than 1 million won - less than 2 million won, 3 = more than 2 million won - less than 3 million won, 4 = more than 3 million won - less than 4 million won, 5 = 400 over 10,000 won

**open_chat_exp** - Whether or not the user has open chat experience: 1 = Yes, 2 = No

**friend_persona** - 'friendliness' rated by users for personas: 1 - 4 points

**friend_user** - 'friendliness' rated by personas for users: 1 - 4 points.

**engaging_persona** - 'engaging', rated by users for persona: 1 - 4 points

**engaging_user** - 'engaging', rated by personas for users: 1 - 4 points

**connect_persona** - Feeling of 'connection', rated by users for personas: 1 - 4 points

**connect_user** - Feeling of 'connection' rated by personas for users: 1 - 4 points

**respect_persona** - 'respect' rated by users for personas: 1 - 4 points

**respect_user** - 'respect' rated by personas for users: 1 - 4 points

**fun_persona** - 'fun' rated by users for personas: 1 - 4 points

**fun_user** - 'fun' rated by personas for the users: 1 - 4 points

**natural_persona** - 'naturalness' rated by users for personas: 1 - 4 points

**natural_user** - 'naturalness' rated by personas for users: 1 - 4 points

**blri_persona** - The level of 'empathy' of personas rated by users: out of 64 (minimum of 16)

**blri_user** - The level of 'empathy' of users rated by personas: out of 64 (minimum of 16)

**persona_text_all** - The entire text uttered by the persona from the conversation dataset (each sentence is separated by an enter key)

**user_text_all** - The entire text uttered by the user in the conversation dataset (each sentence is separated by an enter key)

**persona_summary** - Summary of conversation by personas (in form of hashtags) 

**user_summary** - Summary of conversation by users (in form of hashtags)

**labelerX_strange** - The level of strangeness rated for the sentence by the Xth labeler: 1 = the sentence is not strange, 0 = the sentence is strange

**labelerX_uneasy** - The level of uneasiness rated by the Xth labeler for the sentence: 0 = the sentence is uncomfortable, 1 = the sentence is not uncomfortable

**labelerX_engage** - The level of engagingness rated by the Xth labeler for the sentence: 0 = unlikely to find the sentence engaging, 1 = likely to find the sentence engaging.

**labelerX_active** - The level of activeness rated by the Xth labeler for the sentence: 0 = It is unlikely that the sentence was felt as active, 1 = It is likely that the sentence was felt as active

**labelerX_self** - The level of self-disclosure rated by the Xth labeler for the sentence: 0 = No self-disclosure, 1 = Self-disclosure by sharing only objective facts or simple tastes/information, 2 = subjective, Self-disclosure, including expressing feelings and emotions

**labelerX_empathy** - The level of empathy rated by the Xth labeler for that sentence: 0 = Not Applicable, 1 = Empathic Failure, 2 = Low Empathy Response, 3 = Moderate Empathic Response, 4 = High Level of active empathy


## Annotated data

All attributes are written per statement (per line shift to be exact).

**doc_id** - Persona name_userID_total turns_total sentences_labeler1 gender and number_labeler2 gender and number_labeler3 gender and number

**sent_id** - Persona name_userID_total number of turns_total number of sentences_corresponding sentence number

**person_type** - User = if the sentence is a user, persona = if the sentence is a persona

**person_name** - User: a unique number assigned to a user within the project (eg user0001), Persona: abbreviated form of the persona's full name for conversation (eg, ‘little donut’: donut, ‘careful ferret’: ferret)

**person_name_original** - The full name used by the persona in the actual conversation, such as 'Careful Ferret' or 'Little Donut'

**turn_notation** - Which turn the sentence is in the entire conversation

**time** - The persona and the time the user actually sent the conversation on the chat platform

**is_pause** - 1 = if the sentence is used to set a hypothetical time interval (eg 1 hour has elapsed), 0 = if the sentence contains general conversational content rather than a hypothetical time interval

**text** - The actual conversation content between the persona and the user (one conversation sent to the conversation platform corresponds to one cell)
  
**labelerX_strange** - The level of strangeness rated for the sentence by the Xth labeler: 1 = the sentence is not strange, 0 = the sentence is strange

**labelerX_uneasy** - The level of uneasiness rated by the Xth labeler for the sentence: 0 = the sentence is uncomfortable, 1 = the sentence is not uncomfortable

**labelerX_engage** - The level of engagingness rated by the Xth labeler for the sentence: 0 = unlikely to find the sentence engaging, 1 = likely to find the sentence engaging

**labelerX_active** - The level of activeness rated by the Xth labeler for the sentence: 0 = unlikely to feel the sentence as active, 1 = likely to feel the sentence as active

**labelerX_self** - The level of self-disclosure rated by the Xth labeler for the sentence: 0 = No self-disclosure, 1 = Self-disclosure by sharing only objective facts or simple tastes/information, 2 = subjective, Self-disclosure, including expressing feelings and emotions

**labelerX_empathy** - The level of empathy rated by the Xth labeler for that sentence: 0 = Not Applicable, 1 = Empathic Failure, 2 = Low Empathy Response, 3 = Moderate Empathic Response, 4 = High Level of active empathy

**person_id** - Unique ID given to the persona and user at the time of the project
  
**labeler_strange** - The final determined strange label reflecting the annotations of the three labelers: details are the same as labeler1_strange

**labeler_uneasy** - The final uneasy label: details are the same as labeler1_uneasy

**labeler_engage** - The final engaging label: details are the same as labeler1_engage

**labeler_active** - The final activeness label: details are the same as labeler1_active

**labeler_self** - The final self-disclosure label: details are the same as labeler1_self

**labeler_empathy** - The final empathy label: details are the same as labeler1_empathy


### Final Label Determination

* When there are two label candidates (strange, uneasy, engaging, active)
    - The final label is decided through three annotations majority voting.
* If there are 3 or more label candidates (self, empathy)
    - When the final label is decided by majority voting (a), the final label is decided only by voting.
        - If the annotations of all three labelers are different (b), the final label is decided through the following logic.
    - For the number of C label candidate classes, calculate the frequency at which a specific labeler belongs to the majority in advance in case of majority voting with the label in (a).
        - The obtained C by 3 matrices can also be defined as 'reliability of each labeler's annotation' for each label candidate.
    - Also, for C label candidate classes, `the frequency at which a specific labeler chooses the corresponding label and does not belong to the majority (a) is calculated in advance.
        - The obtained C by 3 matrices can also be defined as the 'reliability of each labeler's annotation' for each label candidate.
    - For the sample in (b) where the conflict occurs, the product of the labeler's annotation reliability and unreliability is calculated for the label class written by each labeler.
    - The label class filled in by the labeler with the highest reliability is determined as the final label.
    - If it is not determined through the above process, find the frequency that a specific labeler belongs to the majority in (a), and determine the label annotated by the labeler with the highest frequency as the final label. (regardless of label candidates)
    - If it is not determined by this method, it is determined randomly among three label candidates. (none detected to this point)



### Precautions

- The data were generated in a unique setting known as a crowdsourcing platform, and some conversation patterns may differ from that of typical open dialogue. Participants' (crowdworkers') time was compensated, and some of the information and content they provided may not be accurate.

- The data could reflect participants' subjective feelings on socially notable individuals, brands, or social phenomena, which was not ruled out if it wasn't ethically harmful.

- The opinions represented in the survey results may differ from those of other individuals.

- Because the labeling in this data may reflect the subjectivity of the annotator, it is recommended to utilize these findings as a guide.

- Because our goal was to collect realistic conversation from diverse communities, we didn't remove content advocating or referencing pseudoscience to the conversational partner for enjoyment (e.g., determining personality with blood types, the Myers-Briggs Type Indicator, and other popular non-scientific beliefs, etc.). However, the aforementioned instances lack scientific backing and are unrelated to the study's scientific objectives and findings. Researchers' discretion is advised when utilizing this data for psychology research.



### Cite
```
@misc{SmilegateAI2022OPELA,
  title         = {OPELA stands for Open-domain conversations by Personas with Empathy, Long-term memory, and Attractive personality.},
  author        = {Smilegate AI},
  year          = {2022},
  howpublished  = {\url{https://github.com/smilegate-ai/OPELA}},
}
```
```
@article{lee2022feels,
  title={"Feels like I've known you forever": empathy and self-awareness in human open-domain dialogs},
  author={Lee, Yoon Kyung and Cho, Won Ik and Bae, Seoyeon and 
  Choi, Hyunwoo and Park, Jisang and Kim, Nam Soo and Hahn, Sowon},
  year={2022},
  publisher={PsyArXiv}
}
```

### Inquiries
***
- E -mail : smilegate_ai@smilegate.com
- 주최 : Smilegate AI 센터
***

![logo_black_gray](https://user-images.githubusercontent.com/95196586/147066863-b9f99434-3ce8-463f-abb4-5e672b3a1fda.png)
