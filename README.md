# Data-Bias

# Hypothesis
This project aims to explore the effectiveness of adjusting the Perspective bias model's severity threshold in identifying varying levels of toxicity in TikTok comments.

The hypothesis is that the model might miss a lot of the toxicity because tiktok uses lingo that might not be familiar to language models yet.

To evaluate the model's performance, the project utilizes a dataset of TikTok comments, with the initial exploration focusing on the first 10 comments. This approach aims to gauge the model's ability to discern toxicity nuances in the context of TikTok interactions.

# Perspective API
I am using the Perspective API code to run through the moderation machine learning model to find the toxicity scores of the tiktok comments I gathered from my feed.

The Perspective API's toxicity tool is a useful tool for identifying and flagging potentially toxic content. It is used in a variety of applications, like social media moderation, online forums, and other digital interactions.

To evaluate the toxicity levels of trending news headlines, I used the Perspective API.

The initial step involved importing the necessary libraries to run the API's operation. Then, a unique API key from Google Cloud was utilized to establish a connection between the API and the project.

The codebase provided in the assignment instructions served as the foundation for this analysis. I made modifications to enable the incorporation of the dataset into the model via a CSV file.

Additionally, I also added a code to generate a new file containing both the headlines and their corresponding toxicity scores.

Finally I also added code categorize the toxicity scores into a column in the new file that contained both the headline text and toxicity scores.

# Results
The implementation of this approach resulted in a analysis of the toxicity levels within trending news headlines. I ran the code twice in order to see where the threshold is for this API to flag content as Toxic and there was a stark difference in just the 0.2 adjustment of the score.

The hypothesis that the model might miss a lot of the toxicity because tiktok uses lingo that might not be familiar to language models yet seems to be corret as the API doesn't flag a lot of the hate comments as toxic unless the score measure is dropped to 0.1.
