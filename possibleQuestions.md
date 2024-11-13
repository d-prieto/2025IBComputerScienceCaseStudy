Based on this part of the paper 3 (at the end) here there are several questions that you will find in the exam (probably written in another way)


![imagen](https://github.com/user-attachments/assets/3d3efa54-d541-4abb-b076-659ace5aacac)


* Evaluate three different ways of reducing the latency of the system
* Analyize the different stages of natural language processing and what are the useful inputs (for the context of the insurance company bot) that we can find at each step.
* Use in the previous question the example phrase "I want to fix a problem with my premium" (the premium is the fee that you pay monthly/yearly to an insurance company)
* Evaluate if a Transformer NN is better for processing language than a Recurring NN
* What would we need to have a good dataset for our insurance company?
* To what extend is ethical use a bot like this?
* What are the power requirements that we need to create a bot like this? (in comparassion with a human helpdesk)


## Answers (by students)


* Evaluate three different ways of reducing the latency of the system:

  In order to reduce the latency of a system, we can manage the dependencies. When these dependencies are tightly coupled (meaning they rely heavily on each other), they can create bottlenecks if one component is delayed or experiences an error. Reducing or decoupling dependencies can improve system performance and responsiveness by allowing different parts of the system to operate more independently. There can be three ways:
  * Use of the Natural language understanding (NLU) pipeline: the NLU pipeline can be used to transform unstructured text into machine-actionable information. On one hand, this helps to identify and filter out unnecessary models, leading to a reduced latency. The LU can also handle a wide variety of user inputs without requiring predefined commands, making it easier to scale up user interaction capabilities. Additionally, advanced NLU can maintain context over interactions, allowing it to predict and prefetch data related to previous user actions or queries and enabling faster responses to follow-up questions, as well as reducing repetitive dependency calls and enhancing user experience.
  However, on the other hand, many NLU solutions rely on third-party APIs (e.g., Google Dialogflow), meaning that there’s unpredictable latency if there are network issues or if the third-party service experiences downtime. Moreover, NLU models, especially complex ones, can require significant processing time to parse and understand inputs, potentially slowing down response time. Regarding privacy concerns, NLU systems often process and store user input data to improve accuracy. In cases where third-party services are used, sensitive information may be transferred externally. Privacy and security concerns can limit NLU’s usage, especially in sensitive applications, and might require additional security measures, which could further impact latency.
  * Implementing asynchronous processing:
  * Use dependency caching: 


----
Evaluate three different ways of reducing the latency of the system

1) Latency is...
2) Smaller versions- reduce latency - but..
3) Training - reduce latency - but..
4) Critical path - what is it- how it reduces
5) Conclusion


Latency refers to a delay or lag in response time and can be faced in different systems such as chat bots.
It takes a vast network of machine learning models for conversational artificial intelligence (AI) to 
determine what to say next, with each model solving a small piece of the puzzle. One model might 
take the user’s location into account, while another could analyze the history of user interactions, 
including the feedback provided by users on similar responses. Every model should add 
improvement but at the cost of increasing the system’s latency.

One way to overcome latency is to use smaller modules of IA. For example chat GPT -4o mini, that is a more efficient and slightly smaller version of GPT-4, optimized to perform faster while using fewer resources. The latency would be decreased, however the reply won't be that deep and explained as in a bigger version.
 
Training a chatbot is another step towards improving a chatbot’s ability to understand text that then reduce response time. The training dataset needs to be large, accurate, classified, readable, domain specific and relevant. A well-designed training dataset can improve the chatbot’s response quality and indirectly reduce latency by reducing the amount of time needed to process and interpret user inputs.

That latency is a product of a decision algorithm known as the “critical path”, which is the shortest 
and most efficient sequence of linked machine learning models required to go from the input of the 
user’s message to the output of the chatbot’s response. It is known that changes to one model can 
impact larger machine learning networks with machine learning dependencies.
 One way to overcome dependencies is to transform unstructured text into machine-actionable 
information. Natural language understanding (NLU) is a pipeline created through many machine 
learning models that carry out different functions to improve the chatbot’s understanding of user 
input. This helps to identify and filter out unnecessary models, leading to a reduced latency.
 

In conclusion all the methods above help to reduce latency for an IA system, however all of them require specific features (and difficulties) in return.

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

To what extend is ethical use a bot like this?
Answer:
In order to ethically use this bot there are a few conditions that developers must adhere to. 
The first condition is constant moderating and checking of paterns. This is to ensure that the bot is not biased and does not give discriminatory answers. This is quite important for users. 
Another very important thing for me is security and privacy. Every user is very much concerned about their data. So the developer should minimize the requests for any information to avoid conflicts. Also if there is any data collection then the user should be aware of it and he should agree to it.

Also the important thing is to check the information for fake. In order for the bot to be safe to use the developer must implement information verification in it. After all, if this does not happen, the user will be misled.

In summary, I can say that the bot is ethical to use if the above conditions are met. 

Answer 2:
<br>
The extend of how ethical it is to use a bot like this depends largely on the situation. In the case study, the context the bot is used it is accident reports. 
<br>
One of the first things to worry about is old datasets. In order to make an informed decision, the bot analyses previous responses to similar reports from databases it has access to. Go far enough in the databases, and you will find that, historically, when such requests were handled by people, there was bias based upon various factors: ethnicity, socioeconomic position, and gender. Because the bot doesn't know any better, and because it bases its decisions on precedent, the answers it gives to the report made will be biased if the reporter's ethnicity, socioeconomic position or gender are historically marginalized. An easy way to solve this, would be to ignore such factors to begin with. However, by doing this, we ignore possible benefits depending on such factors. For instance say that due to the socioeconomic position of a client (ex: unemployed) he gets a bonus, if we ignore this factor, the bonus would not be given to him. There is no easy way to fix this, and there is only so much programming that can be done to get around it. 
<br>
Another ethical point is the question of accountability. If the bot makes a mistake, who does the client complain to? Mistakes are especially hard to fix, because the bot does not admit to them. You can't report a mistake if it doesn't register as one. Also, because the bot is not human, no matter what they do (say, loose a large amount of money during transaction) you cant sue them, because they're just machines. You could sue the programmers. But just like the bot can avoid responsibility, so can they, by resting responsibility solely on the bot's feet. Moreover, because of how literal the bot is, its most likely to overreact. For examples, if a customer is angry says something like they're going to kill the person who messes up their car, the bot could register this as the intent to commit a crime, and report it to the police. Causing problems for the customer, who was clearly exaggerating. 
<br>
What would we need to have a good dataset for our insurance company?
  To ensure that the insurance company will have a good dataset we need to determine the accuracy, responsiveness and overall user experience of the chatbot. As the company has right now poorly trained chatbot which needs to have more diverse dataset. This can be done by focusing on domain specific data, data diversity, labeling accuracy and ethical considerations.
Domain specific data will ensure that chatbot will deliver accurate responses. This will include insurance claims, customer service interactions, policy documents. By having domain specific data we ensure that the responses will be both accurate and relevant to the context.
Chatbot to be successful needs to have diverse and high quality data. This involves the data to be specific to the intended purpose and well as incorporating wider data from different geographical locations which reduces the risk of having bias present. By having multiple servicing on the chatbot we can assure that the chatbot won´t have biases and if so they will be removed.
Chatbot´s dataset will include real world scenarios as well as synthetic data which will assure to simulate rare occasions for which the chatbot might not have been well enough prepared for.
The accurate data labeling will be important as it helps chatbot to correctly interpret and respond to the customer's needs. This would help with avoiding general responses that do not respond specifically to the questions asked. 

