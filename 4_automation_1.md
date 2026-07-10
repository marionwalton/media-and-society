---
layout: home
title: 04. GenAI - automating media production
---
# GenAI & automated media production
{: .no_toc }

*By Marion Walton, University of Cape Town*

If you’ve used a chatbot such as ChatGPT (OpenAI), Meta AI, Copilot (Microsoft), Claude (Anthropic), if you’ve used Gemini (Google) for search, or Canva AI, DaVinci AI, Dall-E or Midjourney to generate synthetic images and video you’ve interacted with **[Generative Artificial Intelligence](definitions.html#generative-ai) (GenAI) models**. 

GenAI usually takes the form of a chat interface to a statistical model, which returns responses (e.g. text, images, videos) to user **prompts**. These interactions are a type of automated media production.

This chapter provides an introductory explanation of how the models and systems underlying **Generative AI** 
 are used to create synthetic media and briefly addresses questions about . 

- TOC
{:toc}

### What is GenerativeAI?

The term "Artificial Intelligence" (AI) refers to a wide range of technologies and the term is used very loosely, often for marketing purposes ([Bender, 2026](definitions.html#bender_2026)). For now we'll focus on defining Generative AI and explaining how GenAI systems work, since these technologies are highly relevant to you as a student in Media Studies. 

{: .definition}
Generative AI are computational systems which respond to prompts from users as **input** (text and various forms of digital media) and produce synthetic media **output** (such as digital text, images, videos, audio, and software code) using **generative (statistical) models**. 

[Generative AI](definitions.html#generative-ai){: .btn .btn-blue }

### How do generative models work?

#### Large language models
The generative models in chatbots which produce synthetic text are known as Large Language Models (LLMs) which work by predicting the most likely words to follow your prompt, based on patterns recorded in a statistical model created from billions of human-created sources (such as online news articles, Wikipedia, social media posts etc). 

#### Whose language?
Despite the fact that so many sources have been used to train LLMs, the training data and consequently the linguistic patterns LLMs reproduce are dominated by English and other "high resource" languages (languages which are well represented online).  African languages, although they comprise 30% of spoken languages, are far less well represented online or in digital resources used for natural language processing ([Matsilele & Tshuma , 2025](references.html#matsilele_2025)), thus missing the practices and perspectives of African language speakers. 
 
#### Visual models
While language models predict the most likely next word, visual models predict the most likely pixel based on patterns they've encoded from downloading and processing many online photographs and artworks. This visual data is matched with the prompts that users enter. 

Multimodal means that a model processes text, image, and audio. Multimodal prompting combines LLMs and visual models. Multimodal GenAI systems encode verbal user prompts using statistical models created from sources such as the labels of large collections of online images. The output images are composite patterns of pixels which the model associates with labels similar to the encoded user prompt. 

As we've already learned, this output is known as synthetic media. Once you understand how GenAI works, you should find it easier to evaluate whether and when to use a text, image or video which is synthesized with GenAI.

[Synthetic media](definitions.html#synthetic-media){: .btn .btn-blue }

### Generative AI, academic work and sources

Relying on chatbots for academic work without verifying their output has serious drawbacks. 

Chatbots are not designed to show accurately the sources of the information they synthesize. The case studies we've already discussed show us that their responses have a highly confident tone but are often prone to serious factual errors. We'll also look at case studies showing how they tend to reproduce biases and dominant ideologies of the societies that produce them. Because language reflects and perpetuates many social inequalities chatbots may in fact exacerbate social biases present in the training data.  

In particular it's important for you to know that if you use Generative AI to generate citations, the model synthesizes likely-looking sources which follow the pattern of the references in its training data. Some models are trained to please you at all costs, and so the fabricated references they offer you may not exist at all.

If you make a habit of using GenAI to speed up your work, you're less likely to learn to read quickly, widely and with an eye for detail, and to develop your ideas as you write. This can have negative effects on your learning and may leave you deskilled when you need to work without GenAI.

As you learn more about the political economy of digital media and the revenue models of the GenAI industry, you'll understand that relying too heavily on GenAI at the cost of developing your own skills and knowledge leaves you in a vulnerable position when popular chatbots inevitably increase their prices. 

> “We see a future where intelligence is a utility, like electricity or water, and people buy it from us on a meter,” [Sam Altman, CEO of OpenAI](https://x.com/TheChiefNerd/status/2032012809433723158). March 11 2026 at the BlackRock 2026 Infrastructure Summit in Washington, D.C.  

### Prompting

In future courses, we'll study techniques for prompting. The more you know about a subject, the more you have command of the specialised language used for prompts, and the easier it is to evaluate GenAI output using your own knowledge of the topic.

For now, it's important to remember that, when prompting a model, any information you provide (including highly personal information) is being harvested by the system to create a model of you. You should also not upload copyrighted material such as published articles as part of your prompt. Many people accidentally publish their interactions, which leaves their chats exposed.

### Provenance
Think of [synthetic media](definitions.html#synthetic_media) as a kind of linguistic or visual average of what is in the training data (media which other people have created and posted online). 

In academic and many other contexts, we need to know where media and ideas come from, not only to avoid plagiarism, but also to be aware of the different contexts in which ideas arise and have been used. This is known as provenance. 

Provenance requires transparency regarding the origins and operations of information. Academic referencing is one system of establishing provenance. Provenance goes beyond the basic information usually included in citations (author, date, publisher etc), but also identifies where a media text has "travelled",  and how it is used in these contexts. 

Provenance is particularly important for synthetic media and Generative AI, since LLMs often don't reveal these details at all. If the dominant perspective becomes your default or only source,you are likely missing out. You are surrounding yourself with primarily Western ideas and are unlikely to encounter decolonial perspectives or alternative approaches.  

#### Retrieval Augmented Generation 

As discussed in the case study of synthetic media, Retrieval Augmented Generation (RAG) is used by search engines in AI mode (e.g. Google's Gemini) in order to provide an overview which links to probable sources (websites) and to access recently updated information. 

RAG is also used on academic platforms, where models are trained on peer reviewed sources such as academic journal articles not available to commercial chatbots.  

RAG combines information retrieval (which matches your query to a specific article or website) and then uses a LLM to synthesize a response, which takes the form of a likely "answer" to your question.  While RAG can link you to sources which probably address your query, you still need to verify the response carefully, consider the language you're using in your prompt, check the linked sources to see what they actually say, consider whether you trust them, and (most difficult) think carefully about what information might **not** be reflected in the synthetic output.

RAG makes information retrieval easier in comparison to trawling through a number of matches to a query, nonetheless the engine is filtering and synthesizing a relatively small number of sources, while the information or perspective you need might be in a totally different source, or might not exist online at all.

## What is a GenAI model?

A GenAI model (e.g. LLM or GANS) models a training dataset. When we use the word "model" in this way, we mean a **statistical model**, which is not an exact replica or copy of the training dataset. Instead, it's intended to be used to synthesize data from the training dataset to generate similar texts and images to those included in the training data. 

## Large Language Models 
{: .definition}
Large Language Models include OpenAI’s ChatGPT, Google’s Gemini, Anthropic's Claude and Meta’s Llama. LLMs are trained on massive collections of text, are able to generate lengthy plausible sounding text answers and simulate convincing conversations fluently. 

### Training data
The text used to build a language model is known as the model's **training data** since it provides the source material which the model will use to synthesise and output text. 

Such training data is copied from online sources such as Wikipedia, and (usually without permission) from digital versions of books and websites.  

### From text to numbers

The text from the training data is broken up into tokens (in simple terms, a token is a word or a part of a word), which is converted to numbers (known as an embedding). 

When the user generates a text prompt, the prompt is also tokenised and converted to numbers. These numbers are then matched with numbers from the training data.

### Finding the most probable next word

During a process known as pre-training, a transformer powers the model to answer the following question: 

	"What is the most probable next word/token that will follow this input?". 

Statistical **probabilities** are used to work out which word/token should come next in the output text. 

Transformers capture **contextual information** i.e. the relationships between the words/tokens in the prompt (the co-text). This technique helps to ensure that synonyms are not confused e.g. [river] bank vs. bank [account]. 

Finally the numbers are converted back to words and the model outputs a text signifier (response to the user's prompt).

LLMs are good at copying the textual patterns in writing. Their output requires verification, and they should not be used where accuracy is important.

{: .activity}
![Activity](img/pencilpencil.svg) Try out this [Transformer Explainer](https://poloclub.github.io/transformer-explainer/) to get a feeling for how the text prediction works ([Poloclub Transformer Explainer, nd](https://poloclub.github.io/transformer-explainer/)). Try varying pronouns e.g. "He trained as a ..." "She trained as a ..."

## Multimodal LLMs

Multimodal LLMs can generate text as well as images and other forms of media. 

### Training data

GANS and Diffusion image generation models collect huge datasets of text-image pairs (e.g. images and their descriptions copied from the web) as their training data. Various models are trained on different types of image data e.g. Midjourney is notorious for having been trained on artworks without permission.

### Image -> numbers <- text description
These types of models are trained to convert an **image and its text description** into similar numbers. 

### Prompt -> numbers -> image
When prompted with a text prompt, the model converts the text prompt into numbers (much as an LLM would), and then generates visual signifiers which are a numeric match for the prompt.

Synthetic images are superficially cohesive because GenAI models reconstruct their training data. Generating logical coherence in images is challenging (e.g. differentiating between a left and a right arm).

![Activity](img/pencilpencil.svg) Try out this Image generation [Explainer](https://poloclub.github.io/diffusion-explainer/) to get a feeling for how a multimodal LLM works  ([Poloclub Diffusion Explainer, nd](references.html#poloclub_diffusion_nd)). Try varying the prompt.

## Problems with models
Models can be biased, erroneous or harmful  when the data used to train them comes only from one hegemonic cultural group or gender. 

As a simple example of bias in a model, clothing manufacturers work with models of human body shapes and sizes so that the  clothing they sell is likely to fit children at different ages or people of different sizes. Some children will not fit into the clothing manufactured for their age group, some adults need to buy children's sizes and certain kinds of fashion are not even made in “plus size” ranges. 



