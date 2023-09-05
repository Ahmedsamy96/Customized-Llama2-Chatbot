# Customized-Llama2-Chatbot 🦙

## Repository's Intro: 🤷‍♂️🤷‍♂️
We all as AI Engineers and generative AI enthusiasts believe that using openAI API in creating chatbots specified for specific businesses and many other tools, gives us state-of-the-art results. But we also know that this has concessions like : (service cost - our data blurry confidentiality state) so I spent about 2 months searching for a solution that is based on Open source models, open for commercial use.

Have you ever wanted to dispense with the ChatGBT API at all costs and find an open-source alternative available for commercial use??  
Yes, I am sure you have thought about this, but implementation may be more difficult later on, but here A strong competitor has appeared: (Llama 2 🦙).  

The idea is that I wanted to insert a CSV file into a model using vector store, available on langchain, in order to obtain a model that specializes in a specific business, has deep knowledge of its information, and is able to respond with specific answers, which is something that was a challenge for all models, no matter how many parameters they had or how large their architecture was.  It was difficult to achieve without using a convenient vector db and model quantization method.

## Projects' Steps: 🪜🚶‍♂️
1. **Efficient Model Loading and Configuration:** The notebook defines and loads a pre-trained language model, configuring it for efficient use of GPU memory. It also sets up authentication for accessing the Hugging Face model repository.
2. **Tokenization and Stop List Preparation:** Tokenization and stop list preparation are crucial for handling text inputs. The notebook utilizes the Hugging Face tokenizer to generate tokens and IDs for special text sequences. It defines a custom stopping criteria for generating responses.
3. **Text Generation Pipeline:** A text generation pipeline is established using the loaded model and tokenizer. It incorporates parameters such as temperature and repetition penalty to control the randomness and quality of generated responses.
4. **Data Loading:** The notebook loads a CSV file containing Q&A pairs, which serves as the knowledge base for the chatbot. It previews the loaded data and selects a subset for processing.
5. **Embeddings and Vectorization:** Text embeddings are generated using a pre-trained Sentence Transformers model, and a vector store is created using FAISS to facilitate efficient retrieval of relevant responses.
6. **Conversational Retrieval Chain:** The chatbot's retrieval chain is set up, combining the text generation pipeline, vector store, and custom stopping criteria. This enables the chatbot to respond to user queries based on the loaded knowledge base.
7. **User Interface Deployment:** The notebook concludes by creating a user interface for the chatbot using Gradio. Users can interact with the chatbot by entering questions related to physical distancing, and the chatbot provides informative responses.


## Notebook's WorkFlow: 🎴🕸️
Here you can see my project's workflow, so you can understand used tools and techniques Only by looking...
![LLM-diagram](https://github.com/Ahmedsamy96/Customized-Llama2-Chatbot/blob/main/LLM-diagram.drawio.png)


## Tools and technologies used: 🔨✂️
- Vector store (FIASS)
- Langchain
- Llama 2 - 13b from hugging face
- Colab (GPU T4)
- 4bit Quantization using BitsAndBytesConfig

## Results and inference: 🍰🍰
Now let's Notice the results...
![Result1](https://github.com/Ahmedsamy96/Customized-Llama2-Chatbot/blob/main/Screenshot%202023-09-04%20104751.png)
