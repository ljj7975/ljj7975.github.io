## How can we verify that the model actually understands a concept?

### TL;DR: There are three different ways to validate a model's understanding: free-form explanations, data-driven validation, and task-specific reasoning.

During a recent presentation to my lab colleagues outlining my upcoming project on explaining a model's understanding, I faced a question: "How can we verify that the model actually understands the concept?" This query momentarily gave me pause, not because I lacked an answer, but because I hadn't anticipated such a question after already outlining my approach using heatmap-based visualizations for verification.

As I mentioned in [my previous blog](README.md), I believe the way to demonstrate understanding is through the model's ability to apply its knowledge to a new domain (transferability). However, this sentence can still be quite vague. Reflecting on discussions with my colleagues, I categorized potential methods into three main approaches:

**1. Explaining in free form**:
This type of method involves the model providing an explanation in natural language, drawings, or other forms. Similar to how humans describe what a bird is—its appearance, dictionary definition, or sound—this approach is the most natural way to explain an idea to others.

- Pros: Natural and intuitive method. No additional resources are necessary as the explanations are generated.
- Cons: Subjective evaluations make quantitative assessment challenging.

  **2. Retrieving relevant data**:
  Here, the model identifies relevant information from a data source. For example, we can verify if a model has the right understanding by asking it to select images that best match its understanding.

- Pros: Quantitative evaluation is feasible (e.g., retrieval accuracy).
- Cons: Heavy reliance on the quality and representativeness of available data.

  **3. Showing reasoning within a limited scope**:
  When the target task is known, we can verify the model's understanding by reverse engineering how the final outcome is deduced. For example, in the case of computer vision, heatmap visualization can highlight which parts of an image influence its decisions the most, providing insight into the model's understanding within a specific context.

- Pros: Being specific to the task, it can indicate whether the model possesses the requisite understanding to perform the intended task effectively or not.
- Cons: Limited to explaining decisions within a predefined scope (e.g., the reasoning is valid only for the input provided and the specific target task it addresses).

Unfortunately, there is no one-size-fits-all approach. Each method comes with unique advantages and drawbacks. It is also important to remember that, regardless of which method we choose, there may be method-specific biases to consider. The choice of method depends on the level of detail required for explanation, making some methods more suitable than others. Overall, employing multiple methods is highly recommended to accurately verify the model's understanding.
