---
title: DaSH Creating content in Markdown
teaching: 15
exercises: 15
questions:
- How to write a tutorial in Markdown?
- What are the different content options?
- Why structure and colours matters?
objectives:
- Identify the importance of consistent training materials
- Explain the Markdown options and benefits
- Create DaSh training materials
keypoints:
- Template/instructions for DaSh fellows content creators 
- Self-learning FAIR trianing materials 
contributions:
  authorship:
  - kkamieniecka
  editing:
  - poterlowicz-lab
abbreviations:
  API: Application Programming Interface
  JSON: JavaScript Object Notation
--- 

##### Introduction
ELIXIR-UK DaSH FAIRifying your data resources for the course can be provided in self-learning training manner:
> <agenda-title></agenda-title>
>
> In this tutorial, we will cover:
>
> 1. TOC
> {:toc}
>
{: .agenda}

The tutorial's content should be placed in the episodes directory file `ep[].md`. Its syntax and structure are adjustable, and will have the following structure:

```markdown
---
layout: tutorial_dash

title: 'title of the tutorial (it will appear on the tutorial page and the topic page)'
zenodo_link: 'link on Zenodo to the input data for the tutorial'
questions: 'questions addressed by the tutorial'
objectives: 'learning objectives and goals'
time_estimation: '15 min'
key_points: 'take-home messages'
contributions: 'everybody who has contributed to this tutorial'
  authorship: 'author'
  editing: 'DaSh team'

---

introduction text

> <agenda​-title></agenda​-title>
>
>
> 1. TOC
> {:toc}

# Section 1
'your text'
## Subsection 1
'your text'
# Conclusion
'your text'
```
<hands-on-title>Update template with your metadata</hands-on-title>

1. Update the tutorial information in the header section:

     ```
     title: "My Content in Markdown"
     ```
 2. (Optional) Add the Zenodo link (if created)

{: .hands_on}

<hands-on-title>Fill out the pedagogical metadata</hands-on-title>

 3. Define questions addressed by the tutorial 
      ```
     questions: "Why do we need this trianing?"
     ```
 4. Define learning objectives and goals 
      ```
     objectives: "What am I going to learn?"
     ```
 5. Define key_points
      ```
     key_points: "How I can apply it in my research?"
     ```
  6. Add contributors
      ```
     contributions: "name surname / github user"
     ```    
{: .hands_on}

<comment-title>Filling up the Metadata</comment-title>
We recommend that you fill out the *questions* and the *learning objectives* metadata before starting writing the tutorial content. Make sure all contributors are listed!
{: .comment}

##### Improving the learning experience
To add *figures* into training we use the following markdown syntax:

{% raw %}
```markdown
![Figure 1. description of the figure](../fig/yourfigure.png)
```
{% endraw %}

To add *URL* into training we use the following markdown syntax:
{% raw %}
```markdown
[description of the URL](https://URL)
```
{% endraw %}

To add tables in markdown syntax we use `|` symbol to indicate column dividers, and `--` for table headers:

{% raw %}
```markdown
|       | Obs1 | Obs2 | Obs3 |
|------ |--------------------|
| row1  | 0    | 1    | 2    |
| row2  | 1    | 2    | 3    |
| row3  | 2    | 3    | 4    |
```
{% endraw %}

To add challanges or highlight content boxes we use the following markdown syntax:

{% raw %}
```markdown
> <type​-title>title</type​-title>
> description
{: .type}
```
{% endraw %}