## What is AGI (Artificial General Intelligence)

1. Ability to reproduce human intelligence and capabilities in machines.
2. Capabilities include:
   1. Learn new skills through observation.
   2. Understand abstract concepts and apply reasoning.
   3. Communicate using a language and understand the nonverbal cues, such as facial recognition, tone variation, and body language.
   4. Handle complex situations in real time.
   5. Plan for short and long-term situations or projects.
   6. Create music and art or invent something new.
3. Need for AI:
   1. Automation and decision making.
   2. Creative support.
4. AI examples: language translation, image classification, text-to-speech, product recommendations, anomaly detection, self-driving cars, weather forecasting, and image from text.
5. Language AI models refer to artificial intelligence models that are specifically designed to understand, process, and generate natural language.
6. Deep Learning Models used for language AI models:
   1. Recurrent neural networks, which process data sequentially and store hidden states.
   2. Long short-term memory, which processes data sequentially and can retain the context better through the use of gates.
   3. Transformers, which process data in parallel.
## Machine Learning
7. ML (Machine Learning) is a subset of AI that focuses on the development of algorithms that enable machines to learn from and make predictions or decisions based on data. Algorithms learn from past data and predict outcomes and trends.
8. DL (Deep Learning) is a subfield of ML that uses neural networks with many layers, deep neural networks, to learn and make sense of complex patterns in data.
9. Training a model:
   1. Defining features are the input data to the model.
   2. The label is the corresponding output, also provided by the user.
   3. The machine learning model is trained with this data set.
   4. The training data set consists of a set of features and output labels and is given as an input to the machine learning model.
   5. In training, the model learns between the input features and the output label. Once it is trained, it is called a trained model.
   6. Inference is a process of getting a prediction by giving a data point.
10. Types of Machine Learning:
    1. In supervised machine learning, labeled data is used to train the model. Model learns the relation between features and labels.
    2. Unsupervised learning is generally used to understand relationships within a data set. Labels are not used or are not available.
    3. Reinforcement learning uses algorithms that learn from outcomes to make decisions or choices.
11. Types of Supervised learning: Regression, Classification.
    1. In a supervised machine learning model, the output can be either categorical or continuous.
    2. When the output is continuous, we use regression to predict a numeric output.
    3. When the output is categorical, we use classification to predict a category or a label.
    4. In classification, there are binary and multi-class.
    5. Logistic Regression is a binary classification algorithm commonly used in Machine Learning to predict binary outcomes.
    6. Sigmoidal function to predict the probability of a binary outcome. The sigmoidal function, often represented as the sigmoid function, has an S-shaped curve that maps any input value to an output value between 0 and 1.
    7. Linear Regression is a regression algorithm used for predicting continuous numerical values by modeling the relationship between dependent and independent variables using a straight line.
    8. Decision Tree Classification is also used for classification tasks, not regression.
12. Clustering is the grouping of similar data items. The data items are more similar within a cluster than outside it.
13. Workflow of Unsupervised Workflow:
    1. Prepare the data: Remove missing values, normalize the data, and perform feature scaling.
    2. Create similarity metrics: Choose similarity based on the nature of the data and clustering algorithm used.
    3. Run clustering algorithm: Use the similarity matrix to cluster the data.
    4. Cluster algorithms: partition-based, hierarchical-based, density-based, and distribution-based.
    5. Interpret the results and adjust clustering by iteratively experimenting.
    6. K-Means Clustering is an unsupervised learning algorithm used for clustering data points, not for regression.
14. Reinforcement learning:
    1. A type of machine learning that enables an agent to learn from its interaction with the environment while receiving feedback in the form of rewards or penalties without any labeled data.
    2. Agent: A learner or decision maker that interacts with the environment, takes actions, and learns from the feedback received.
    3. Environment: The external system with which the agent interacts.
    4. Action: Is a set of possible moves or decisions that the agent can take in a given state. Actions have an impact on the environment and influence future states.
    5. Policy: A strategy or mapping that the agent uses to decide which action to take in a given state. It defines the agent's behavior and determines how it selects actions.

## Deep Learning
15. Deep learning is a subset of machine learning that focuses on training artificial neural networks (ANN) to solve a task at hand.
16. An important quality of the ANN is that it can process raw data like pixels of an image and extract patterns from it. These patterns are treated as features to predict the outcomes.
17. Need for Deep Learning:
    1. Specify features.
    2. Extract features from raw complex data.
    3. Internal representation of data is built using extracted features.
    4. Dl algorithms allow parallel processing of data.
    5. So these algorithms can process large amounts of data in a short time to learn the features and their combinations. This leads to scalability and performance.
   
