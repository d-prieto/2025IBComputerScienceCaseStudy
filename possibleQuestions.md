Based on this part of the paper 3 (at the end) here there are several questions that you will find in the exam (probably written in another way)


![imagen](https://github.com/user-attachments/assets/3d3efa54-d541-4abb-b076-659ace5aacac)


* Evaluate three different ways of reducing the latency of the system
* Analyize the different stages of natural language processing and what are the useful inputs (for the context of the insurance company bot) that we can find at each step.
* Use in the previous question the example phrase "I want to fix a problem with my premium" (the premium is the fee that you pay monthly/yearly to an insurance company)
* Evaluate if a Transformer NN is better for processing language than a Recurring NN
* What would we need to have a good dataset for our insurance company?
* To what extend is ethical use a bot like this?
* What are the power requirements that we need to create a bot like this? (in comparassion with a human helpdesk)


Answers 
* Evaluate three different ways of reducing the latency of the system:

  In order to reduce the latency of a system, we can manage the dependencies. When these dependencies are tightly coupled (meaning they rely heavily on each other), they can create bottlenecks if one component is delayed or experiences an error. Reducing or decoupling dependencies can improve system performance and responsiveness by allowing different parts of the system to operate more independently. There can be three ways:
  * Use of the Natural language understanding (NLU) pipeline: the NLU pipeline can be used to transform unstructured text into machine-actionable information. On one hand, this helps to identify and filter out unnecessary models, leading to a reduced latency. The LU can also handle a wide variety of user inputs without requiring predefined commands, making it easier to scale up user interaction capabilities. Additionally, advanced NLU can maintain context over interactions, allowing it to predict and prefetch data related to previous user actions or queries and enabling faster responses to follow-up questions, as well as reducing repetitive dependency calls and enhancing user experience.
  However, on the other hand, many NLU solutions rely on third-party APIs (e.g., Google Dialogflow), meaning that there’s unpredictable latency if there are network issues or if the third-party service experiences downtime. Moreover, NLU models, especially complex ones, can require significant processing time to parse and understand inputs, potentially slowing down response time. Regarding privacy concerns, NLU systems often process and store user input data to improve accuracy. In cases where third-party services are used, sensitive information may be transferred externally. Privacy and security concerns can limit NLU’s usage, especially in sensitive applications, and might require additional security measures, which could further impact latency.

* Analyize the different stages of natural language processing and what are the useful inputs (for the context of the insurance company bot) that we can find at each step.

The five different stages of natural language processing are lexical analysis, syntactic analysis, semantic analysis, discourse integration, and pragmatic analysis. 
<br>
The lexical analysis and syntactic analysis try to understand the structural aspects of language. In lexical analysis, the input is broken down into words and sentences. In this step, the customer’s raw text is used as input. It is very useful to have an input in which the words are separated and not together. 
<br>
The syntactic analysis is about understanding the grammar of the sentence. For example: “He” is the subject, “ate” is a verb, and “poison” is the object. During this step, it is useful to have inputs where it follows the grammar of the sentences of the dataset that the model is trained on. So a sentence without a proper grammatical structure or numbers may not be useful during this step. The other three steps are focused on the understanding meaning of the language. 
<br>
After identifying the structure of the sentence, the model runs a semantic analysis. Here the model is trying to understand the meaning of the sentence. The model tries to derive an objective meaning rather than trying to interpret it in a wider context. The useful inputs here will be insurance-specific entities and concepts. 
<br>
The next step is discourse integration. Here, the model goes on to integrate the meaning of the sentence into the wider context of the whole conversation. This requires interpretations and can be more subjective. The useful inputs here will be the data of previous conversations within the chat or other chats, customer information, and any other recent queries that can all help the chatbot with more context, making the answer more accurate for the customer.
<br>
Lastly, the pragmatic analysis analyzes the social, legal, and cultural context of the sentence. In this case, context-specific knowledge, such as insurance policies or legal standards and typical scenarios are useful inputs. For instance, knowing that "make a claim" usually implies urgency which can guide the chatbot toward a helpful, sensitive response.
