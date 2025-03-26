# 🚀 Project Name - Context Aware Testing System 
 
## Team Name - Memory Overflow

## 📌 Table of Contents
- Demo videos are uploaded to artifacts.
- Architecture diagram uploaded to arch folder
- PPD Uploaded into the artifacts Folder
- (For reference ) Uploaded Generated Feature files and python test cases under (artifacts/Generated_BDD_PyTest)
- 

## Completed Items / Achievements
**Built and an Multi Agent system (Around 10 + Agents ) are working together 
And providing the complete AI Testing suit.**
1. BDD Test cases generated  based **Functional Document** + **API Document**(Swagger)
2. PyTest Test cases generation based on **BDD Feature files**  +**Functional Document** + **API Document**
3. Agents will Automatically identifying the Documents and mapping it with Swagger document
4. API Test Data Schema Identification before generating the test data
5. Agents having ability to Link between BDD files and Python Test Files
6. Proivded Ability for Agents to generate structured output for the modified Funcitonal document versions
7. Ability to identify difference between two functional document versions and understand the context
8. Agents will understand the  Testing Pre-Request Context to automatically setup the Test user and Authentication Context 
9. (If user wants) Ability for the users to modify the existing Feature files and update the test cases Using Gen AI Agent (Demo Added)
10. Agents having Self healing ability if there is any update/addition in  Functional Document or API Document and update the multiple BDD Files and PyTest Files

![Uploading image.png…]()



---
 
 

## 🛠️ How We Built It
 1. We Used Auto gen (Agentic AI Framework), RAG , Function Calling and Structured output. And used Open AI gpt-4o and gpt-3.5-turbo models.
 2. Used text-embedding-ada-002 for text embedding for RAG Agents
 3. Used PyTest for API test cases
 4. Used Chroma as Vector DB
 5. Requests - For API Calls
 6. And we used Structured ouput to identify the changes in the Funcitonal document for self healing
 7. Used difflib to identify the differences between two funcitonal documents

## 🚧 Challenges We Faced
My Open AI  Threashold limit reached. So i have Partially completed the demo video on Self Healing part. But other parts i have captured. If required i can show a live demo with some other LLM (from GROQ)
Not able to Upload complete Demo Video as the size exeeds the limit. So i have splitted it 12 video files and uploaded. please watch files in the order number provided

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
   - MODIFED_FUNCTIONAL_DOCS_PATH=<localsource code path>\GenAITester\documentsmodified  (For a  **SELF HEALING**  Copy the any modified/ updated funcitonal documentation files.  This will by used by RAG Agents)
   - OPENAI_API_KEY=<OpenAI Key>  (Name should be OPEN AI but initially miss spelled it )
3. Run the project  
   ```sh
   cd GenAITester
   python main.py
   ```
 
## 👥 Team
- **Saravana Manikandan Nagarajan** - [GitHub](#) | [LinkedIn](#)

