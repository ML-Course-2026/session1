# Week 1: TX00EX91 - Machine Learning

This page contains the Week 1 session overview, supporting materials, activities, and homework.


### Announcements

- Zoom recording: the link will be added after the session.

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

---

### Part 1: About the course

- Current landscape examples:
  - [Qwen CLI - Demo](https://github.com/QwenLM/qwen-code)
  - OLMo family: [www](https://allenai.org/),[GitHub](https://github.com/allenai)
  - [BloombergGPT](https://www.bloomberg.com/company/press/bloomberggpt-50-billion-parameter-llm-tuned-finance/)
- Why this course?
  - LLMs: custom models (fine-tuned or trained from scratch) vs proprietary models
  - Finnish industry and custom LLMs: adopting AI tools and domain-specific models is increasingly important for competitiveness
  - Different ways to use LLMs:
    - Inference [Ollama](https://ollama.com/)
    - Fine-tuning: [Hugging Face](https://huggingface.co/models)
    - Training: [nanochat](https://github.com/karpathy/nanochat) 
- What are we going to cover?
  - [Course Mechanics and Assessment](./material/about-course.md)
  - Mini Projects: Details will be provided later
- How?
  - [Vibe coding](https://en.wikipedia.org/wiki/Vibe_coding) e.g. using [Bing Copilot](https://copilot.microsoft.com) vs [Vibe engineering](https://simonwillison.net/2025/Oct/7/vibe-engineering/)
  - [We will work in Groups](./material/teams.md) 
- Activities:
  - [Activity 0 (Optional)](./material/activity0.md)
  - [Activity 1](./material/activity1.md)

> [!NOTE]  
> When it comes to defining what exactly constitutes vibe coding, [Simon Willison](https://arstechnica.com/ai/2025/03/is-vibe-coding-with-ai-gnarly-or-reckless-maybe-some-of-both/) makes an important distinction: "If an LLM wrote every line of your code, but you've reviewed, tested, and understood it all, that's not vibe coding in my book—that's using an LLM as a typing assistant." Vibe coding, by contrast, involves accepting code without fully understanding how it works.

---

### Part 2: Types of ML Systems (Bird's-Eye View)

- Machine Learning vs Deep Learning vs Generative AI
  - [(draw.io)](https://kodexolabs.com/what-is-machine-learning-ml/)
  - ML vs DL vs AI: [blog](https://www.ibm.com/think/topics/ai-vs-machine-learning-vs-deep-learning-vs-neural-networks), [Illustration](./material/ml-dl.jpg)
- ML systems fall into one or more of the following categories based on how they learn to make predictions or generate content:
  - [Supervised learning](https://developers.google.com/machine-learning/intro-to-ml/supervised)
    - Regression
    - Classification
  - [Unsupervised learning](https://developers.google.com/machine-learning/intro-to-ml/what-is-ml#unsupervised_learning)
  - Reinforcement learning
- Generative AI
  - Alpaca: [Website](https://crfm.stanford.edu/2023/03/13/alpaca.html), [​​How Stanford researchers attempted to make a new ChatGPT with less than $600](https://stanforddaily.com/2023/04/02/how-stanford-researchers-attempted-to-make-a-new-chatgpt-with-less-than-600/)
  - [HuggingFace](https://huggingface.co/models)
  - AI Alignment: [src 1], [src 2], [src 3]

---

### Part 3: Tools

> [!NOTE]  
> - We will use [Google Colab](https://colab.research.google.com/) for browser-based Python notebooks and access to cloud compute resources.
> - We will also use [Google AI Studio](https://aistudio.google.com/) for free API experiments, so please register with a **personal** Gmail account. Otherwise, you may not be able to obtain the API key needed later in the course.

- [Google Colab](https://colab.research.google.com)
  - [Create Colab notebook](http://colab.research.google.com/#create=true)
  - Markdown: [Intro](https://colab.research.google.com/notebooks/markdown_guide.ipynb), [Basic Syntax](https://www.markdownguide.org/basic-syntax/)
- [Activity 2](./material/activity2.md)
- [Activity 3](./material/activity3.md)

---

### Homework Assignments

1. **Python Review**: Choose **one** of the following videos to refresh your Python skills before the upcoming machine learning topics.
   - Beginners: [Learn Python - Visually Explained](https://www.youtube.com/playlist?list=PL8HmoRTjTSlEgS2GsFaDr9zDLC1xD9FZf)
   - Intermediate: [Python Full Course for Free](https://youtu.be/ix9cRaBkVe0)

2. **Google Colab**:
   - Beginners: [Google Colab for Python Beginners - Visually Explained (8 min)](https://youtu.be/5sgJsCah9bs)
   - Intermediate: [Google Colab Tutorial (18 min)](https://www.youtube.com/watch?v=JJYZ3OE_lGo)

3. **Watch the Following Videos**:
   These videos provide perspectives on the future of AI and its impact on work.
   - [Andrew Ng: Building Faster with AI (44 min)](https://www.youtube.com/watch?v=RNJCfif1dPY)
   - [Andrew Ng: AI Won’t Replace Workers. It Will Redesign Work (12 min)](https://www.youtube.com/watch?v=5p248yoa3oE)
   - [Career Advice in AI](https://www.youtube.com/watch?v=AuZoDsNmG_s&t=1151s)



<!-- Links -->
[src 1]:https://alignment.openai.com/
[src 2]:https://storage.googleapis.com/deepmind-media/gemini/gemini_3_pro_fsf_report.pdf
[src 3]:https://deepmind.google/blog/updating-the-frontier-safety-framework/



