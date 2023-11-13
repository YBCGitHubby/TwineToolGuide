---
section_id: Create Content
nav_order: 3
title: Create Your First Story
topics: New Story; Passages; Links; Basic Syntax
---

{% include video-embed.html youtubeid="dtNHIgcI2nY" caption="Create a Basic Story with Twine" %}

#### STEP 1
Open Twine and click +New button under Story tab. Enter a name for your story. Click Create button.

{% include figure.html img="Create a new story.jpg" alt="New Story" caption="Click +New and name your story!" width="100%" %}

#### STEP 2
Once you create your story, Twine will open the Story Map screen to create passages and links. Every new story starts with a single passage which appears on the Story Map as a square with a green rocket icon attached to it. When you double click on it, Twine opens a dialogue box to edit the passage.

Enter your initial content of your story into the passage editor. 

#### STEP 3
Add Links. Use double square brackets `([[ ]])` to create a link to another passage. 

{% capture text %}
You find yourself in a room with two doors.
`[[Go through the left door]]`
`[[Go through the right door]]`
{% endcapture %}
{% include card.html text=text header="Enter" title="..." %}

The text "Go through the left door" and "Go through the right door" are clickable links that will lead to new passages when clicked. 

{% include figure.html img="Creating passage 02.jpg" alt="Add Links" width="100%" %}

The pipe `(|)` can be used to rename the link.

{% capture text %} 
You find yourself in a room with two doors.
`[[Go through the left door.|Left Door]]`
`[[Go through the right door.|Right Door]]`
{% endcapture %}

In this example, "Go through the left door" and "Go through the right door" are clickable links. The text after the pipe `(|)` is the displayed link text, and the text before the pipe is the name of the passage to which the link leads.

{% include figure.html img="Creating passage-pipe.jpg" alt="Rename links" width="100%" %}
