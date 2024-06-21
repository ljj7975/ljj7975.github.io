## What is my interest?

### TL;DR: If we cannot interpret, we cannot make any conclusion there cannot use it.

About a year ago, I began working on few-shot object detection and classification. Throughout my research, I have constantly wondered whether the model truly understands the concept or simply memorizes it based on the examples, especially when reviewing the improved detection accuracy. This question has shaped the direction of my research, but I struggled to clearly describe the end goal due to its dependency on multiple interconnected components. Recently, I had engaging conversations with several very smart people about AI, which helped me finally articulate this in a clear sentence.

**I define intelligence as the ability to extract abstract concepts from knowledge (comprehension) and adapt to a new domain (transferability)**. In other words, I argue that an agent is intelligent only if it demonstrates both comprehension and transferability. This is how we learn and convey our understanding.

As an individual with a research-oriented mindset and a solid understanding of industry priorities, **my personal interest lies in studying how to build an intelligent agent that demonstrates its intelligence in an interpretable form, ultimately benefiting humans**.

**I believe information sharing across different modalities plays a crucial role in building an intelligent agent by enabling the alignment between representation of human knowledge and representation of model knowledge**. (Although I strongly believe that data-driven and statistical methods introduce bias,) I think single-modality models may already possess intelligence, but it is represented in a way that humans cannot interpret. When asked if latest vision language models are intelligent, people often give different answers because we tend to interpret the model's knowledge from a human perspective, assuming the model represents knowledge in the same way humans do (e.g., visualizing attention maps and checking if they fall on reasonable pixels).

I believe that the knowledge obtained by a model from single-modality data would never be interpretable by humans. However, the latest advancements in AI, which aim to align multiple modalities in a human-interpretable fashion through similarity-based learning objectives, have indicated the direction I need to pursue in building an intelligent agent: If my goal is to create an intelligent agent that perceives and interprets the world like humans do, the knowledge representation must at least be aligned with that of humans.

One excellent example of this is Explainable AI designed around visualizing cross-attention between text and image inputs. When self-attentions from a vision-only model are visualized, the groups of similar pixel features do not make much sense to humans. However, with text-guided attention introduced, pixels correlated with the provided text show higher scores, enabling humans to understand where the model is focusing. I see this as the text modality serving as an interface for interpreting the model's knowledge represented in the visual modality. In other words, a vision-only model becomes more accessible to non-expert users through a text-based interface.

Overall, my research goal can be (finally) summarized as **building an intelligent agent that possesses human-interpretable comprehension ability and demonstrates its benefits to humanity through effective transferability**.

(As you might have inferred from my previous experiences,) I have had a genuine interest in deep learning itself rather than its domain or modality-specific applications since the beginning of my career. After solidifying the type of research I want to pursue, I believe this perspective has helped me establish the aforementioned view on AI significantly. More importantly, while I have previously thought my diverse experience might lack specialization, I now see that my experiences align well with my future direction.