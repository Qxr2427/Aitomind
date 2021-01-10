# Inspiration
With remote learning seeming to be the norm for a significant period of time many students are finding the transitions difficult. Particularly that consuming large amounts of online content through hour long videos and online textbooks isn't the most engaging or effective form of learning. We wanted to build something that helped students learn in a more interactive and efficient manner. Aiming to promote conceptual understanding rather than brute memorization

# What it does
Aitomind (Auto+AI generated mindmaps) is web application that transcribes the speech of a video and organizes it into a mind map structure. Users upload a video of their choice and a couple minutes later a mind map containing the key concepts of the video is generated. This helps the user understand the structure of the video/lesson as well understand the relation between key ideas. Most importantly, each concept will have a timestamp so that the user can easily navigate to the part of the video where the concept was discussed.

# How We built it
The core of Aitomand is the natural language processing algorithm that transcribes text from videos and analyzes it to create a mindmap. This was made up of several azure services including: azure text-analytics, text-to-speech as well as the azure machine learning platform to implement our own models. We used azure text-to-speech to transcribe the text form the video, then used azure text-analytics to do key word and entity analysis. From there we used our own machine learning model, which is trained on a variety of academic datasets using a word to vector model. This is all ran on an express server and written in node.js. The frontend was built using react and styled with the bulma css library

