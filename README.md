# flowise-project
CCSW 325 - Flowise (Category C) LLM orchestration project + replication package

Problem Statement:
Hospitals and clinics receive frequent patient questions about specialty availability, on-duty doctors, and appointment options, but these inquiries are often handled through a call center limited to working hours. This creates delays during peak times, reduces access at night/weekends/holidays, and increases repetitive workload on staff. Our project automates these inquiries using a Flowise-based assistant that provides consistent 24/7 responses about available specialties and doctors based on hospital-provided data, improving response time and reducing dependence on call-center availability
 Solution Overview:![Solution ](docs/images/ImplementationWalkthrough(Step-by-Step).pdf)
 
 Implementation Walkthrough: ![Architecture](docs/images/Architecturediagram.jpg)

 How to Run (Flowise Cloud)
1.	Log in to Flowise Cloud and open the Chatflow ![Chatflow](flowise/export/CustomerServiceChatflow.json.png) ,press add new then load the the chatflow file .
2.	Go to Credentials and add/select your GoogleAI (Gemini) API Key.
3.	Ensure the credential is selected in both nodes: ChatGoogleGenerativeAI and GoogleGenerativeAI Embeddings.
4.	Verify key settings: Text Splitter (Chunk Size 800, Overlap 120), Embeddings model gemini-embedding-001 with RETRIEVAL_DOCUMENT, and Vector Store Top K = 4.
5.	Click Save, then open Chat Preview/Test Chat.
6.	Ask a question (e.g., “What is the WhatsApp number?”) and confirm the bot responds using the stored clinic information.
   
    Demo : ![DEMO](docs/images/demo_result_video.mp4)
