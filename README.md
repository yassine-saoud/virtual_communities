# Fitness Communities: Building Online Well-being Experiences

## General Introduction

Our project focuses on creating online fitness communities to support and enhance a great well-being experience. Online communities provide a conducive environment where members can share their knowledge, connect with like-minded individuals, and work together to achieve their fitness goals. Renowned brands such as Strava, Fitbit, and MyFitnessPal serve as successful examples of such online communities.

The objective of our project is to bring together people of all fitness levels within specific communities. These communities will enable members to share knowledge, network with peers, and engage in a learning, challenge, and motivation environment to enhance their overall well-being. To facilitate this, we harness artificial intelligence (AI) to analyze user data and integrate them into communities tailored to their profiles, goals, experience levels, workout types, coaches, and activities. Various AI techniques, including clustering, similarity analysis, and neural networks, are employed to create groups based on user characteristics such as fitness goals, experience levels, training profiles, and more.

## Data Collection

To initiate our project, the first step involved data collection. Given the absence of a preexisting dataset suitable for our study, we decided to create our dataset using web scraping techniques. However, this approach presented certain challenges, necessitating answers to questions such as:
- What variables should we extract to build our dataset?
- What are the relevant topics or subjects to search for?
- How should we create this dataset (i.e., which websites or platforms to use)?

In regards to the first question, our goal was to base information on customers' details, such as their age, gender, country, and a personal description outlining their well-being interests. However, it's difficult to find personal data (e.g., age, gender, country) on the Internet, and even if available, it's often limited to a small number of people. Yet, we wanted to create a larger dataset to obtain more relevant results (we considered generating this data randomly, but found that it would simply bias the results as these data are supplementary). Hence, we decided to collect only comments (as it's the most important variable for us to gain a clear understanding of a customer's interests and assign relevant communities) along with the authors' names (to group comments created by the same author and avoid any bias). Thus, our final dataset will consist of two columns: "author" and "comment."

Regarding the topics to search for, we identified three main subjects in the well-being domain: health, fitness, and nutrition. However, as we conducted research, we discovered other interesting sub-topics. Here's the final list of key topics we used: [- Fitness - nutrition - obesity - diabetes - smoking - intermittent fasting - vegetables and fruits - drink water - sugar challenge - hear loss - teeth health - heart disease - wake up early - lower back pain - eye disease - dry eye - blood pressure - nerves - Exercise routines for beginners - Yoga - Healthy meal plans and recipes - mental health - Running and endurance training - Strength training and muscle building - Sleep hygiene and the importance of rest - healthy lifestyle].

Now that we have defined our dataset structure and the topics to search for, we need to select the platforms to target for data collection. This step was particularly challenging because we had to find platforms that contained sharing spaces where people could express their views through comments. Furthermore, these comments had to be relevant, as we often encountered irrelevant content such as "ok" or "thanks." Thus, we had to look for platforms where relevant comments were available for the previously mentioned topics. After extensive research, we ultimately chose to work with YouTube platforms.
[Scarping code](https://github.com/yassine-saoud/virtual_communities/blob/main/v_scrap.ipynb)

## Preprocessing

In this chapter, we will begin the preprocessing of our dataset, a crucial step that plays an essential role in preparing our raw data for the next stage.
and to achieve this we use NLP techniques to optimize results
[preprocessing notebook](https://github.com/yassine-saoud/virtual_communities/blob/main/preprocessing.ipynb)

## Creating clustering models

to achieve best results we tried many approch (during the numeric representation of comments or during model selection) to choose our final clustering model
[model building code](https://github.com/yassine-saoud/virtual_communities/blob/main/pfa.ipynb)

## Technologies

- Web scraping
- NLP
- Clustering


