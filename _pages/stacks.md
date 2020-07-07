---
title: "Who Stacks Up?"
permalink: /stacks/
header:
  image: stacks_header.png
read_time: false
excerpt: Who Stacks Up? is a 'people to follow' recommendation system that connects users with content that they love and that keeps them coming back.
---

## A 'people to follow' recommender

As a Data Science fellow at Insight, I worked with social-media startup Stacks (previously Muze.tv), which lets users easily make video memes by adding punch lines, voice commentary, or labels. As a platform trying to enter the social media space, Stacks is really invested in motivating their users to generate and interact with content in order to create a really rich and lively space that users will want to keep coming back to. To help solve this problem, I consulted with Stacks over a three-week period to build a 'people-to-follow' recommendation system that empowers their users to find content that they'll love. 

I used a hybrid collaborative filtering/content-based recommendation model to leverage information from three data sources: 1) user-account interactions (like following, 'laughing' at a content creator's memes, or sharing memes), 2) user-based features (e.g., interests like 'animals' or 'sports'), and account-based features(e.g., to what extent an account posts about 'politics', 'parties', or 'video games'). The collaborative filtering component of the model is centered around recommending accounts that users similar to you find engaging, which nicely parallels how we naturally find people to connect with. 

Unfortunately, this approach doesn't work for new users who have not yet interacted with much content. To still give these users good recommendations to ideally turn new users into daily ones, the content-based component of the model makes some initial recommendations by matching a user's interests with different accounts' content. And as those users start to interact with content themselves, their recommendations for people to follow will become even more personalized.

To integrate this model into Stacks' existing infrastructure on AWS, I set up two serverless applications to automatically deploy through continuous integration and delivery processes. The first application is a scheduled Lambda function that retrains the model and stores it in an S3 bucket. The second application responds to incoming API requests with the model predictions.

Finally, a few weeks from now, when this feature goes live and people open the Stacks app, personalized suggestions will show up on their phones to help them find relevant content at the tap of a button.