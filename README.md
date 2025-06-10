# 📜 prompts.py

**prompts.py** is a centralized Python module that defines reusable, well-structured, and strategically designed prompts for generative AI applications. It follows frameworks like R.A.C.E. (Role, Action, Context, Example) and A.P.E. (Action, Prompt, Expectation) to ensure prompt clarity, consistency, and high performance across tasks such as text generation, comparison, classification, summarization, and more.

---

## 🚀 Purpose

The goal of `prompts.py` is to:

- Maintain clean and consistent prompt engineering practices
- Enable zero-shot, one-shot, few-shot, and framework-based prompting
- Facilitate easy experimentation and reuse of prompt templates in AI-driven applications
- Support education, research, and production-level LLM workflows

---

## 📂 Structure

Each prompt follows a consistent schema for clarity and adaptability:

```python
{
    "name": "descriptive_prompt_name",
    "framework": "RACE | APE | TAG",
    "strategy": "zero-shot | one-shot | framework prompting",
    "tool": "ChatGPT",
    "goal": "Describe the problem this prompt solves",
    "prompt": """Full text of the prompt"""
}
```

---

🧠 **Best Practices**

- Use structured frameworks (R.A.C.E., A.P.E.) to ensure clarity  
- Include goals to track the purpose of each prompt  
- Test and iterate prompts regularly with your LLMs  
- Organize prompts by domain (e.g., education, marketing, code generation)  

---

🤝 **Contributing**

Feel free to fork and contribute additional prompt templates, framework styles, or enhancements. Prompt responsibly.

---

📬 **Contact**
Data Scientist: Heba Abdelhadi
📧 habdelhadi08@gmail.com
📍 Shelby Township, MI
📅 Capstone Project for Qwasar Data Science & Machine Learning Bootcamp

---


