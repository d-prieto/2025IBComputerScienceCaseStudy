# November test questions


ℹ️In this exam, since it was the first Paper 3 exam the last question (6) have been nerfed to 6 marks instead of 12 but it should marked as a 12 mark boundary. (to add up to 30 marks) ℹ️

1)	Identify two reasons why we use GPUs or TPUs to train NN. [2]
2)	Define the term Long short-term memory [2]
3)	Explain how the ethical challenges of transparency and accountability and responsibility could be tackled (if it can be tackled) using a LLM in the context of RAKT. [4]
4)	Describe the different information can we get from the different levels of natural language processing [4]
5)	Explain what is required to create a large high-quality, unbiased dataset in the context of RAKT. [6]
6)	Discuss whether a transformer NN could improve upon the performance of an RNN for natural language processing.  [6] 

## Answers from studends

Here the students can add their actual answers or their answers after some feedback. 

### Identify two reasons why we use GPUs or TPUs to train NN. [2]
<br> Answer: GPU's and TPU's are great at processing multiple tasks at the same time. So it is great for parallelization due to it having multiple ores or ALU's which can be tasked with different tasks at the same time to run in parallel. Another reason we use GPU's and TPU's is because it has it's own memory called VRAM. This ensures the NN does not use the memory of the other parts of the system.

### Define the term Long short-term memory [2]
<br> Long short-term memory is a type of Recurrent Neural Network designed to overcome the problem of vanishing gradient, which results in the model to stop stop learning more. So instead of changing the gradients dramatically during each time stop, we implement LSTM (long short-term memory) to selectively retain and forget information over time so the past data has an affect on the weights, biases and gradients generated during process and tackles the problem of vansihing or exploding gradient.

Answer full marks:
Long short-term memory (LSTM) - is a type of recurrent neural network designed to overcome the problem of vanishing gradient.

### Explain how the ethical challenges of transparency and accountability and responsibility could be tackled (if it can be tackled) using a LLM in the context of RAKT. [4]

full marks answer: 

_1. Transparency and accountability_

The chatbots's large language model may have issues with transparency, as the decision-making will be unclear and it will not allow the users or developers to see the reasoning behind the decision. This may lead to problems with invalid responses and the company representative will be accountable(held liable) for the mistakes. The LLM can be restructured or guven only specific data foe trining to avoid the problem.

_2. Responsibility_

In a business like RAKT, an insurance company, it is veyr important that the data given to the customers is accurate. If a worker shares wrong forms with a customer, the worker will be held accountable and punished. However, in the case of the chatbot, the error-rate will probably reduce but it will be harder to put blame on a specific person when the errors do occur. This may be tackled by having a representative, who will take over when the customers are ont satisfied with the service of the bot. The chatbot will further be trained on these cases to improve the LLM.


### Describe the different information can we get from the different levels of natural language processing [4]
Answer 3 out of 4 - no examples:
Natural language processing have 5 stages:
	1) Lexical analysis:  breaking down the text - input to sentences and then to words - information: separate words;
	2) Syntatic analysis: interpreting grammar and structure of a sentence, getting "role" of each separated word - information: identifies what is object, subject, verb;
	3) Semantic analysis: analysing the meaning of each word - information: this word means this;
	4) Discourse integration: applying the meaning of the sentence to the longer context of the conversation - information: user wants to get "object" from chatbot;
	5) Pragmatic analysis: analysing social, cultural context.


### Explain what is required to create a large high-quality, unbiased dataset in the context of RAKT. [6]

### Discuss whether a transformer NN could improve upon the performance of an RNN for natural language processing.  [6] 
