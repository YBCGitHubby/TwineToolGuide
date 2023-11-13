---
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

{% capture text %}
`You find yourself in a room with two doors.`
{% endcapture %}
{% include card.html text=text header="Enter your initial content of your story into the passage editor." title="" %}

{% include figure.html img="Creating first passage.jpg" alt="First passage" caption="Story Map and Passage Editor" width="100%" %}

#### STEP 3
Add Links. Use double square brackets `([[ ]])` to create a link to another passage. 

{% capture text %}
You find yourself in a room with two doors.
`[[Go through the left door]]`
`[[Go through the right door]]`
{% endcapture %}
{% include card.html text=text header="Enter" title="" %}

The text "Go through the left door" and "Go through the right door" are clickable links that will lead to new passages when clicked. 

{% include figure.html img="Creating passage 02.jpg" alt="Add Links" width="100%" %}

The pipe `(|)` can be used to rename the link.

{% capture text %} 
You find yourself in a room with two doors.
`[[Go through the left door.|Left Door]]`
`[[Go through the right door.|Right Door]]`
{% endcapture %}
{% include card.html text=text header="Enter" title="" %}

In this example, "Go through the left door" and "Go through the right door" are clickable links. The text after the pipe `(|)` is the displayed link text, and the text before the pipe is the name of the passage to which the link leads.

{% include figure.html img="Creating passage-pipe.jpg" alt="Rename links" width="100%" %}

#### STEP 4 
Create Linked Passages | Double click on the newly appeared passages on the Story Map to open the passage editor. 

{% capture text %}You enter a garden with colorful flowers.
`[[Explore the garden.|Explore Garden]]`
{% endcapture %}
{% include card.html text=text header="Enter for Left Door" title="" %}

{% capture text %}You find a dark cave.
`[[Enter the cave.|Dark Cave]]`
{% endcapture %}
{% include card.html text=text header="Enter for Right Door" title="" %}

Here, the `(Go through the left Door)` and `(Right Door)` passages are linked to from the previous passage. The links take the reader to different parts of the story based on their choices.

#### STEP 5
Continue creating linked passages to build the branching structure of your narrative.

{% capture text %}As you walk through the garden, you find a hidden treasure.
`[[Take the treasure.|Treasure]]`
{% endcapture %}
{% include card.html text=text header="Enter for Explore Garden" title="" %}

{% capture text %}Inside the cave, you encounter a dragon.
`[[Confront the dragon.|Confront Dragon]]`
{% endcapture %}
{% include card.html text=text header="Enter for Dark Cave" title="" %}

The link texts are customized for clarity, but the passage names remain distinct. Your can give the same name to different passages.

#### STEP 6
Add Endings or Further Links | Conclude your story or provide further choices in linked passages.

{% capture text %}Congratulations! You found the treasure and completed the adventure.
`[[Restart]]`
{% endcapture %}
{% include card.html text=text header="Enter for Treasure" title="" %}

{% capture text %}The dragon breathes fire, and your journey comes to an end.
`[[Restart]]`
{% endcapture %}
{% include card.html text=text header="Enter for Confront Dragon" title="" %}

In these examples, `Restart` is the displayed link text leading to the `Start` passage.

#### STEP 7
Rename your starting passage as `Adventure begins` to link it to the last passage. Open the passage editor for the starting passage by double clicking on it. Then use `Rename` button to change the name of the passage. 

{% include figure.html img="RenamePassage.jpg" alt="A complete story" width="100%" %}

Let's link the last passage to the first passage and complete your first story! Open the passage editor for `Restart`.

{% capture text %}
`[[Adventure begins]]`
{% endcapture %}
{% include card.html text=text header="Enter" title="" %}

{% include figure.html img="AllPassages.jpg" alt="A complete story" width="100%" %}

{% include alert.html text="Congragulations! You created your first story/game with Twine. Let's [[play]](https://ybalogluc.github.io/TwineToolGuide/content/docs/publishstory.html)" align="center" color="success" %}
