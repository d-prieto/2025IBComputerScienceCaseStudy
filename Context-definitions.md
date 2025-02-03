# Previous concepts
These concepts are relevant to get some information for the concepts that we're going to work later. I divided because they are implicit in later concepts so understanding these are helpful for the next ones. 

_test_

## More generic lexicon tha is applied here

### Query
A query is an organized method of retrieving data from an information system for use or modification. In the context of databases, queries are precisely formulated requests. [1]
#### Difference between a Query and Prompt
In computer science, a query is a request for information or data from a database, while a prompt is an input or instruction given to a system (like an AI) to generate or execute a specific response. 

1. https://www.techopedia.com/definition/5736/query


### Pipeline 
Pipeline is a set of data-processing stages, where the output of the previous task is used as input for the next one. This allows for big tasks to be broken down into smaller ones and for the tasks themselves to run concurrently or sequentially.

In neural networks, a pipeline is a multi-stage process where tasks like data preprocessing, feature extraction, model training, tuning, evaluation, and deployment are performed in sequence

### Architecture of a system
An architecture of a system is a framework structured that defines the system's components, their relationships and how they interact with each other to achieve their specific goals. It covers both the high-level design and the low-level details of a system.

The architecture of a system can be splitted in different parts:
- Components of the system: Individual parts or modules that perform specific tasks or functions.
- Relationships: How the components interact and how they communicate with each other
- Patterns and Styles: Established metodologies by the framework to structure the components and their interactions
- The software and hardware used to implement the architecture
- How the system works in different situations and environments
Examples:
- Client-server architecture
    - As we've seen in topic 3, in this model clients request queries to a server that provide responses to those queries.
    - A web application where the browser (client) requests web pages from a web server. The server processes the request and sends back the HTML/CSS/JavaScript needed to render the page.
- Microservices architecture
    - This architecture breaks down a large application into smaller
    - An e-commerce platform where different microservices handle user authentication, product catalog, payment processing, and order management. Each service communicates through APIs.
- Layered architecture
    - Also seen in topic 3, This architecture organizes the system into layers, each with a specific responsibility, such as presentation, business logic, and data access.
- Artificial intellignece example
    - AI architectures typically consist of components like data collection, preprocessing, model training, inference, and feedback loops.
    - Example: In a recommendation system, the architecture might include:
        - Data Ingestion Layer: Collects user data and interaction history.
        - Data Processing Layer: Cleans and transforms data for analysis.
        - Model Training Layer: Trains machine learning models using historical data.
        - Inference Layer: Generates real-time recommendations for users.
        - Feedback Loop: Collects user responses to improve the model over time.


### Decision algorithm 
**DEFINITION**
Decision algorithm—also know as the decision tree—is a supervised learning algorithm widely used for machine learning for modeling and predicting outcomes based on input data. It takes the form of a tree, where each internal node represents a test on a specific attribute, each branch signifies a possible attribute value, and each leaf node indicates the final decision or prediction. Decision trees are part of the supervised learning category and apply to both regression and classification tasks.

**EXAMPLES**
- Decision trees can help with **medical areas** such as diagnosis and selection of a treatment. Additionally, they can evaluating the risks of the various choices and then factoring in personal values, a person can make more informed choices about medical care.
    
    ![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/eb7e7b41-687b-4e3b-be2c-9d05bcd320ba/b6d4ed08-6cd6-430a-a766-cacb042e7bf4/image.png)
    
- Decide trees can also help when it comes to **software engineering**.  For example, this tree outlines potential outcomes based on the severity and probability of each risk, helping teams make informed decisions to ensure projects stay on schedule and within budget.

