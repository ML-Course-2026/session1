# Week 1:  TX00EX91 - Machine Learning


### Announcements

- Zoom Recordings

<!--
https://opinto-opas.metropolia.fi/88094/en/67/70331/3638/2650/62718

The ML portion of the course is worth 3 credits, and each credit corresponds to an estimated workload of 27 hours. This includes in-class sessions, assignments, and group project work.
In the first session, we will form project groups. It is highly recommended that groups aim for diversity and shared objectives, rather than being based solely on friendships. A diverse group fosters creativity and collaboration, which are key to success in machine learning projects. If you already have a group with shared objectives, please feel free to send me an email in advance.
-->

---

### Tentative Timeline

- Week 1
  - Course Intro: Why, How, What, Group Formation
  - Break (~15min)
  - Mini lecture: Colab, Python Basics, Project Brainstorming
  - Group activity
- Week 2-7
  - Mini lecture (~35min)
  - Group activity + Break (50min)
  - Mini lecture (~35min)
  - Group activity (~35min)
- Week 8
  - Group Presentations
  - Break (~15min)
  - Group Presentations
  - Break (~15min) ...  




<!-- 
The ML portion of the course is worth 3 credits, and each credit corresponds to an estimated workload of 27 hours. This includes in-class sessions, assignments, and group project work.

In the first session, we will form project groups. It is highly recommended that groups aim for diversity and shared objectives, rather than being based solely on friendships. A diverse group fosters creativity and collaboration, which are key to success in machine learning projects. If you already have a group with shared objectives, please feel free to send me an email in advance.
-->

---


> [!NOTE]  
> We’ll be using [Google Colab](https://colab.research.google.com/), so please make sure to register with a personal Gmail account. Otherwise, you won’t be able to obtain the API key needed in Week 5.

---
### Part 1: About the course

- Why?
  - LLMs: Custom vs Proprietary
  - [Ollama](https://ollama.com/)
- What ?
  - [Course Mechanics](./material/about-course.md)
- How?
  - [Vibe coding](https://en.wikipedia.org/wiki/Vibe_coding) e.g. using [Bing Copilot](https://copilot.microsoft.com) vs [LLM as typing assistant](https://en.wikipedia.org/wiki/Vibe_coding#cite_note-:3-1)
  - [Group Formation](./material/teams.md) 
  - Mini Projects: Details will be provided later
- Big Picture
  - Finnish Industry & Custom LLMs
  - AI Agents, RAG etc. (Out of Scope)
- Activities:
  - [Activity 0 (Optional)](./material/activity0.md)
  - [Activity 1](./material/activity1.md)


> When it comes to defining what exactly constitutes vibe coding, [Simon Willison](https://arstechnica.com/ai/2025/03/is-vibe-coding-with-ai-gnarly-or-reckless-maybe-some-of-both/) makes an important distinction: "If an LLM wrote every line of your code, but you've reviewed, tested, and understood it all, that's not vibe coding in my book—that's using an LLM as a typing assistant." Vibe coding, by contrast, involves accepting code without fully understanding how it works.

---

### Part 2: Generative AI - Timeline

- History of AI (draw.io)
- [ML vs DL vs AI](https://www.ibm.com/think/topics/ai-vs-machine-learning-vs-deep-learning-vs-neural-networks)
  - [NN vs DL](./material/ml.jpg)
  - NN (on/off) vs human brain (Continuous)
- [BloombergGPT](https://www.bloomberg.com/company/press/bloomberggpt-50-billion-parameter-llm-tuned-finance/)
- Alpaca
  - [Website](https://crfm.stanford.edu/2023/03/13/alpaca.html)
  - [​​How Stanford researchers attempted to make a new ChatGPT with less than $600](https://stanforddaily.com/2023/04/02/how-stanford-researchers-attempted-to-make-a-new-chatgpt-with-less-than-600/)
  - AI Alignment: [src 1], [src 2], [src 3]
  - [LLaMA](https://ai.meta.com/blog/large-language-model-llama-meta-ai/)
  - [Llama 2](https://ai.meta.com/blog/llama-2/), [Llama 3](https://ollama.com/library/llama3.3)
  - [Deepseek R1](https://ollama.com/library/deepseek-r1)
  - OLMo family: [www](https://allenai.org/),[GitHub](https://github.com/allenai)
  - [ Mistral AI](https://github.com/mistralai)
  - [S1: The $6 R1 LLM](https://arxiv.org/abs/2501.19393)



### Part 3: Types of ML Systems

- Machine Learning vs Deep Learning vs Generative AI
- ML systems fall into one or more of the [following categories] based on how they learn to make predictions or generate content:
  - [Supervised learning]
    - Regression
    - Classification
  - Unsupervised learning
  - Reinforcement learning

### Part 4: Tools

- [Google Colab](https://colab.research.google.com)
  - [Create colab](http://colab.research.google.com/#create=true)
  - Markdown: [Intro](https://colab.research.google.com/notebooks/markdown_guide.ipynb), [Basic Syntax](https://www.markdownguide.org/basic-syntax/)
- [Activity 2](./material/activity2.md)
- [Activity 3 (Optional)](./material/activity3.md)

---

### Homework Assignments

1. **Python Review**: Please choose **one** of the following videos. This will help you refresh your Python skills and ensure you're ready for the upcoming machine learning concepts.
  - Beginners: [Learn Python - Visually Explained](https://www.youtube.com/playlist?list=PL8HmoRTjTSlEgS2GsFaDr9zDLC1xD9FZf) 
  - Intermediate: [Python Full Course for free](https://youtu.be/ix9cRaBkVe0) 

2. **Google Colab**:
   - Beginners: [ Google Colab for Python Beginners - Visually Explained  (8 min)](https://youtu.be/5sgJsCah9bs)
   - Intermediate [Google Colab Tutorial (18 min)](https://www.youtube.com/watch?v=JJYZ3OE_lGo)

2. **Watch the Following Videos**:
   These videos provide insights into the future of AI and its impact on the labor force.
   - [ Andrew Ng: Building Faster with AI (44 min)](https://www.youtube.com/watch?v=RNJCfif1dPY)
   - [ Andrew Ng: AI Won’t Replace Workers. It Will Redesign Work (12 min)](https://www.youtube.com/watch?v=5p248yoa3oE)
   - [Career Advice in AI](https://www.youtube.com/watch?v=AuZoDsNmG_s&t=1151s)
   <!-- -  [The future of intelligence | Demis Hassabis (Co-founder and CEO of DeepMind)](https://www.youtube.com/watch?v=PqVbypvxDto)  -->





<!-- Links -->
[src 1]:https://arxiv.org/abs/2309.15025
[src 2]:https://openai.com/research/instruction-following
[src 3]:https://arxiv.org/abs/2203.02155
[following categories]:https://developers.google.com/machine-learning/intro-to-ml/what-is-ml
[Supervised learning]:https://developers.google.com/machine-learning/intro-to-ml/supervised


<!-- 

> [!NOTE]  
> Highlights information that users should take into account, even when skimming.

> [!TIP]
> Optional information to help a user be more successful.

> [!IMPORTANT]  
> Crucial information necessary for users to succeed.

> [!WARNING]  
> Critical content demanding immediate user attention due to potential risks.

> [!CAUTION]
> Negative potential consequences of an action. 

-->