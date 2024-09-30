
# HogwartsBot-RAG based LLM app for Potterheads
This project is a simple Retrieval-Augmented Generation based Q&A application specially designed for Potterheads. The project has uses Pathway LLM-app framework.
Pathway framework is a Python data processing framework for analytics and AI pipelines over data streams. It’s the ideal solution for real-time processing use cases like streaming ETL or RAG pipelines for unstructured data and LLM applications. 
## About the Project 
This LLM App has a  `/data` storage in which all 7 Harry Potter books are present which provide context to the LLM for giving accurate Harry-Potter based answers.
### Key Features : 
- **Harry Potter Knowledge Base**: Understands and responds to questions related to characters, events, and lore from all seven Harry Potter books.
- **RAG-Based Architecture**: Combines retrieval and generation capabilities to ensure answers are contextually relevant.
- **Contextual Conversations**: Provides intelligent and fact-based responses using LLM capabilities and document search.
- **Modular Design**: Separate modules for retrieval, generation, and response synthesis.
# Demo Usage
Here's the link to the demo use of this application.
# Installation
To set-up HogwartsBot, follow the steps below:

- Clone the repository in your **VSCode terminal**:

    `git clone https://github.com/KaranS2111/HogwartsBot_RAG_LLM`

- Run the application using **Docker**:

    `docker build -t hbot`\
    `docker run -p 8000:8000 hbot`
    
    Running the docker container may take upto 3-4 minutes.
- Use either Postman or ThunderClient API service to give prompt requests:
 
    URL : `http://localhost:8000/v1/pw_ai_answer`
    
    - Here's how to do it in **Thunder Client**:

        - Set the **HTTP** method to **POST**.
        - Go to the **Headers** tab.
        - Add a header with:

                Key: Content-Type
                Value: application/json
        Setting the Content-Type as `application/json` is necessary for most APIs to correctly parse and understand the JSON data you send in the request body.

        - **Body**: Click on the Body tab, select JSON format, and enter the following JSON:

                {
                    "prompt": "Hey Potterhead! Ask your question!"
                }



# License
This project is licensed under the MIT License. See the **LICENSE** file for more details.

# Contributing
Contributions are welcome! If you have suggestions or improvements, feel free to submit a pull request.

