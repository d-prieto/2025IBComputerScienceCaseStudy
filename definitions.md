# Case Study definitions (in orden of appearance) 

Before getting into the case study definitions in Depth I'm using another layer of definitions a bit more simple to later get into these concepts. You can access [here](https://github.com/d-prieto/2025IBComputerScienceCaseStudy/blob/main/Context-definitions.md)

## Latency
Latency refers to a delay or lag in response time and is used in various contexts. Here’s a breakdown of how it’s understood in different fields:

### 1. Computing and Networking
Definition: Latency refers to the time it takes for data to travel from its source to its destination.
Example: The time it takes for a signal to be sent from your computer to a server and back is called network latency.
High Latency: Causes lag or delay in data transmission, affecting real-time applications like video calls or online gaming.
Low Latency: Means faster communication and is ideal for tasks that require quick responses, like high-frequency trading.

### 2. Audio and Music Production
Definition: In audio processing, latency is the delay between when an audio signal is input (e.g., you play a note) and when it’s heard through the output (e.g., your speakers).
Example: When recording music, if there is too much latency, there can be an audible delay between what you play and what you hear back.
Importance: Low audio latency is crucial for live performances or real-time recording.

### 3. Telecommunications
Definition: In telecommunications, latency refers to the time delay experienced in a system when transmitting a signal.
Example: Latency in satellite communications, where signals travel to space and back, leading to noticeable delay during calls.
Importance: Lower latency is crucial for seamless communication, especially in real-time services like VoIP.

### 4. Cloud Computing
Definition: In cloud services, latency refers to the time delay between a request made by a user (such as accessing data or running a computation) and the time it takes to receive a response.
Example: The time it takes for a file to load from a cloud storage service like Google Drive or Dropbox.
Impact: Low latency is important for applications like streaming services, where users expect minimal lag.

### 5. Storage Devices (e.g., SSDs, Hard Drives)
Definition: In the context of storage, latency refers to the time delay between when a request for data is made and when the data is actually retrieved from a storage device.
Example: On an SSD (solid-state drive), latency is much lower than on a traditional hard drive, resulting in faster access to files.

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
A big dataset is represented by a very huge amount of data, typically in the millions or more, which can be comprehensively analyzed to discover patterns. The size is adequate for effectively training machine learning models.

Example
For instance, social network datasets like Instagram or TikTok store massive amounts of data such as posts, likes, comments, etc. These datasets provide ample data for research, analysis, or improving recommendation algorithms, which show us posts we want to see.

Bad example
A dataset that holds a small amount of data, such as only a few rows from a small grocery store. This would not be useful for deep learning as it lacks the large amount of data needed for analysis or training.

### Accurate
An accurate dataset closely reflects the real-world situation it depicts, with very few errors, ensuring correctness, up-to-date status, and data precision.

Example
A dataset used by hospitals, which contains up-to-date patient diagnoses and health records.

Bad example
A dataset where images are incorrectly labeled, such as vegetables being named fruits. This would negatively impact any analysis.
### Classified
A classified dataset is organized into specific categories or classes, making it easier to analyze.

Example
A dataset with clearly labeled images categorized into ten distinct groups, such as vehicles classified as airplanes, cars, motorcycles etc.

Bad example
A dataset with images that are not clearly labeled and randomized, requiring someone to label them individually.
### Readable 
A readable dataset is formatted in a standard computer language, making it automatically readable by a web application or computer system.

Example
Spreadsheets with header columns that can be exported as comma-separated values (CSV).

Bad example
A poorly formatted dataset stored in a proprietary or binary format, without documentation. It would be difficult to parse or understand without specific tools.
### Domain specific
A domain-specific dataset contains data relevant to a particular field or industry, allowing experts to derive meaningful insights and develop specialized models.

Example
A dataset used in medicinal chemistry, containing data on specific chemical reactions. This kind of dataset is focused on the relevant field.

Bad example
A generic dataset for sea animals that contains data on land mammals. This would not be useful for scientists trying to develop models focused on sea animals.
### Relevant
A relevant dataset contains data directly related to the research or analysis task, aligning with the objectives and goals of the study.

Example
A dataset for an underwater study containing data on sea animals and underwater plants, all relevant to the research topic.

Bad example
A dataset on pet ownership used to study global economic trends, which would be irrelevant to the context of the research.
### The concepts of synthetic and real data in this context
This is artificially generated data created using algorithms to simulate real-world conditions. It is useful for training models when real data is scarce or privacy is a concern. Synthetic data can create large datasets without violating privacy laws but may lack the complexity and variability of real-world data.

Example
A computer-generated dataset that simulates credit card transactions to test a fraud detection model without using actual customer data.

Real Data
This is data collected from real-world observations or events. Real data is often messier, with noise, missing values, and inconsistencies, but it reflects actual scenarios. It is generally more accurate for building predictive models in real applications.

Example
Actual credit card transaction records used to train a model to detect fraudulent activities.
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
Deploying a machine learning model involves transitioning a trained model from its development environment to a production system, where it can perform real-time tasks such as generating predictions or interacting with users, as in a chatbot. This process requires setting up the necessary infrastructure to ensure the model runs efficiently, handling factors like computational power, memory, and storage. For large-scale models, such as those used for natural language processing (NLP), significant hardware resources like GPUs (Graphics Processing Units) or TPUs (Tensor Processing Units) are often needed to ensure fast inference and low latency. Additionally, it’s crucial that the infrastructure is flexible to handle fluctuating demand, especially for real-time applications with high user interaction. 
Deploying on Infrastructure as a Service (IaaS) platforms, such as Amazon Web Services (AWS) or Google Cloud Platform (GCP), is often the best approach. These platforms provide elastic scaling, advanced hardware, and cost-efficiency by allowing businesses to pay only for the resources they use. IaaS also supports automatic scaling and load balancing, ensuring that the chatbot performs well under varying loads and maintains high availability. In short, IaaS solutions offer the flexibility and power required to deploy, scale, and maintain large models like those used in sophisticated chatbots.
