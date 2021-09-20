---
layout: post
published: true
category: updates
title: Project Ideation - Holly Rieping
author: Holly Rieping
---
### What is the issue, aspect that you would like to address?
I would like to address auto-processing audios through Natural Language Processing as well as exploring how different ranking/connecting algorithms of audio files would impact a user’s experience.

### Who is the audience for your project?
My audience is ideally the general public. I want everyone who comes to the website to be able to both learn more about something they wanted to and something they didn’t know before. I also want to include auto-scrolling transcripts that match the audio clips to prioritize accessibility in the website.

### How does your envisioned audience benefit from your approach?
I want to give users the capability to hear about topics they want to hear and be able to explore related topics that emerge as they listed. I also want to let them choose who they want to hear from, whether that be a specific person by name or any student, faculty, alumn, etc. This way, users can explore what they want to know about, and can explore different paths based on what they hear.

### What is the level and kind of participation by your audience?
My audience would have to first choose who they want to hear from in a dropdown that would include options for black/nonblack students/alumni, faculty, staff and administrators, anyone, or the option to type in a specific name. Then they would have the option to input keywords for topics that they want to hear about or listen to a randomly selected audio clip.

### How do you envision to achieve this goal?
I plan to first develop a natural language processing script (probably in python) that could be run on any audio file and outputs a file of metadata that includes “chunking” time stamps for distinct breaks in the audio to auto-segment the clips, tags for the file as a whole, and tags for each chunk. To get the tags from each chunk, we can select the top N most frequently used nouns, verbs, adjectives, or phrases through natural language processing as well. This file creation and audio processing would be done offline and the premade files would be accessed by the website.

Next, I plan to develop a few different algorithms for what order audio files can be presented to the user based on their inputs. This could include exploring different data structures like trees or linked lists, or creating graphs with different edge weights based on tags and ranking how related an audio clip is to the user’s input. The order of the user’s experience would be generated in real time when they submit their inputs.

Once they submit their inputs, they would be taken to their first audio clip and given information about who the speaker is. They could then be presented with the option to listen to the full interview from that speaker, or continue on their journey by selecting a related topic or tag from this audio. This would be done with a web-based script that runs the ranking algorithm.

![hrieping intial design.JPG]({{site.baseurl}}/assets/hrieping%20intial%20design.JPG)

