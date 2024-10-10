# Case Study definitions (in orden of appearance) 

Before getting into the case study definitions in Depth I'm using another layer of definitions a bit more simple to later get into these concepts. You can access [here](https://github.com/d-prieto/2025IBComputerScienceCaseStudy/blob/main/Context-definitions.md)

## Latency
[Expand bit by bit the different concepts from the booklet, with some more explanations in the marked concepts]

### Critical Path
A series of activities in a project which, when delayed, will delay the project completion time. In other words, the critical path is the sequence of stages or steps in a process that determine the minimum time required to complete a project. In the context of software development, identifying the critical path helps in pinpointing the tasks that cannot be delayed without affecting the overall timeline. These tasks form the longest sequence in the project's network diagram, and any delay in a critical path task will directly delay the entire project. In system performance, it is the path that dictates the latency of an overall task.\




### Machine learning dependencies

Machine learning (ML) dependencies refer to the prerequisite components, libraries, or data needed for a machine learning model to function. These include:

1. Training Data: Large datasets needed to train the model.
2. Libraries & Frameworks: Tools like TensorFlow, PyTorch, or Scikit-learn provide pre-built functions for training and implementing models.
3. Compute Resources: Powerful GPUs or TPUs (tensor processing units) are often necessary to process complex ML tasks efficiently.
4. Dependencies Between Models: Sometimes, one ML model's output serves as the input for another, which creates dependency across different models.

Machine learning models rely heavily on these dependencies for accuracy and efficiency. For instance, poor-quality training data or insufficient compute resources can significantly impact the model's performance.


### Natural language understanding (NLU)


## Different types of analysis of a phrase by a Natural Language Processing Model
[Do a table of different types of analysis of a phrase and then explain them and their relationship with this context]

### Discourse integration
### Lexical analysis
### Pragmatic analysis
### Semantic analysis
### Syntactical analysis (parsing)

## Recurrent neural network (RNN)
[Build from the understanding of Neural Networks and gradient of a function from up above and explain the different concepts]

### Memory of the network

### Layer weight

### Hyperparameter tuning

### Backpropagation through time (BPTT)

### Loss function

### Vanishing gradient

## Long short-term memory (LSTM)
[Expand the the definition from the booklet with examples so everybody can understand it]

### Memory cell state
### Input gate
### Forget gate
### Output gate 

## Transformer Neural Networks (Transformer NNs)
[Build from the understanding of Neural Networks and gradient of a function from up above and explain the different concepts]


### Self-attention mechanism 
[Go in detail with this]

## Specifications of a dataset: large, accurate, classified, readable, domain specific, relevant
[For each specification write the definition and an example of a dataset that complies that specification and a dataset that doesn't comply that specification]

### Large

### Accurate

### Classified

### Readable 

### Domain specific

### Relevant

### The concepts of synthetic and real data in this context


## Types of bias of datasets. 
[For each types of bias expand the definitions from the booklet and be specific in why (if applicable) are these biases unfair or inaccurate]

### Confirmation bias: The tendency to search for, interpret, favor and recall information in a way that confirms one's preexisting beliefs or hypotheses. In machine learning or AI contexts, this bias can creep into both the data collection process and model development stages. When data is selected or interpreted in a way that aligns with existing assumptions, it skews the model toward reinforcing preconceived notions. This results in models that may ignore contradictory evidence, leading to biased predictions. 

### Historical bias: Historical bias refers to bias present in data that stems from societal and institutional inequities in the past. Even if a dataset is large and representative of the population, it can still carry the prejudices and systemic inequalities of the time when the data was collected. Models trained on historical data may reproduce and perpetuate unfair practices, such as gender or racial discrimination, because they inherit the biases embedded in the data. Even though the model may be functioning "accurately" by learning from patterns, the predictions or outputs can still perpetuate unjust outcomes. 

### Labelling bias:  Labeling bias occurs when the labels assigned to data are influenced by subjective opinions, cultural norms, or societal biases. This bias can arise during the annotation process where human annotators may bring in their personal biases when labeling data, such as sentiment, categories, or other classifications. When labels reflect the biased views of the annotators rather than objective reality, models trained on this data will learn these biased associations. This is particularly problematic in areas like sentiment analysis, facial recognition, or object classification where subjectivity is a factor.


### Linguistic bias: Linguistic bias arises when language models or NLP systems are trained on text data that reflects biased or prejudiced language patterns. This can include biases related to gender, race, socioeconomic status, or other social categories, embedded in the way language is used. Language reflects social and cultural biases, and if these biases are not corrected or balanced in training data, models may perpetuate harmful stereotypes. For example, language models may associate certain professions with men and others with women because of historical gender roles in text. 

### Sampling bias: Sampling bias occurs when the data collected is not representative of the population or domain it is intended to model. This happens when certain groups or categories are underrepresented or overrepresented, leading to skewed predictions and inaccurate outcomes. A biased sample leads to models that generalize poorly across the population. If the data is skewed toward a particular demographic, the model’s performance will degrade when applied to underrepresented groups, resulting in unfair outcomes.

### Selection bias: Selection bias occurs when the process of selecting data points for analysis introduces systematic differences between the chosen data and the target population. This happens when certain individuals, cases, or events are more likely to be included in the dataset than others, often leading to a distorted view of reality. When data selection is biased, the resulting model will be less generalizable and prone to errors in real-world applications. Selection bias can reinforce disparities if certain groups are consistently left out or overrepresented in the training data. 

## Processing the data

## Preprocessing  the input data
[Explain how do you clean, select, transform y reduce the data and how you improve the quality and accuracy]

### Cleaning the data.

### Selection

### Transformation

### Reduction of data 

## Bag-of-words algorithm
[Expand the definition from the booklet with examples so everybody can understand it]

## Training a model
[Expand the definition from the booklet. Try to find how big and how much calculations do we need for training a chatbot for this context and explain the concepts related to the hardware]

### Clusters of GPU

### Tensor Processing Unit (TPU)

## Deploying a model
[Expand the definition from the booklet. Try to find how much calculations and how big we need our servers to handle this type of chatbot or if we need to use Infrastructure As A Service (IaaS)]




Weights
