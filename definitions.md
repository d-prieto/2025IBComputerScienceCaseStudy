# Case Study definitions (in orden of appearance) 

Before getting into the case study definitions in Depth I'm using another layer of definitions a bit more simple to later get into these concepts. You can access [here](https://github.com/d-prieto/2025IBComputerScienceCaseStudy/blob/main/Context-definitions.md)

## Latency

Latency refers to a delay or lag in response time and is used in various contexts. Here’s a breakdown of how it’s understood in different fields:

#### 1. Computing and Networking
**Definition:** Latency refers to the time it takes for data to travel from its source to its destination.
<br> **Example:** The time it takes for a signal to be sent from your computer to a server and back is called network latency.
<br> **High Latency:** Causes lag or delay in data transmission, affecting real-time applications like video calls or online gaming.
<br> **Low Latency:** Means faster communication and is ideal for tasks that require quick responses, like high-frequency trading.

#### 2. Audio and Music Production
**Definition:** In audio processing, latency is the delay between when an audio signal is input (e.g., you play a note) and when it’s heard through the output (e.g., your speakers).
<br> **Example:** When recording music, if there is too much latency, there can be an audible delay between what you play and what you hear back.
<br> **Importance:** Low audio latency is crucial for live performances or real-time recording.

#### 3. Telecommunications
**Definition:** In telecommunications, latency refers to the time delay experienced in a system when transmitting a signal.
<br> **Example:** Latency in satellite communications, where signals travel to space and back, leading to noticeable delay during calls.
<br>**Importance:** Lower latency is crucial for seamless communication, especially in real-time services like VoIP.

#### 4. Cloud Computing
**Definition:** In cloud services, latency refers to the time delay between a request made by a user (such as accessing data or running a computation) and the time it takes to receive a response.
<br> **Example:** The time it takes for a file to load from a cloud storage service like Google Drive or Dropbox.
<br> **Impact:** Low latency is important for applications like streaming services, where users expect minimal lag.

#### 5. Storage Devices (e.g., SSDs, Hard Drives)
**Definition:** In the context of storage, latency refers to the time delay between when a request for data is made and when the data is actually retrieved from a storage device.
<br> **Example:** On an SSD (solid-state drive), latency is much lower than on a traditional hard drive, resulting in faster access to files.

#### Latency refered to RAKT and what it may be influencing it. 

// TO DO BY THE STUDENTS. 

### Critical Path

