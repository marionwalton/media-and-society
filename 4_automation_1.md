---
layout: home
title: 04. GenAI - automating media production
---
# GenAI & automating media production
{: .no_toc }

*By Marion Walton, University of Cape Town*

If you’ve used a chatbot such as ChatGPT (OpenAI), Meta AI, Copilot (Microsoft), Claude (Anthropic), if you’ve used Gemini (Google) for search, or Canva AI, DaVinci AI, Dall-E or Midjourney to generate images and video you’ve interacted with **[Generative Artificial Intelligence](definitions.html#generative-ai) (GenAI) models**. 

GenAI usually takes the form of a chat interface to a statistical model, which returns responses (e.g. text, images, videos) to user **prompts**. 

There is no widely accepted definition of "Artificial Intelligence" (AI) and the term is used very broadly for marketing purposes ([Bender, 2026](definitions.html#bender_2026)). For now we'll focus on defining Generative AI and explaining how GenAI systems work.

{: .definition}
Generative AI are computational systems which respond to prompts from users as **input** (text and various forms of digital media) and produce synthetic media **output** (such as digital text, images, videos, audio, and software code) using **generative (statistical) models**. 

Generative AI chatbots (LLMs) work by predicting the most likely words to follow your prompt, based on patterns recorded in a statistical model created from billions of human-created sources (such as online news articles, wikipedia, social media posts etc). 

Similarly, visual models predict the most likely pixel based on patterns they've encoded from downloading and processing many online photographs and artworks. 

Multimodal prompting combines LLMs and visual models. These systems encode verbal user prompts using statistical models created from sources such as the labels of large collections of online images. The output images are composite patterns of pixels which the model associates with labels similar to the encoded user prompt. 

Think of synthetic media as a kind of linguistic or visual average of what is in the training data (media which other people have created).  

This chapter provides an introductory explanation of how the models and systems underlying **Generative AI** 
models are used to create synthetic media. 

- TOC
{:toc}


## What is a GenAI model?

A GenAI model (e.g. LLM or GANS) models a training dataset. When we use the word "model" in this way, we mean a **statistical model**, which is not an exact replica or copy of the training dataset. Instead, it's intended to be used to synthesize data from the training dataset to generate similar texts and images to those included in the training data. 

## Large Language Models 

Large language models such as OpenAI's ChatGPT and Google's Gemini are created from massive collections of text data. 

### Training data
This text is known as the model's **training data** since it provides the source material which the model will use to synthesise and output text. 

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
Models can be biased, erroneous or harmful when they make assumptions about people, or when the data used to train 
them comes only from one hegemonic cultural group or gender. 

As a simple example of bias in a model, clothing manufacturers work with models of human body shapes and sizes so that the  clothing they sell is likely to fit children at different ages or people of different sizes. Some children will not fit into the clothing manufactured for their age group, some adults need to buy children's sizes and certain kinds of fashion are not even made in “plus size” ranges. 



