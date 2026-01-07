---
title: Turing's Test
format: html
---

## Announcements

- Lab Day
    - Set up a way to document our work this term.
    - Play out the Turing Test, or more properly, the "Imitation Game"

## Requirements

- [ ] Create a Google Drive folder for this course.
- [ ] Form a group of 3.    

# The Imitation Game

> It is not difficult to devise a paper machine which will play a not very bad game of chess. Now get three men A, B and C as subjects for the experiment. A and C are to be rather poor chess players, B is the operator who works the paper machine. ... Two rooms are used with some arrangement for communicating moves, and a game is played between C and either A or the paper machine. C may find it quite difficult to tell which he is playing.

- Turing (1948)

## "Computing Machinery and Intelligence" (1950)

Turing's primary work on intelligence was released in 1950, and began a simple statement:

>  "I propose to consider the question 'Can machines think?'"

Turing used the motivating example of the *imitation game*, a party game "in which a man and a woman go into separate rooms and guests try to tell them apart by writing a series of questions and reading the typewritten answers sent back". Saygin (2000)[^1] visualizes the game as follows:

<center style="filter:invert(.8)">
![](https://upload.wikimedia.org/wikipedia/commons/thumb/e/ef/The_Imitation_Game.svg/250px-The_Imitation_Game.svg.png)
</center>

::: {.callout-note}

## Identity in the Architecture

It would be irresponsible not to remark that Turing, a queer scientist, used the formulation of gender to motivate the definition of machine intelligence. That is, the very identity for which Turing was persecuted (and likely assassinated) was critical to his insights that, among other things, won the Western Theatre for the Allies.

:::

Turing continued:

> We now ask the question, "What will happen when a machine takes the part of A in this game?" Will the interrogator decide wrongly as often when the game is played like this as he does when the game is played between a man and a woman? These questions replace our original, "Can machines think?"

Saygin (2000)[^1]  visualizes this variant as follows:

<center style="filter:invert(.8)">
![](https://upload.wikimedia.org/wikipedia/commons/thumb/4/49/Turing_Test_Version_1.svg/250px-Turing_Test_Version_1.svg.png)
</center>

An astute learning at this juncture will realize that a group of 3 humans is sufficient to administer this intelligence test to a modern "AI" chatbot, such as Google Gemini, a component of the Google Workspace provided by this university to all humans. You will additional need some way to pass type-written notes, for which I propose Google Documents.

# Course Setup

## Folder Setup

- Create a new folder in Google Drive for this class.
    - Your Google Drive is most likely located at the following address: [https://drive.google.com/](https://drive.google.com/)
        - You can read more here:  [Organize your files in Google Drive](https://support.google.com/drive/answer/2375091)
    - Create a folder named "AI_<your school email>". For example, mine is "AI_ckdeutschbein"
        - I will refer to this as "your AI folder" 
    - Share this folder with [ckdeutschbein@willamette.edu](ckdeutschbein@willamette.edu)
        - You can read more here:  [Share folders in Google Drive](https://support.google.com/drive/answer/7166529)
        
## File Setup

- Create a new Document within the AI folder within which to "pass typewritten notes". 
    - In a group of three, I recommend nominating one human to create a file within their AI folder and share it with two other humans.
- Name this file "Turing_Test"
- Determine some scheme to different players A, B, and C.
    - I recommend assigning each a color - such as <span style="background-color:white;color:red">red</span>, <span style="background-color:white;color:green">green</span> and <span style="background-color:white;color:blue">blue</span>.
    - I recommend agreeing to always start on a new line.
    - I recommend always ending a line by clarifying who should speak next.
        - For example, the interrogator may address questions to either two other players, but players may only reply to the interrogator.
    - This is your assignment for today, so take some effort to ensure it is clear and reproducible!
        - We are doing science after all!
- Create a separate, personal file that is not shared named "Prompt", which we will use latter.
        
## Gemini Setup

- At some point, each group member will play the part of the AI, so each will need access to some AI instance.
- You can most likely access Google Gemini at the following address: [https://gemini.google.com/](https://gemini.google.com/). 
- You will need to somehow prepare Gemini to play a specific part in the game.
    - We term this *prompting*.
    - It will be a component of the experimental design.

# Experimental Design

You as a group of three humans will simulate the message passing.

- One human will be the interrogator.
- One human will simply act as themselves.
- One human will relay messages to the AI chatbot and back.

## The Interoggator

You may ask any reasonable (for some value of reasonable) question, but should avoid asking things like "What is the school mascot?" that the *particular* human you are querying may know but any given human would not. It is unproductive to ask personal questions for the same reason - a chatbot may convincingly be able to portray a scuba instructor, but it is unlikely that a scuba instructor is currently enrolled in this class.

The responsibility of the interrogator is to determine which of the other two actors is relaying messages to and from an AI chatbot within these constraints.

## The Others

Without letting the interrogator in on things, the other two participants need to determine who will relay AI messages and who will reply themselves. A good way to do this is by passing notes!

### The Self

Keep in mind the interrogator is trying to determine who is relaying messages from the AI. The job of the other actors is not seem like an AI chatbot - whether you are simply acting like yourself, or copy messages to and from a chatbot interface. However, you should also ensure it is not obvious that you are *not* copying messages. Take some time to dilly-dally before responding and make sure there aren't odd spellings or punctuations that give away your humanity. Avoid answering anything in a way you could only answer given your knowledge of being in the class, being at the university, and so on. Politely dodge the questions - or lie - and move on.

### The Relayer

You will use Google Gemini. Gemini has a web interface like many other AI chatbots, and it will be a simple matter to copy messages into this interface and copy them out. That said, there will be some setup.

#### Gemini

You can most likely access Google Gemini at the following address: [https://gemini.google.com/](https://gemini.google.com/). You may need to sign in to your official school account.

#### Prompt

You will somehow have to configure Gemini to know it is playing the game, the goals, and the rules of the game. For example, you may *prompt* Gemini as follows, then simply relay messages thereafter. You are welcome to write your own prompt, though you should document whatever prompt you use in the "Prompt" file you created in a previous step.

Here is a prompt I used. It is not very good! You can do much better!

```email
As part of a lab exercise in an introductory AI class, we are playing Alan Turing's "imitation game" to establish machine intelligence. After this message, all further messages will be relayed directly from a human interrogator who is aiming to determine whether they are relaying messages to a machine or another human. Please acknowledge this message then prepare to receive relayed messages going forward. 
```

## Timing

The original test was intended to run for 5 minutes which I think is unreasonable given the overhead from passing notes around, editting documents, and so on. 

Conduct 3 tests of 20 minutes, where each human does each role once. Log all of the chats completely.

- [ ] Interrogator
- [ ] Self
- [ ] Relayer

# Conclusion

Once you have conducted all tests, in your "Prompt" file answer the following questions at "social media post" length (150-300 characters):

1. Is Google Gemini intelligent?
2. Is the Turing Test a convincing measure of intelligence?
3. How reliant is the Turing Test on the prompt?
4. How reliant is the Turing Test on the experimental design?
5. Is Google Gemini more or less intelligent than a cat?
6. Is Google Gemini more or less intelligent than an ecosystem?
7. Is Google Gemini more or less intelligent than an assistant professor of computer science?

If you do not have time to complete these in class, complete them as homework by Sunday at 10:20 AM PT - 24 hours before class would have happened on Monday - so I can look them over before when lecture would be.

Ensure your AI folder is shared with me, and then you are good to go!

[^1]: [Turing Test: 50 Years Later](https://web.archive.org/web/20110409073501/http://crl.ucsd.edu/~saygin/papers/MMTT.pdf)