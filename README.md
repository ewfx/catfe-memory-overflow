# 🚀 Project Name - Context Aware Testing System 
![Uploading image.png…]()
## Team Name - Memory Overflow

## 📌 Table of Contents
- Demo videos are uploaded to artifacts.
- Architecture diagram uploaded to arch folder 
- This application can perfrom
  1. BDD Feature file generation based on Functional Documentaiton and OpenAPI (Swagger Documentation)
  2. Able to Generate the PyTest Test cases for API
  3. Gen AI help to update the existing Test cases/ BDD  feature files
  4. Self healing the BDD Feature file and  PyTest Test Cases


---
 
 

## 🛠️ How We Built It
 1. We Used Auto gen (Agentic AI Framework), RAG , Function Calling and Structured output. And used Open AI gpt-4o and gpt-3.5-turbo models.
 2. Used text-embedding-ada-002 for text embedding for RAG Agents
 3. And we used Structured ouput to identify the changes in the Funcitonal document for self healing
 4. Used difflib to identify the differences between two funcitonal documents

## 🚧 Challenges We Faced
My Open AI  Threashold limit reached. So i have Partially completed the demo video on Self Healing part. But other parts i have captured. If required i can show a live demo with some other LLM (from GROQ)

## 🏃 How to Run
1. Clone the repository  
   ```sh
   [git clone https://github.com/your-repo.git](https://github.com/ewfx/catfe-memory-overflow.git)
   ```
2. Install dependencies  
   ```sh
   pip install -r requirements.txt
   ```
4. Environment Configuration
    Create .env file at the root and configure below env variables   
   - BDDFILESPATH=<localsource code path>\pytestexplore\generated\bdd\      (This where the BDD feature files and python test case files will be generated)
   - FUNCTIONAL_DOCS_PATH=<localsource code path>\GenAITester\documents     (Copy required funcitonal documentations for API/ Microservice applicaiton. This will by used by RAG Agents)
   - MODIFED_FUNCTIONAL_DOCS_PATH=<localsource code path>\GenAITester\documentsmodified  ( **SELF HEALING**  Copy the any modified/ updated funcitonal documentation files.  This will by used by RAG Agents)
   - OPENAI_API_KEY=<OpenAI Key>  (Name should be OPEN AI but initially miss spelled it )
3. Run the project  
   ```sh
   cd GenAITester
   python main.py
   ```

## 🏗️ Tech Stack
- 🔹 Frontend: React / Vue / Angular
- 🔹 Backend: Node.js / FastAPI / Django
- 🔹 Database: PostgreSQL / Firebase
- 🔹 Other: OpenAI API / Twilio / Stripe

## 👥 Team
- **Your Name** - [GitHub](#) | [LinkedIn](#)
- **Teammate 2** - [GitHub](#) | [LinkedIn](#)
