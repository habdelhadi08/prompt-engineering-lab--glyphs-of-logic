
'''"""
Description:
This file includes multiple prompt engineering examples using different frameworks:
- R.A.C.E (Role, Action, Context, Expectation)
- A.P.E (Action, Prompt, Expectation)
- T.A.G (Task, Action, Goal)

Each example includes the prompt, the LLM's response, and observations.
"""

# ========================================
# Framework 1: R.A.C.E
# ========================================

"""
Framework: R.A.C.E (Role, Action, Context, Expectation)
Prompt Strategy: Zero-shot
Tool Used: ChatGPT (GPT-4o)

Goal: Generate a comparison table of generative AI models by modality.
"""

prompt= """
Role: "Imagine you are a domain expert in generative AI."

Action: "Please provide a comparative analysis of different types of prompts."

Context: "we are building a resource to help developers and learners quickly understand the differences between zero-shot, few-shot, and framework prompting techniques."

Expectation: "Return a concise table that includes each model type, its main advantages, disadvantages, and a few real-world application scenarios."
"""

response= """
Certainly! Here's a concise comparative table of Zero-Shot, Few-Shot, and Framework Prompting techniques in generative AI:
| **Prompting Type**      | **Description**                                                                                | **Main Advantages**                                                                                    | **Main Disadvantages**                                                 | **Real-World Application Scenarios**                                                            |
| ----------------------- | ---------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| **Zero-Shot**           | No examples provided; model generates output based on prompt alone.                            | - Quick and easy to use<br>- No need for labeled examples<br>- Flexible for many tasks                 | - Often less accurate<br>- May misunderstand complex tasks             | - Simple Q\&A<br>- Translation<br>- Summarization where no training examples are available      |
| **Few-Shot**            | Provides a few example input-output pairs in the prompt to guide the model.                    | - Better accuracy than zero-shot<br>- Adaptable with minimal examples<br>- Can specify style or format | - Requires careful example design<br>- Limited by prompt length        | - Custom classification<br>- Code generation<br>- Structured data extraction                    |
| **Framework Prompting** | Uses a structured or layered prompt strategy (e.g., chain-of-thought, step-by-step reasoning). | - Enables complex reasoning<br>- Improves interpretability<br>- Can break down multi-step tasks        | - More complex to design<br>- Longer prompts increase latency and cost | - Multi-step math problems<br>- Legal reasoning<br>- Complex instructions with reasoning chains |
Would you like me to expand on any of these or provide example prompts?
"""

# Observation: The model accurately structured a comparative table with minimal prompt detail.

# ========================================
# Framework 2: A.P.E
# ========================================

"""
Framework: A.P.E (Action, Purpose, Expectation)
Prompt Strategy: One-shot
Tool Used: ChatGPT (GPT-4o)

Goal: Help a high student graduate to decide which is engineering school has the best porgram in Detoit, Michigan.
"""

prompt= """
Action: "Explain the advantages and disadvantages of engineering schools in Detroit, Michigan."

Purpose: "You are a senior engineer who was born and raised in Detroit, Michigan. You have a lot of experience with the engineering schools in the area."
Expectation: "Provide a brief overview of the top engineering schools in Detroit, including their strengths and weaknesses."
"""

response= """
Got it! Speaking as a senior engineer from Detroit familiar with the local engineering education scene, here’s a quick overview of the top engineering schools in the Detroit metro area:

1. University of Michigan – College of Engineering (Ann Arbor)
Strengths:

Consistently ranked among the top engineering schools nationally.

Strong research programs across multiple disciplines — automotive, aerospace, electrical, computer, and mechanical engineering.

Excellent industry connections, especially with Detroit’s automotive and tech sectors.

Vast alumni network and strong career placement.

Weaknesses:

Located in Ann Arbor, about 45 minutes from Detroit, so not exactly in the city.

Highly competitive admissions.

Large size can sometimes make personalized attention more challenging.

2. Wayne State University – College of Engineering
Strengths:

Located right in the heart of Detroit, offering great access to local industry, especially automotive suppliers and startups.

Strong focus on urban engineering challenges, including sustainability and infrastructure.

Offers cooperative education (co-op) programs linking students directly to Detroit employers.

Diverse student body reflecting the city’s demographics.

Weaknesses:

Smaller research funding compared to UM.

Facilities are good but not as modern or expansive as some peer institutions.

Perception challenges due to Detroit’s economic history, though this is improving.

3. Lawrence Technological University
Strengths:

Strong emphasis on practical, hands-on learning with smaller class sizes.

Known for programs in automotive engineering and robotics.

Close ties with Detroit’s automotive industry and engineering firms.

More accessible admission process for local students.

Weaknesses:

Smaller institution, so fewer resources compared to UM or WSU.

Less research focus, more teaching oriented.

Less recognized nationally but highly respected regionally.

4. Michigan State University – College of Engineering (East Lansing)
Strengths:

Solid engineering programs with a good balance of research and teaching.

Strong in civil, mechanical, and electrical engineering.

Growing reputation in sustainable and environmental engineering.

Weaknesses:

Located about 90 minutes from Detroit, so less direct local industry interaction.

Less specialized in automotive compared to UM or Lawrence Tech.

Summary
If you want top-tier research and prestige, UM Ann Arbor is the clear leader, but it’s a bit outside the city. For direct Detroit access and urban-focused engineering, Wayne State is the go-to. Lawrence Tech offers great hands-on experience with strong industry ties, especially in automotive. MSU is solid but less Detroit-centric.

If you want, I can also share insights on student life, scholarships, or career support at these schools!
"""

# Observation: By writing only a two-line prompt, the model gave me detailed advantages and disadvantages of each school..

# ========================================
# Framework 3: T.A.G
# ========================================

"""
Framework: T.A.G (Task, Action, Goal)
Prompt Strategy: Few-shot with role
Tool Used: ChatGPT (GPT-4o)

Goal: Extract key themes from a user review for a wine app.
"""

prompt = """
Task: "Analyze the advantages and disadvantages of using AI in general"

Action: Return 3 adavantages of disadvatages of using AI.

Goal: We want to identify common reasons why we should or shouldn`t use AI.
"""

response= """
Here are three common advantages and disadvantages of using AI, based on practical and ethical considerations:

✅ Advantages of Using AI:
Increased Efficiency and Automation
AI can automate repetitive tasks, analyze data faster, and operate continuously without fatigue, significantly increasing productivity in industries like manufacturing, healthcare, and finance.

Enhanced Decision-Making
AI systems can process large volumes of data and identify patterns humans might miss, leading to better forecasting, diagnostics, and strategic decisions.

Personalization and Customer Experience
AI powers recommendation engines and chatbots, enabling businesses to deliver personalized services and improve user satisfaction across platforms like e-commerce, streaming, and customer support.

❌ Disadvantages of Using AI:
Job Displacement and Economic Inequality
Automation of tasks can lead to job losses, particularly in sectors like transportation, retail, and clerical work, potentially widening economic inequality if not managed properly.

Bias and Ethical Concerns
AI systems can inherit biases from training data, leading to unfair or discriminatory outcomes—especially in sensitive applications like hiring, policing, or lending.

Lack of Transparency (Black Box Problem)
Many AI models, especially deep learning ones, operate in ways that are not easily understandable. This makes it difficult to audit decisions or hold systems accountable for mistakes.

These pros and cons highlight the need for responsible development, regulation, and human oversight when implementing AI technologies.
"""

# Observation: The model successfully broke down sentiments into actionable insights.

# ========================================
# Summary & Reflection
# ========================================

"""
Tools Used:
- ChatGPT (GPT-4o)

Prompting Strategies:
- Zero-shot, one-shot, Framework Prompting
- R.A.C.E, A.P.E, T.A.G frameworks
- Clarified roles and goals to guide outputs

Learnings:
- The clearer the role and goal, the better the output quality.
- Using analogies or examples is very effective for simplifying technical ideas.
- Structuring prompts using frameworks helped reduce ambiguity and improved consistency in model responses.
"""
'''