18. Types of Deep learning algorithms:
   1. CNN (Convolutional Neural Networks): For image classification, object detection, image segmentation, or facial recognition.
   2. Transformers, Long-Short-term Memory (LSTM), and Recurrent Neural Networks (RNN): Sequential, Time Series, and Natural Language Data.
   3. Transformers, Diffusion Models, and Generative Adversarial Networks (GAN): generating images, text-to-image generation, and Audio generation.

19. Artificial Neural Networks (ANN): Inspired by the human brain, consist of interconnected nodes called neurons and process information.
20. Building blocks of ANN:
   1. Layers: Input, hidden, and output layers receive inputs, transform it, and produce output.
   2. Neurons: A Computational unit from an input and produces an output.
   3. Weights: Determines the strength of connection between neurons.
   4. Activation function: Works on the weighted sum of inputs to a neuron and produces an output.
   5.  Bias: Additional input to a neuron that allows a certain degree of flexibility.
21. Sequence models: Used to solve problems where the input data is in the form of sequences. The sequences are ordered lists of data points or events. The goal in sequence models is to find patterns and dependencies within the data and make predictions, classifications, or even generate new sequences.
22. Types of RNN: One-to-one, One-to-many, Many-to-many, Many-to-one.
23. LSTM: Works by using a specialized memory cell and a gating mechanism to capture long-term dependencies in the sequential data. The key idea behind LSTM is to selectively remember or forget information over time, enabling the model to maintain relevant information over long sequences, which helps overcome the vanishing gradients problem. It has 3 gates: Input, Forget, and Output.
24. Deep Learning Models:
    1. Feed-forward Neural Networks (FNN)
    2. Convolutional Neural Network (CNN): This can automatically detect and learn local patterns and features in images and videos.
    3. Recurrent Neural Network (RNN): Designed to handle sequential data such as time-series data or natural language. They have a feedback loop that allows them to maintain hidden states and capture temporal dependencies.
    4. Autoencoders: Unsupervised learning models used for feature extraction and dimensionality reduction, and are commonly employed in data compression and anomaly detection.
    5. LSTM
    6. Generative Adversarial Networks (GAN): Used for generating realistic synthetic data such as images, audio, and text.
    7. Transformers: "state of the art" models for tasks like machine translation, text generation, and language understanding.
25. CNN layers: Input, Feature extraction, and classification.

## Generative AI
26. A type of AI that can create new content.
27. Learns the underlying patterns in a given data and uses that knowledge to create new data that shares those patterns.
28. Types: Text-based, Multimodal.
29. Applications: Image and video generation, creative content, medical imaging, NLP, data synthesis and so on.
30. Langugage Model: It is a probabilistic model of text that determines the probability of a given sequence of words occurring in a sentence based on the previous words. It helps to predict which word is more likely to appear next in the sentence.
31. The large in the large language model (LLM) refers to the number of parameters. Now there is no agreed upon threshold upon which a model becomes large or a small. LLMs are fine tuned by taking a pretrained foundational model and providing additional training using custom data. 
32. Based on the deep learning architecture Transformers.
33. Transformers have 2 main parts(models): encoder and decoder.
34. Encoder model converts a sequence of words to an embedding vector representation.
35. Decoder model take a sequence of words and output the next word. Produces single token at a time.

## Prompt Engineering
36. Prompt: The input or initial text provided to the model.
37. Prompt Engineering: The process of iteratively refining a prompt for the purpose of eliciting a particular style of response.
38. Reinforcement Learning from Human Feedback (RLHF) is used to fine-tune the LLMs to follow a broad class of written instructions.
39. Strategies for generating prompts:
   1. In-context learning: Conditioning an LLM with instructions or demonstrations of the task it is meant to complete.
   2. k-shot prompting: Explicitly providing k examples of the intended task in the prompt. Can also start with k = 0.
   3. Chain-of-thought prompting: Prompt the model to break the problem into small chunks, exactly like you would solve it if you were solving it yourself, and then you break it into smaller parts, and then you solve each of these intermediate steps or each of these smaller parts.
   4. Hallucination: Model generated text that is non-factual or ungrounded.
40. RAG (Retrieval Augmented Generation): Optimize the output of a LLM with targeted information without modifying the underlying model itself.
