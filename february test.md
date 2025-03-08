_This was set on a mock exam_

 

 1)   Define the term vanishing gradient [2] 

 2)   Outline the relationship between the critical path of the decision algorithm and dependencies of the system [2] 

 3)   Describe the bag-of-words algorithm [4] 

 4)   Describe the relationship between the linguistic analysis and the algorithm of a Transformer Neural Network [4] 

 5)   Discuss if the preprocessing of data can improve the latency of the model or improve its efficiency [6] 

 6)   Discuss the ethical implications of using a chatbot for RAKT and how could be tackled (if they can be tackled). [12] 

 
Markbands

![imagen](https://github.com/user-attachments/assets/641f4821-0a63-47f2-8da7-b2480e1b853c)


Notes on 6. 

## Data anonymization 

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
