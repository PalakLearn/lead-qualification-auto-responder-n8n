[llama3-lead-qualifier-prompt.json](https://github.com/user-attachments/files/21351592/llama3-lead-qualifier-prompt.json)# lead-qualification-auto-responder-n8n
AI-based lead qualification and auto-responder workflow built in n8n using OpenAI and Slack
# 📬 Lead Qualification & AI Auto-Responder (n8n)

##  Objective  
Qualify website form leads automatically using AI, send personalized responses, and alert sales for high-intent prospects — all in real-time.

##  Tools Used  
- n8n (workflow automation)  
- OpenAI GPT-4 (intent analysis + response personalization)  
- Gmail/Outlook (email sender)  
- Slack (sales notification)  
- Typeform / HubSpot (form trigger)

##  Workflow  
1. Webhook receives form submission  
2. OpenAI evaluates the message (urgency, category, fit)  
3. Personalized email response is generated and sent  
4. If marked as hot, a Slack message is sent to Sales  
5. All data is logged for tracking

## 📈 Outcomes  
- 2-minute lead response time  
- Zero manual effort for first touch  
- Increased lead conversion via relevance  
- Prioritized hot leads for faster sales response

##  Files Included  
- `lead-qualification-flow.json`  [Up{
  "model": "meta-llama/Llama-3-8b-chat-hf",
  "messages": [
    {
      "role": "system",
      "content": "You are a lead qualification assistant. Based on the following message, classify it into one of these: 'Hot Lead', 'Warm Lead', or 'Cold Lead'. Only reply with the category."
    },
    {
      "role": "user",
      "content": "Name: John Smith Email: john.smith@example.com Message: I’m ready to purchase your product. Can someone contact me today to discuss the next steps?"
    }
  ],
  "temperature": 0.2,
  "max_tokens": 50,
  "top_p": 1,
  "stop": [],
  "stream": false
}
[Uploading llama3-lead-qualifier-prompt.json…]()

- `lead-analysis-openai.txt`  
- `personalized-response-email.txt`  
- `slack-hot-lead-alert.png`

##  Visuals 

<img width="840" height="159" alt="Screenshot 2025-07-21 221452" src="https://github.com/user-attachments/assets/9a17d55f-f48f-45ab-a00b-cbfb302d36c1" />
<img width="1530" height="842" alt="Screenshot 2025-07-21 223053" src="https://github.com/user-attachments/assets/f52e23b4-6fc5-40f2-b427-3d17cbf4ffe6" />
<img width="1520" height="807" alt="Screenshot 2025-07-21 222120" src="https://github.com/user-attachments/assets/e61d060f-a199-435c-8978-2288ffc3e6a1" />
<img width="917" height="292" alt="Screenshot 2025-07-21 222537" src="https://github.com/user-attachments/assets/d320a66a-948a-4ffa-b862-44e049235111" />
<img width="1093" height="463" alt="Screenshot 2025-07-21 222839" src="https://github.com/user-attachments/assets/d4c867e9-e0f2-463f-ace7-d1c698dced82" />

## ✍️ Author
Palak Chaturvedi  
[LinkedIn](https://linkedin.com/in/palak-chaturvedi) | [Portfolio](https://www.notion.so/Lead-Qualification-AI-Auto-Responder-237080ad24ae80cc8b15e878f455fc78)


