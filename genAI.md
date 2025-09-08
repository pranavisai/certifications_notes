1. A language model is a probabilistic model of text.
2. LLMs:
   1. Encoders and Decoders are built on a building block called a transformer.
   2. Embedding: The process of converting a sequence of words into a single vector or a sequence of vectors.
   3. The embedding of text is a numeric representation of the text that tries to capture the semantics or meaning of the text.
3. Prompt Engineering: This is the process of iteratively refining the model input in an attempt to induce a probability distribution that we like for a particular task.
4. In-context learning: Conditioning an LLm with instructions and or demonstrations of the task it is meant to complete. Usually by prompting.
5. K-shot prompting: Explicitly providing k examples of the intended task in the prompt.
6. Chain-of-thought prompting: Prompt the LLM to emit intermediate reasoning steps.
7. Least-to-most prompting: Prompt the LLM to decompose the problem and solve, easy-first.
8. Issues with prompting: Can be used to elicit unintended or harmful behaviour from a model.
9. Prompt injection: The prompt is being crafted in such a way as to elicit a response from the model that is not intended by the deployer or the developer. Examples: to reveal private information.
10. Training models: The process of giving the model an input, having a guess at a corresponding output.
11. Training styles: Fine-tuning, Parameter Efficient fine-tuning, soft prompting, and continued pre-training.
12. Decoding Types:
    1. Greedy decoding: Pick the word in the vocabulary with the highest probability.
    2. Nucleus Sampling: Govern precisely what portion of the distribution over words you're allowed to sample from.
    3. Beam Search: Ends up outputting sequences that have higher joint probability than the sequences that are output as a result of greedy decoding.
13. LLM Applications:       
   1. RAG (Retrieval Augmented Generation): The system transforms the user input (question) into a query that will be used to search a database. The returned documents will be provided to the LLM as input in addition to the question. And the expectation is that the model will generate a correct answer
   2. Code models: LLMs trained on code, comments, and documentation.
   3. Multi-modal models: Models are trained on multiple data modalities, for example ,text, images, and audio. These models can produce images or even video from textual descriptions and perform similar types of tasks.
   4. Language Agents: Models that are intended for sequential decision-making scenarios, for example playing chess, operating software autonomously, or browsing the web in search of an item expressed in natural language.
17. Types of pretrained foundational models: chat models and embedded models.
18. Embeddings are text converted to a vector of numbers. Embeddings make it easy for computers to understand the relationship between pieces of text.
19. Tokens:
    1. LMs understand "tokens" rather than characters.
    2. One token can be a part of a word, an entire word, or just punctuation.
    3. The number of tokens depends on the complexity of the text.
20. Chat model parameters:
    1. Maximum output tokens: The maximum number of tokens generated per response.
    2. Preamble override: Initial guideline message that can change the model's overall chat behaviour and conversation style.
    3. Temperature: Controls the randomness of the output. Lower values are used in tasks with a correct answer. Higher values generate more creative outputs or use words with lower probabilities, but a higher chance for hallucinations.
    4. Top K: Tells the model to pick the next token from the top "k" tokens in the list, sorted by probability.
    5. Top P: Picks from he top tokens based on the sum of their probabilities.
    6. Frequency and Presence penalties: Useful to get rid of repetition in outputs.
      1. Frequency penalty: Used to give a penalty to a token that has appeared more times to reduce its appearance in the next times. This helps in showing tokens that have not appeared more.
      2. Presence penalty: Used to apply penalties regardless of frequency. If the token appears, it gets penalized.
21. 
