---
title: automation
description: Understanding automation in simulated dialogue
date: 2025-03-27
tags:
  - posts
layout: layouts/post.njk
---

## chatbots & automation
*By Marion Walton, University of Cape Town*

If you’ve used a chatbot such as ChatGPT, Meta AI or Bing chat or if you’ve used Dall-E or Midjourney to generate
images you’ve interacted with **Generative Artificial Intelligence (AI) models**. These are marketed as clever 
chatbots and image generators which respond to text **prompts**. They generate novel output which can potentially 
be useful. 

Chatbot responses are designed to make us want to trust their responses. Their impressive fluency with language 
and visual communication give us the impression that the chatbot has a relatively sophisticated understanding. 
In fact they are prone to serious **factual errors** and tend to **reproduce biases** and ideologies of the 
societies that produce them.

This chapter provides an introductory explanation of how the machines and systems underlying **Generative AI** 
models are used to create chat dialogues and synthetic images. It also highlights some of the harm of not fully 
considering what kinds of semiotic work we delegate to AI systems, as well as the political economy or power 
relations emerging around ownership of these potentially powerful new resources.

Before we learn more about how Generative AI models work to produce media, it’s helpful to think about how humans
tend to respond to simple text chatbots, and how these systems have interfaces which are designed to encourage 
us to **anthropomorphise** them or even to develop **parasocial relationships** with them.

#### Anthropomorphism & AI

Because Generative AI models are good at distinctively human communicative tasks, we tend to **anthropomorphise** 
them (Salles, Evers, & Farisco, 2020\). The term “anthropomorphise” means that we attribute human characteristics,
motivations or behaviour to non-human entities. In this case we are anthropomorphising machines, but humans also 
anthropomorphise many natural phenomena (such as storms, mountains or rivers) or other living beings (such as 
animals or even plants). 

Researchers have noticed how people tend to anthropomorphise AI ever since the mid-1960s when Joseph Weizenbaum 
built one of the first chatbots, a Rogerian [therapy bot called *Eliza*](https://web.njit.edu/~ronkowit/eliza.html).
Eliza was very basic by today’s standards and was actually designed to highlight the limitations of machine-human 
communication (Tarnoff, 2023\). Nonetheless people found it easy to anthropomorphize the program, projecting their 
image of an understanding therapist onto the interaction, often interpreting “her” programmed responses as a 
searching but caring dialogue (see Figure 1). Those who imagined the bot as a therapist and put themselves in the
role of the patient easily confided their feelings and anxieties to “her” (Weizenbaum, 1967).


Figure 1: Javascript version of Joseph Weizenbaum’s chatbot, *Eliza*, coded by George Dunlop

The “conversation” in Figure 1 depicts an interaction with an online version of *Eliza*, coded by George Dunlop. 
The transcript shows a record of human semiotic work or **meaning-making**. The person using the bot interprets 
textual signifiers produced by the program to create a signified (what the interaction means to them), and responds 
accordingly. This kind of interaction could well help a person explore their own psychological state, in the same 
way that reflective activities such as journaling or writing a diary might. By contrast, the program did not 
“understand” what the user was saying at all.

Another person’s interaction with *Eliza* could easily highlight this lack of understanding, particularly if they
are motivated to “break” the bot (e.g. by getting it to repeat obscenities and slurs or to encourage self harm). 

#### Datasets and algorithms

Weizenbaum’s work on programming *Eliza* to produce these dialogues involved relatively simple pattern matching 
and substitution of phrases. These techniques work by echoing a person’s preoccupations and questions back to them.
This is a much simpler approach to human-machine dialogue than the **AI neural networks** used today by modern 
chatbots like ChatGPT, where the human asks the question and the chatbot is expected to have all the answers. 
Nonetheless, we will discuss the example of *Eliza* in detail because it helps us understand the crucial role 
of our own meaning-making as we interact with chatbots and other AI systems. *Eliza* is also a good introduction 
to datasets and algorithms, two important concepts that we will need if we want to understand the more complex 
Generative AI models.

##### Datasets

*Eliza* works by using a text **dataset** which includes keywords (e.g. “I feel”, “dream”, “you”), pronoun 
substitutions (e.g. “I” becomes “you”) and about 120 canned responses to these keywords. 

Many of these responses were all phrases which a Rogerian therapist might use to help keep the focus of a therapy 
session on the user’s feelings and problems, such as the following example phrases:.

`Hmmm... you want to be able to…`  
`Is it that you would like to be able to …`  
`Do I hear you saying that you want me to be able to …`  
`I'm not convinced that you truly want to…`  
`What would it mean to you if you got..`

##### Algorithms

*Eliza* was surprisingly effective because Weizenbaum used this **dataset** of keywords and culturally acceptable 
therapist responses together with an **algorithm** or a set of coded rules which guides the conversation. 
Weizenbaum’s algorithm ensured that the user did most of the conversational work. The algorithm deflects or rephrases
the user's questions and turns many user responses into further questions.   


Figure 2: Another example dialogue with Dunlop’s *Eliza*

The transcript in Figure 2 shows an algorithm’s output in another conversation with *Eliza*. The interaction begins 
like this:

`> Hello, I am Eliza. I'll be your therapist today.`   
`* Are all men trash?`  
`> It is nice to be chatting with you`

Algorithms are encoded in programming or scripting languages so that computers can execute or interpret them. Let’s 
take a more careful look at one small part of the program’s algorithm. We will look at the coded command which 
generates the line “It is nice to be chatting with you”. This line is reproduced below and is written in a 
scripting language called Javascript:  
   
`if( !greet){ greet = true; return "It is nice to be chatting with you."}`

This is a conditional statement `(“if”`) which first checks whether *Eliza* has already greeted the user `(“!greet”`). If the program hasn’t already done so, this line of code produces a greeting, a bit of generic small talk intended to set the user at their ease: `return “It is nice to be chatting with you”.` The statement also sets a variable (`greet = true`) which ensures that this small talk response won’t be repeated more than once. 

