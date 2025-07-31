Slide 1: Title Slide
Title: Enhancing Model Risk Review with Prompt Engineering
Subtitle: Practical AI Techniques for Financial and Regulatory Contexts

Slide 2: What is Prompt Engineering?
Definition:
Prompt engineering is the structured method of crafting inputs to guide AI models (like ChatGPT) to produce reliable, relevant, and high-quality responses.

Relevance in Model Risk Management:

Extract complex insights from lengthy documents

Review regulatory alignment in model development

Assist in drafting structured critique and review reports

Accelerate documentation assessment

Slide 3: Key Prompting Techniques We’ll Cover
We’ll focus on practical, widely adopted prompting types that directly support MRM use cases:

Zero-shot Prompting

Few-shot Prompting

Chain-of-Thought Prompting

Zero-shot Chain-of-Thought

Generated Knowledge Prompting

Self-Refine Prompting

Slide 4: Zero-shot Prompting
What it is:
Directly asking the model to perform a task without providing any examples.

Use Case in MRM:
Ideal when evaluating if model documentation aligns with a known regulatory framework.

Example:
"Identify whether this model documentation sufficiently addresses SR 11-7 governance expectations."

Why it works:
Efficient for known regulatory checks; allows fast and consistent scanning of documents when the model has sufficient training on the domain.

Slide 5: Few-shot Prompting
What it is:
Providing a few examples (typically 2–5) of the desired question-answer format to guide the model.

Use Case in MRM:
Effective for tasks that require nuanced judgment — such as evaluating control effectiveness or the adequacy of model assumptions.

Example:
Prompt:

Example 1:
Input: "Model uses expert judgment to override model output."
Output: "Flagged: Requires justification per SR 11-7 qualitative overlays."

Example 2:
Input: "All assumptions validated using internal historical data."
Output: "No concern. Aligned with principle of empirical support."

Now evaluate: "The model calibration relies on peer bank data."

Why it works:
Helps the model learn tone, reasoning standard, and format of a regulatory review response.

Slide 6: Chain-of-Thought Prompting
What it is:
Encourages step-by-step reasoning before answering complex questions.

Use Case in MRM:
Useful for tracing the logical consistency of model assumptions or policy adherence.

Example:
Prompt:

"Is the model's use of 5-year data for LGD estimation acceptable?"

Let’s think step by step:

Regulatory guidance (OCC 2011-12) recommends representativeness and stability.

5-year span may exclude key stress periods.

LGD is sensitive to macroeconomic cycles.
Answer: The data window may be too short; further justification required.

Why it works:
Improves the quality of AI's regulatory reasoning and mimics reviewer-style analysis.

Slide 7: Zero-shot Chain-of-Thought Prompting
What it is:
Like zero-shot prompting, but explicitly requests reasoning steps without giving examples.

Use Case in MRM:
Best for uncovering flaws or gaps in the narrative of model documentation.

Example:
Prompt:

"Does this model meet CECL’s requirement for reasonable and supportable forecasts? Think step by step."

Why it works:
Guides the model to unpack regulatory logic even with a vague or new policy reference, increasing trust in the response.

Slide 8: Generated Knowledge Prompting
What it is:
The model first retrieves or constructs relevant background knowledge before performing the main task.

Use Case in MRM:
Useful when evaluating models against niche or less frequently cited regulatory standards.

Example:
Prompt:

“List key elements of OCC 2011-12 guidance on model validation.”
Now assess whether the following documentation covers these elements.

Why it works:
Helps ensure the model’s judgment is grounded in an appropriate regulatory framework before answering.

Slide 9: Self-Refine Prompting
What it is:
The model first generates a response, critiques its own reasoning, and improves upon it.

Use Case in MRM:
Valuable for complex review summaries or recommendations where nuance and correctness matter.

Example:
Prompt:

“Summarize the key risks in this challenger model.
Now review your summary for gaps in governance or performance metrics and improve the output.”

Why it works:
Creates more complete and robust assessments by simulating reviewer quality control.

Slide 10: Summary & Recommendations
Prompt Type	Best Use	Strength
Zero-shot	Policy compliance checks	Fast and simple
Few-shot	Controls & qualitative overlays	Learns from prior examples
Chain-of-Thought	Validation, calibration reasoning	Structured thinking
Zero-shot CoT	Auditing vague justifications	Induces multi-step logic
Generated Knowledge	Aligning with rare regulations	Fact-based, reference-driven
Self-Refine	Risk narratives & review reports	Iterative improvement

Slide 11: Final Thoughts for Senior Management
Prompt engineering is a valuable skill for modern model reviewers.

These techniques allow faster, more consistent, and more thorough reviews.

With responsible use, they can augment expertise — not replace it — in risk identification, documentation review, and regulatory assessments.