![](https://prod-files-secure.s3.us-west-2.amazonaws.com/eb7e7b41-687b-4e3b-be2c-9d05bcd320ba/c4923aa9-f387-4168-b3c3-3d3b4a7159a2/image.png)

- **Bank decision trees** can help banks decide whether to launch a new financial product by predicting outcomes based on customer interest and market demand. It helps banks evaluate risks and make well-informed choices to effectively address market needs.

![](https://prod-files-secure.s3.us-west-2.amazonaws.com/eb7e7b41-687b-4e3b-be2c-9d05bcd320ba/43036047-c148-4ee9-bef4-9bccd26e09af/image.png)

### Deployment of a system 
[Define a bit what is the deployment of a system with a several examples, one of them related to Artificial Inteligence]
_definition_
Deployment is the process by which updates, patches, applications and modules are transported from developers' systems to end users and their devices. Therefore the deployment of a system is the transition of all the capabilities to the end users as well as support files and elements needed for maintenance to the end user’s support organizations.

_example_
Softwares, as a system, can also be deployed. An example would be a user downloads a mobile application from the Integration Store and installs it onto their mobile device.

## Deep learning
[Define what is deep learning and its limitations]


## Neural network
[Define Neural Network with examples and explaining the concepts bellow]

### Hyperparameter (in a neural network)

### Layer of a neural network

### Input layer 

### Hidden layer

### Output layer

## Gradient of a function (and relationship with Neural Networks)
[Define what is the gradient of a function with an example and its relationship with Neural Networks]

## Dataset
[Define what is a dataset of a Deep learning network with some examples. Try to get specific]
Deep learning data refers to the datasets used to train, validate, and test deep learning models. For this type of dataset it is much better if it contains huge amount of data from which the model can be trained on (the more the better).
First you input data like image, video, text etc. After that the model tries to output the most accurate prediction by using labels (as categories) ---> if you put an image of a cat it will try to predict output with the label named cat.
It has 3 splits which assures that the model is well trained, validated and most importantly trained effectively:
Training set is used to train neural network by adjusting its parameters, in this phase the model learns patterns and relationships in the data ---> this is usually the largest portion of the dataset.
Validation set is used DURING the training it helps to set and adjust the model's settings, such as its structure and training parameters ---> it shows how well the model is expected to perform on new, unseen data.
Test set is used to provide a final, unbiased evaluation of the model after it has been fully trained. It assesses how well the model generalizes to completely unseen data ---> model is NEVER EXPOSED to this test set (so we could determine its performance on real world scenarios)

We also have types of DATA
## Structured data:
Data that follows a pattern or has a predefined columns for example classification
## Unstructured data:
Data that doesn't follow predefined pattern for example images or audio

Example ---> dataset for electricity usage it does time series forecasting which helps to predict the future electricity consuption based on past consuption patterns.
Dataset that contains a collection of ECG - (electrocardiogram) signals to detect arrhythmia it does time series classification to define if ECG signal should be labeled as normal or abnormal.

---> Each model tries to predict some possible outcome

## Large language model (LLM)
Large language models are a type of foundation models that are trained on huge quantities of data allowing them to understand and generate natural language and sound like a human alongside other types of content to perform a wide range of tasks. They can infer from context, generate coherent and contextually relevant responses, translate to languages other than English, summarize text, answer questions and even assist in creative writing or code generation tasks. LLMs played a huge role in bringing generative AI to the forefront of public interest, as well as the point where businesses are beginning to adopt 	AI across numerous business functions and use cases. LLMs are easily accessible to the public through interfaces such as Open AIs or Chat GPT. 

There are SMLs which are Small Language Models. These are essentially smaller versions of their LLM counterparts. They have significantly less parameters, typically ranging from a few million to a few billion, compared to LLMs with hundreds of billions or even trillions. This makes them more efficient since they require less computational power and memory.  

There are Convolutional Neural Networks (CNNs) they are the heart of deep learning algorithms that are designed for image recognition and processing tasks, such as object detection, segmentation, and image classification. They use three-dimensional data for image classification and object recognition tasks. 

There are audio models that are designed for speech recognition, sound analysis, and music generation. Such as WaveNet that generates speech or RNNs that models music. 

References:
- https://www.ibm.com/topics/large-language-models
- https://medium.com/@nageshmashette32/small-language-models-slms-305597c9edf2
- https://www.ibm.com/topics/convolutional-neural-networks
- https://research.google/blog/audiolm-a-language-modeling-approach-to-audio-generation/


## Natural language processing model 
[Define what is it and the difference between this concept, an LLM and the concept of Natural Language Understanding]

## Machine-actionable information
Machine-actionable information is data which is formatted so that machines can read and interpret it without human action. 
To create machine-actionable information, format data in a clear, structured way like using codes, tags, or standard formats that computers can easily understand. 

For example: Words on a paper are not considered Machine-actionable information because the machine cannot work with it. The information of what pixels need to be white or black, so that they become a picture, is Machine-actionable information, because the machine can work with the pixel data. 

## Extra ball: Tensor
[Define what is a tensor with your words so your colleagues can more less understand it]

[some information here](https://en.wikipedia.org/wiki/Tensor_(machine_learning))


---
