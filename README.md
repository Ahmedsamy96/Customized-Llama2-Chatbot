# Customized-Llama2-Chatbot 🦙

## Repository's Into
We all as AI Engineers and generative AI enthusiasts believe that using openAI API in creating chatbots specified for specific businesses and many other tools, gives us state-of-the-art results. But we also know that this has concessions like : (service cost - our data blurry confidentiality state) so I spent about 2 months searching for a solution that is based on Open source models, open for commercial use.

Have you ever wanted to dispense with the ChatGBT API at all costs and find an open-source alternative available for commercial use??  
Yes, I am sure you have thought about this, but implementation may be more difficult later on, but here A strong competitor has appeared: (Llama 2 🦙).  

The idea is that I wanted to insert a CSV file into a model using vector store, available on langchain, in order to obtain a model that specializes in a specific business, has deep knowledge of its information, and is able to respond with specific answers, which is something that was a challenge for all models, no matter how many parameters they had or how large their architecture was.  It was difficult to achieve without using a convenient vector db and model quantization method.

## Notebook's WorkFlow:
Here you can see my project's workflow, so you can understand used tools and techniques Only by looking...
![LLM-diagram](https://github.com/Ahmedsamy96/Customized-Llama2-Chatbot/blob/main/LLM-diagram.drawio.png)


## Tools and technologies used:
- Vector db
- Langchain
- Llama 2 - 13b from hugging face
- Colab (GPU )
- Quantization using Qlora