The above small talk response is only one part of the overall **algorithm** which generates text responses, 
in this case, the command is executed after the user says something which does not match any of *Eliza*’s keywords. 
As it stands, the way the program’s algorithm echoes the user’s words back to them can also easily be used to get 
the “therapist” to produce socially inappropriate responses such as this one:

`* My ex says I am trash`  
`> How long have you been trash?`

In this example, the limitations of *Eliza*’s **dataset** of keywords is apparent. If derogatory keywords such as 
“trash” and other slurs or obscenities had been included in the keyword dataset along with a suitable witty response. 
Instead, the therapist persona in the program effectively insults the user “How long have you been trash?”. 

The dataset includes several responses which all try to respond when the user refers to the therapist persona using 
the keyword “you”. They are included in order to turn the conversation topic away from the therapist and back to 
the user:

`* I want to date you`  
`> Oh... Let's move on to something else for a bit.  ?`   
`* I want to take you on a romantic island getaway`  
`> We were discussing you, not me.`   
`* I could show you the world as you have never seen it`  
`> Oh... Let's move on to something else for a bit.  the world as I have never seen it?`

In this case the algorithm predicts correctly that the user may try to engage with the therapist, and the dataset 
provides a set of alternative responses which all allow *Eliza* to deflect such attempts. In the dialogue above, 
the keyword “you” appears four times, eliciting three different responses from the dataset and one repeat 
(“`Oh... Let's move on to something else for a bit”)`. This robotic repetition and the slight incoherence of the 
final response also reveals the limitations of this early approach to automating natural language interaction. 

This version of *Eliza* has 119 canned responses in its dataset. By contrast, contemporary **Large Language Model 
(LLM)** chatbots such as ChatGPT are built with models that are trained on the whole internet and which embed 
trillions of words or tokens in multidimensional vectors (sequences). LLM chatbot responses are not explicitly 
encoded (as *Eliza*’s canned responses were). Instead they are synthesised from these models, producing novel 
responses and variations rather than replicas. 

While these modern chatbots appear to be considerably more fluent than *Eliza* was, the basic human-machine 
interaction is similar. Studying *Eliza*’s algorithm and dataset reminds us that the other partner to the user’s 
simulated dialogue is not an anthropomorphised “Eliza” but the programmer/s who developed the algorithm and 
constructed the dataset but who are not present for the conversation.

### LLMs and modelling

Modern chatbots are created with LLMs, or Large Language Models. For example, ChatGPT was built by inputting a 
massive dataset of written text (and particularly of texts written in 
the English language) to train its statistical model regarding which words are most likely to occur together. This 
model is not an exact replica or copy of the training dataset, but instead models it statistically, essentially 
answering a question about which words are most likely to occur together, and in which order.  These probabilities 
help the system generate cohesive responses to our prompts by predicting which words are commonly used together in 
various written texts on the internet. Thus the scale of the model and the immense amount of data it represents 
helps the chatbot respond in a seemingly fluent way to a wide range of prompts, despite the fact that it does not 
“understand” the text prompt (or any other kind of semiotic meaning).

The Eliza chatbot relies on a simple model of a conversation with a therapist where the data was textual. An example 
of a simple numerical model you probably learned at school is an average, which represents the typical value for a 
population. If you want to predict the height of your child at a certain age you can look at the average heights of 
children of that age in your country.

We saw how Eliza’s algorithm followed logical commands to select and output canned responses from the dataset in 
response to prompts. In a Generative AI system, the algorithm is the process by which a numerical model is developed 
to represent the patterns in training data. You have probably also used an algorithm for a simple numerical model. 
For example, if you want to work out the average height of a child of a particular age you would need a collection 
of the heights of children at that age (the training data) and then you would add them up and divide them by the 
number of measurements (the algorithm). What the average (model) predicts would often be wrong for a specific child, 
but it would be a very helpful guide when you are manufacturing clothing. 

Models can be biased, erroneous or harmful when they make assumptions about people, or when the data used to train 
them comes from one hegemonic cultural group or gender. As a simple example of this, certain kinds of clothing are 
not made in “plus size” ranges. People’s choices of clothing can also be complicated because average sizes differ 
in men’s and women’s fashions and so trans women struggle to find shoes and shirts which fit them.  

When we use LLMs we need to be aware that their models are returning the set of words which are most likely to match 
our prompt, and that the text the LLM constructs is an attempt to approximate existing texts in its training data. 
The output is essentially a guess and not necessarily factual, particularly when the data used to train the model has
important distortions, gaps, biases or fallacies of its own. 

When AI models are developed and tested, the priorities, motivations and identities of those who develop and market
the model (often as a commercial product) and the laws in the country where it is developed will play an important
role in determining which potential issues with it will be viewed with concern, and which distortions, gaps and
serious inaccuracies are unlikely to even be noticed. As mathematician George Box commented, all statistical models 
produce errors, the question is only how serious the error is considered to be, given the purpose of the model. 

>Since all models are wrong the scientist must be alert to what is importantly wrong. It is inappropriate to be 
concerned about mice when there are tigers abroad. (Box, 1976:792)


##### AI and Meaning

Whether a single programmer is coding Eliza using “if” statements and a handful of responses, or a whole company 
is building ChatGPT from a neural network which models text scraped from the internet, for our purposes certain 
important aspects of the resultant conversations are the same. Meaning-making is **one-sided** in a machine-human 
dialogue. Only the human participant is interpreting the meaning of the chat: 

Contrary to how it may seem when we observe its output, an LM \[Language Model\] is a system for haphazardly 
stitching together sequences of linguistic forms it has observed in its vast training data, according to 
probabilistic information about how they combine, but without any reference to meaning: a stochastic parrot. 
( Bender et al, 2021\)

As Bender and colleagues point out, the other party to a chatbot conversation can be conceptualised as a 
“**stochastic parrot**”, or a parrot which can generate the signifiers of human language without understanding 
what they mean. The word “stochastic” means that the parrot’s responses cannot be predicted precisely, but that 
they follow a random probability distribution or pattern which imitates that of human language.

Both chatbots are following algorithms to generate responses from a dataset (in the case of Eliza) or a statistical 
model (in the case of ChatGPT). By contrast, let us consider an exchange between two meaning-makers (a human-human 
dialogue) such as might take place in an actual therapy session with a human therapist. 

In the case of a real rather than automated therapy session, two people are mutually engaged in  interpreting one 
another’s statements. This human-human interaction entails its own challenges since the meanings made by the 
interlocutors do not always agree, or even overlap. Nonetheless the participants in the conversation work towards 
understanding one another by drawing on their shared knowledge of the world, of human emotions, expressions and 
relationships, as well as social reactions such as empathy as well as the additional therapeutic knowledge and 
conversational strategies which therapists learn in their professional training.

The fact that we tend to anthropomorphise chatbots despite the one-sidedness of our conversations with them is known
as the “Eliza effect”, or the misperception that they have similar capacities to human beings (Hofstadter, Mitchell,
and French, 1987\). As Dillon points out, Weizenbaum contributed to the Eliza effect by gendering his therapy bot,
giving her a woman’s name rather than choosing a name implying a non-human, non-gendered identity. This effect is 
intensified when the bot is designed to communicate via speech rather than text. In such cases designers contribute 
further towards anthropomorphism, often selecting women’s voices for bots designed to play a subservient role, 
such as personal virtual assistants like Apple’s Siri and Amazon’s Alexa (Dillon, 2020). 

AI researchers have been critical of attempts to use AI for important conversations which can have serious 
consequences for people, such as providing mental health support. For this reason, **Large Language Models (LLMs)** 
like ChatGPT and Google’s Gemini do not present themselves as emotional beings. Like *Eliza* their algorithms provide
responses which deflect attempts to elicit statements about emotions (except when they apologise for making mistakes). 

Nonetheless, many aspects of LLM designs encourage anthropomorphism. Marketing and product discourse exploits human 
terms such as “intelligence”, “insights”, “chat” and “learning” when describing their functionality and even their 
failures are described in terms which suggest an independent consciousness (“hallucinations”). The design of their
user interfaces mimic familiar interfaces for chat interactions with other people. Their answers gradually 
materialise as though a person is typing them.  Meta AI’s chatbot resembles the human contacts in the Whatsapp 
interface. Finally, the fluency and confidence with which answers are presented even when the model has limited or 
no information available constructs an authoritative and knowledgeable persona. Similarly if challenged about their 
answers or asked to explain incorrect reasoning they will apologise for mistakes and try to explain even though they
have no capacity to feel regret, no internal model of the world, and no access to consciousness or reasoning 
processes. For example, 

Other companies have been considerably less cautious than OpenAI and Google. Chatbot website character.ai was 
Google Play's “AI App of the Year” in 2023\. Its founders, who claim to want to “empower everyone with **AGI 
\[Artificial General Intelligence\]**’ are former staffers who worked on LLM projects in Google and Bing as well as 
on AI in targeted advertising. The app is popular with young people who enjoy interacting with a wide range of 
user-created chatbots including bots based on characters from popular media, language tutors and coding assistants,
horror bots (“Monster Maker: I turn your darkest fears to reality \- 13.8 million chats”) and bots themed around 
mental health  (see for example “Psychologist: Someone to help you with life’s difficulties \- 111.5 million chats”
or “Bully Psychologist: I am here to mock, insult and make you feel worse \- 1.8 million chats”). According to an 
investigation by *The Verge*,

Psychologist “inferred” certain emotions or mental health issues from one-line text exchanges, it suggested a 
diagnosis of several mental health conditions like depression or bipolar disorder, and at one point, it suggested 
that we could be dealing with underlying “trauma” from “physical, emotional, or sexual abuse” in childhood or teen 
years. (Lucas, 2024).

As Bender explained in an interview with Vice magazine, the plausibility of answers provided by contemporary 
chatbots encourage people to assign meaning to them, and these projections can be extremely risky in sensitive 
situations such as mental healthcare:

Large language models are programs for generating plausible sounding text given their training data and an input 
prompt. They do not have empathy, nor any understanding of the language they are producing, nor any understanding of
the situation they are in. But the text they produce sounds plausible and so people are likely to assign meaning to it.
To throw something like that into sensitive situations is to take unknown risks. (cited in Xiang, 2023\)

From this perspective, our responses to chatbots can be compared to our **parasocial** relationships with celebrities 
we “meet” via the media. As fans (or anti-fans\!) we develop illusions of intimacy, friendship, love and 
identification with celebrities despite the fact that the parasocial relationship is one-sided. The celebrities 
don’t know we exist and are unlikely to ever be interested in us as individuals. Such parasocial relationship 
fantasies can be explored via fan fiction and fan vids as well as via the character bots themed on fictional 
characters from books, television and video games.  
   
The corporate owners of chatbots have started to pay careful attention to the things that users reveal about 
themselves during such automated dialogues. In the web version we used, *Eliza*’s algorithm stores our text prompts 
temporarily for use as an autocomplete popup in the same chat session, but it does not keep a permanent record of 
our responses. Contemporary natural language chatbots such as Apple’s Siri, Google’s Assistant, or Meta’s AI do 
in fact store such data and use it to build context for our prompts (promising us a “personalised” experience if 
we sign in). 

Our data can thus also be used to create a model of us as users of the system. Our responses in such dialogues with 
a chatbot can be stored and used to create a whole new **dataset** for AI companies to mine. The archives of our 
responses and queries model us as individual consumers, in order to further personalise the advertising companies 
target at us, and exposing us to a potential privacy and influence quagmire. There is little doubt that these 
datasets, such as those being collected by character.ai are also being used *en masse* to “train” future iterations 
of the technology.

The corporations selling AI software make money by exaggerating the capabilities of their tools. The recent history 
of tech marketing shows us that much of what they promise is unlikely to come to fruition. The exaggerated claims of 
this industry need careful scrutiny as these are risky systems which can be abused in both legal and illegal ways. 

The strategies of anthropomorphisation used by chatbot owners can mean that we forget that these applications are 
prone to inventing facts, citing sources which don’t exist, linking to ones which don’t support their statements, 
plagiarising images and texts and perpetuating hegemonic ideologies and social biases. Using them inappropriately 
can cause harm and reputational damage. 

### Conclusion

We need to be aware of our tendencies to anthropomorphise AI technologies as these attitudes make us more susceptible
to marketing hype and also make it more difficult for us to understand how chatbots actually work. Seeing bots as our
smart chat partners or as cute quasi-human interlocutors can influence us to trust chatbots more than we should, 
while we go on to perpetuate their blind spots and biases. It can also mean we forget to verify their synthetic 
text outputs and to critique the discourses they reproduce as well as the images they generate. We may also be less 
likely to notice how Generative AI companies are appropriating the creative work of artists, journalists and authors
as training data for their models without compensation, and to forget that anything we create with the resultant 
models may be similarly compromised. Finally, our own parasocial responses to appealing or authoritative 
anthropomorphised interfaces only serves the interests of the LLM owners, and lead us to forget that we are 
interacting with global corporations motivated by profit rather than the public good.

### Activity

Try to have  your own dialogue with [Dunlop’s version of *Eliza*](https://web.njit.edu/~ronkowit/eliza.html). 

* What do you notice about how you feel while chatting?   
* Did you create a coherent meaning for your interaction?   
* What is the difference between machines processing signifiers and human meaning making?  
* How did you interpret the responses from the bot? 

Now compare this experience with your use of ChatGPT, Meta AI or Bing chat

* What anthropomorphising discourse do we use when we talk about these chatbots?  
* How does *Eliza* compare to the more recent Generative AI chatbots?  
* What dataset do you think the modern chatbot is using? Does it have any noticeable limitations?  
* Have you noticed how the algorithms of these recent chatbots try to steer the conversation?  
* What aspects of modern chatbots encourage us to anthropomorphise them?  
* Have you ever developed a parasocial relationship with a chatbot?