![Pert_chart_colored svg](https://github.com/user-attachments/assets/53cac605-8ec3-40d1-8f63-06dbe2cc4648)

A series of activities in a project which, when delayed, will delay the project completion time. In other words, the critical path is the sequence of stages or steps in a process that determine the minimum time required to complete a project. In the context of software development, identifying the critical path helps in pinpointing the tasks that cannot be delayed without affecting the overall timeline. These tasks form the longest sequence in the project's network diagram, and any delay in a critical path task will directly delay the entire project. In system performance, it is the path that dictates the latency of an overall task.\

#### Reference

https://en.wikipedia.org/wiki/Critical_path_method


### Machine learning dependencies

// TO - DO BY THE STUDENTS. 

### Natural language understanding (NLU)

Natural Language Processing (NLP) systems map out linguistic elements and structures. A subset of research and development called "natural language understanding" is based on these systems' fundamental components. Natural Language Understanding aims to achieve comprehension, while Natural Language Processing concentrates on developing systems to interpret human language.


## Different types of analysis of a phrase by a Natural Language Processing Model
[Do a table of different types of analysis of a phrase and then explain them and their relationship with this context]

### Discourse Integration
(Also known as Contextual Analysis) is when a program also takes contextual clues of the text in order to understand it.

For example if the program sees "This is not true", it is hard to understand what exactly is being reffered to by "this." By looking at the sentance before and after (context) it will be more clear, what the text is talking about

### Lexical analysis
(Also known as Morphological analysis) is the process of the program breaking the text down into paragraphs, sentences, and words. Using this, the text is not analysed as a whole, but words are seen as components.
### Pragmatic analysis
Is a process of the program deriving meaning from the cultural norms of the text.
For example, if the text sees "I heart you" it will understand that here the noun heart replaces the verb "love" and Pragmatic analysis is used to understand this.
### Semantic analysis
Is used to undertsand the literal meaning of the words, without any non-direct meaning or interpretation to analyse the text for meaningfulness. 
For example such sentance as "hot ice-cream" will not be flagged as okay, because it's literla meaning is unclear.
### Syntactical analysis (parsing)
is used to analyse the proper order of the wording. It is able to transform the words a bit in order to make sense of the sentance. 
For example if the sentence "train is going station to the Fred," it will get flagged and possibly changed to "Fred is going to the train station." The program is able to detect such inproper sentences due to syntactical analysis.

1. https://www.linkedin.com/pulse/natural-language-processing-nlp-gaurav-haramkar#:~:text=Discourse%20Integration%2FContextual%20Analysis%20%2D%20Discourse,This%22%20in%20the%20previous%20sentences.


## Recurrent neural network (RNN)
[Build from the understanding of Neural Networks and gradient of a function from up above and explain the different concepts]

### Memory of the network

### Layer weight

### Hyperparameter tuning
Hyperparameter tuning is the process of finding the best configuration settings for parameters in a machine learning model that aren't learned from data, like learning rate or batch size. Its purpose is to optimize the machine performance by testing a lot of different parameter combinations. Most commons methods used are: grid search, random search, Bayesian Optimization and evolutionary algorithms. Each of the methods make more efficient the machine.
### Backpropagation through time (BPTT)
Is an algorithm for training RNNs on sequential data. The RNN follow steps to learn, calculates errors at each step, and use these errors to adjust weights. BPTT enables RNN to learn from temporal dependencies but it can struggle with long sequences because of vanishing or exploding gradients
### Loss function
It measures the difference between a RNN model and its actual target values. Common types used are Mean Squared Error for regression, Cross-Entropy Loss for classification, and Hinge Loss for SVMs. The loss function choice depends on the problem type and impacts the model’s learning quality.
### Vanishing gradient

![anishing-Gradient-Problem-Graves-2012_W640](https://github.com/user-attachments/assets/7d00de7b-6141-4d40-8ac6-80136a474576)



The Vanishing gradient problem happens in deep Neural Networks when gradients become to small for backpropagation, which means that it unable learning from early layers. This issue affects the model's ability to learn complex patterns. Solutions commonly used are ReLU activations, Batch Normalization, or architectures like LSTMs.

(this part was added by the teacher)

In recurring neural networks usually the output is reintroduced with the previous input to find the next part of the output. So if you want to answer "What's the weather like in Minessotta?" (the input) the RNN will first have an output of "The" because it's what is most likely to happen and introduce it with the rest. So now the input will be "What's the weather like in Minessotta? The" and then add the word "weather" and so on. The disadvantadge of this is that the importance of the first words will be less and less over time. 

It's called vanishing gradient because it's about the partial derivative. (Gradients are found using derivatives)

#### Reference

https://en.wikipedia.org/wiki/Vanishing_gradient_problem

https://www.researchgate.net/publication/339873479_A_Comparative_Study_of_Sequence_Classification_Models_for_Privacy_Policy_Coverage_Analysis


## Long short-term memory (LSTM)
[Expand the the definition from the booklet with examples so everybody can understand it]

### Memory cell state
- The cell state is the memory unit of the network.
- The cell state carries information that can be stored in, written to, or read from a previous cell state via gates that open or close.
- Information from previous steps can enter the cell state and carry relevant information throughout the processing of the sequence.
- A single classic Long Short Term Memory unit consists of a cell state and its three gates: an input gate, an output gate and a forget gate.

### Input gate
It works as an input to the cell state. It consists of two parts; first, we pass the previous hidden state and current input into a sigmoid function to decide which values will be updated. Then, pass the same two inputs into the tanh activation to regulate the network. Finally, multiply the tanh output with the sigmoid output to decide which information is important to update the cell state. 

### Forget gate
The first block represented in the LSTM architecture is the forget gate. The forget gate decides what is relevant to keep from the prior cell state. The information from the current input and the previous hidden state is passed through the sigmoid activation function. If the output value is closer to 0 means forget, and the closer to 1 means to retain. 

### Output gate 
The hidden state contains information on previous inputs and is used for prediction. The output gate regulates the present hidden state. The previous hidden state and current input are passed to the sigmoid function. This output is multiplied with the output of the tanh function to obtain the present hidden state. The current state and present hidden state are the final outputs from a classic LSTM unit.  

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

### Confirmation bias: 
The tendency to search for, interpret, favor and recall information in a way that confirms one's preexisting beliefs or hypotheses. In machine learning or AI contexts, this bias can creep into both the data collection process and model development stages. When data is selected or interpreted in a way that aligns with existing assumptions, it skews the model toward reinforcing preconceived notions. This results in models that may ignore contradictory evidence, leading to biased predictions. 

### Historical bias:
Historical bias refers to bias present in data that stems from societal and institutional inequities in the past. Even if a dataset is large and representative of the population, it can still carry the prejudices and systemic inequalities of the time when the data was collected. Models trained on historical data may reproduce and perpetuate unfair practices, such as gender or racial discrimination, because they inherit the biases embedded in the data. Even though the model may be functioning "accurately" by learning from patterns, the predictions or outputs can still perpetuate unjust outcomes. 

### Labelling bias: 
Labeling bias occurs when the labels assigned to data are influenced by subjective opinions, cultural norms, or societal biases. This bias can arise during the annotation process where human annotators may bring in their personal biases when labeling data, such as sentiment, categories, or other classifications. When labels reflect the biased views of the annotators rather than objective reality, models trained on this data will learn these biased associations. This is particularly problematic in areas like sentiment analysis, facial recognition, or object classification where subjectivity is a factor.


### Linguistic bias: 
 Linguistic bias arises when language models or NLP systems are trained on text data that reflects biased or prejudiced language patterns. This can include biases related to gender, race, socioeconomic status, or other social categories, embedded in the way language is used. Language reflects social and cultural biases, and if these biases are not corrected or balanced in training data, models may perpetuate harmful stereotypes. For example, language models may associate certain professions with men and others with women because of historical gender roles in text. 

### Sampling bias: 
Sampling bias occurs when the data collected is not representative of the population or domain it is intended to model. This happens when certain groups or categories are underrepresented or overrepresented, leading to skewed predictions and inaccurate outcomes. A biased sample leads to models that generalize poorly across the population. If the data is skewed toward a particular demographic, the model’s performance will degrade when applied to underrepresented groups, resulting in unfair outcomes.

### Selection bias: 
Selection bias occurs when the process of selecting data points for analysis introduces systematic differences between the chosen data and the target population. This happens when certain individuals, cases, or events are more likely to be included in the dataset than others, often leading to a distorted view of reality. When data selection is biased, the resulting model will be less generalizable and prone to errors in real-world applications. Selection bias can reinforce disparities if certain groups are consistently left out or overrepresented in the training data. 

## Processing the data

## Preprocessing  the input data
[Explain how do you clean, select, transform y reduce the data and how you improve the quality and accuracy]

### Cleaning the data: 
Data Cleaning is the process of removing or fixing incorrect, duplicate, or incomplete information from a dataset to ensure that machine learning models—such as neural networks—are trained on the highest-quality data possible.

### Selection: 
Selection, or Feature Selection, is choosing the most relevant variables from a dataset so a neural network can learn efficiently, without being overwhelmed by unnecessary or redundant information.

### Transformation: 
Transformation is converting or modifying data into a form that is better suited for a neural network’s training process, often making it more uniform or reducing skewness.

### Reduction of data: 
Data Reduction is about compressing a large set of features into fewer, more meaningful components while retaining as much information as possible for the neural network to learn effectively.

## Bag-of-words algorithm:
_This was expanded by the teacher_

![1740730228463](https://github.com/user-attachments/assets/7a087402-bc47-4d1a-bf71-90177a6b150b)

Bag-of-Words (BoW) is a fundamental technique in natural language processing that represents text as a collection of word counts, ignoring word order or grammar. Used to represent the processing of natural languages and the retrieval of information. In general, it's a text representation technique which describes a document as a collection of words, with no grammar or word order, only focusing on preserving frequency (multiplicity). Thereby converting the textual data into a numerical one. (a very long vector, usually)

### Uses

The bag-of-words model is commonly used in methods of document classification where, for example, the (frequency of) occurrence of each word is used as a feature for training a classifier. It has also been used for computer vision.

In the case of RAKT(the case study) could be used for classifying either the dataset or the input. 

### Advantadges

- Fast, efficient and relativately easy to code.
- You don't need a Neural Network for this algorithm!

### Disadvantadges

- There could be some nuances regarding the appearance of certain words that should be addressed in design.
- The text is acutally not understood by the code. We can make just inferences. 

More references for Bag-of-words

https://en.wikipedia.org/wiki/Bag-of-words_model

https://builtin.com/machine-learning/bag-of-words

## Training a model
This refers to the act of teaching an algorithm to recognize patterns in data by tailoring its parameters from test runs using training datasets, thereby achieving optimization of the model's parameters. 

In the context of training a chatbot, massive datasets and computational power is required. Depending on hardware efficiency the training may take weeks to months. In terms of costs, for examples, training GPT-3 costs millions of dollars because GPU is used and also due to the electricity consumption. When considering hardware, it is important to note that GPU's accelerate training by processing thousands of operations in parallel. Other things needed are high speed storage (for data loading) and RAM (to store model weights). So, training a model requires a lot of resources, like massive datasets, high performance GPUs and terabytes of memory. Often, companies rely on things like cloud AI servies in order to ditribute the workload. 

### Clusters of GPU

### Tensor Processing Unit (TPU)

## Deploying a model
Deploying a machine learning model involves transitioning a trained model from its development environment to a production system, where it can perform real-time tasks such as generating predictions or interacting with users, as in a chatbot. This process requires setting up the necessary infrastructure to ensure the model runs efficiently, handling factors like computational power, memory, and storage. For large-scale models, such as those used for natural language processing (NLP), significant hardware resources like GPUs (Graphics Processing Units) or TPUs (Tensor Processing Units) are often needed to ensure fast inference and low latency. Additionally, it’s crucial that the infrastructure is flexible to handle fluctuating demand, especially for real-time applications with high user interaction. 
Deploying on Infrastructure as a Service (IaaS) platforms, such as Amazon Web Services (AWS) or Google Cloud Platform (GCP), is often the best approach. These platforms provide elastic scaling, advanced hardware, and cost-efficiency by allowing businesses to pay only for the resources they use. IaaS also supports automatic scaling and load balancing, ensuring that the chatbot performs well under varying loads and maintains high availability. In short, IaaS solutions offer the flexibility and power required to deploy, scale, and maintain large models like those used in sophisticated chatbots.

### Energy use of AI models

![d051832eeda42513](https://github.com/user-attachments/assets/2b97659b-33ed-4fb0-8a8f-2bf49f75f848)
(source https://www.nature.com/articles/d41586-025-00616-z)

## Ethical challenges faced

### Privacy 

#### Data anonymization 

https://en.wikipedia.org/wiki/Data_anonymization


Privacy is a concern, that is a problem that we need to tackle with the training and the operation of the chat model. For that probably we would need that no personal data is being fed not in training or execution of the model. In this case the main problem is that the algorithm could spit out the names or information that was input

For example, let's say that in the training we have an interaction like this:

"I'd like to do a claim about a car accident, my car with plate 4431FHG had a problem in Burgos" "Don't worry madam, we will send you a taxi"

It's possible that if we have later in operation an input of: 

"I'd like to do a claim about a car accident"

We may have an output of 

"Don't worry, madam, we're sending a taxi right away for your car plate 4431FHG"

So how do we solve this? One way could be stripping out the names from the training system so if we have a conversation like before we strip from the personal data. 

"I'd like to do a claim about a car accident, my car with plate $PLATE had a problem in $LOCATION" "Don't worry $TREATMENT, we will send you a taxi"

So if we have an input like 

"I'd like to do a claim about a car accident in Madrid"

Before arriving to the decision algorithm is already translated (this is a type of pre-processing) to "I'd like to do a claim about a car accident in $LOCATION" so the chatbot NN will create an answer similar to "Don't worry, we're sending somebody to $LOCATION" and later we post process the output of the NN to put back the actual location and answer "Don't worry, we're sending somebody to $MADRID"

This doesn't mean that we don't need to have other measures to ensure privacy, but it's one that is specific for this context. If you write something like "VPN" or "firewall" it's not on the topic. 


### Transparency

We talked about this in class. Here you have a caption:


![imagen](https://github.com/user-attachments/assets/0f4e0777-7029-4cf2-828c-b10b44893353)
source: https://www.youtube.com/watch?v=AaU6tI2pb3M
### What are counterfactual explanations and why is relevant here?



## Example of using ChagGPT text:
(don't do this if you want to actually do some notes on something) 

Machine learning (ML) dependencies refer to the prerequisite components, libraries, or data needed for a machine learning model to function. These include:

1. Training Data: Large datasets needed to train the model.
2. Libraries & Frameworks: Tools like TensorFlow, PyTorch, or Scikit-learn provide pre-built functions for training and implementing models.
3. Compute Resources: Powerful GPUs or TPUs (tensor processing units) are often necessary to process complex ML tasks efficiently.
4. Dependencies Between Models: Sometimes, one ML model's output serves as the input for another, which creates dependency across different models.

Machine learning models rely heavily on these dependencies for accuracy and efficiency. For instance, poor-quality training data or insufficient compute resources can significantly impact the model's performance.

