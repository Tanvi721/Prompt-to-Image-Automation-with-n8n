# 🎨 AI Image Generator with n8n (Form → AI Agent → DALL·E 3)

This project is an **end-to-end automated image generation workflow** built using **n8n**, **AI Agent**, and **OpenAI DALL·E 3**.  
Users simply enter a short text (title or concept) in a form, and the workflow automatically:

1. Receives input from an n8n Form  
2. Passes it to an AI Agent  
3. Converts it into a detailed image prompt  
4. Generates a high-quality AI image using DALL·E 3  
5. Displays the final output inside n8n  

---

## 📌 Features

- ✔ **User-friendly web form** for entering the image title/idea  
- ✔ **AI Agent transforms simple text into a detailed prompt**  
- ✔ **DALL·E 3 generates realistic, high-quality images**  
- ✔ **Fully automated workflow**  
- ✔ **Drag & drop workflow in n8n**  
- ✔ **Great for image creation tools, dashboards, automations, and demos**

---

## 🛠️ Workflow Structure


### **1️⃣ On Form Submission**
- Collects user input through an n8n form  
- Field used: `title`

### **2️⃣ AI Agent**
- Receives text and rewrites it into a creative image prompt  
- Example transformation:  

### **3️⃣ Generate an Image**
- Uses OpenAI DALL·E 3  
- Prompt is taken from AI Agent output:  

---

## 🧩 Prompt Used Inside the AI Agent

text
You are an AI image generator.

Take user input from the form ({{ $json.title }}) and convert it into a detailed image prompt including:
- main subject
- background
- lighting
- mood
- style (realistic / 3D / anime etc.)
- camera angle

# 📷 Workflow & Output
<img width="1920" height="1080" alt="Screenshot (229)" src="https://github.com/user-attachments/assets/d042cc61-a356-4f0a-9505-5f807a939a93" />
<img width="1920" height="1080" alt="Screenshot (231)" src="https://github.com/user-attachments/assets/15b9a6b4-035d-495a-b963-864ef6606a3c" />
<img width="1920" height="1080" alt="Screenshot (232)" src="https://github.com/user-attachments/assets/f3c791bd-4af2-4d10-b0e2-1cdfa52b8132" />
<img width="1920" height="1080" alt="Screenshot (233)" src="https://github.com/user-attachments/assets/74341c26-d878-4646-8174-f977d96349d4" />


# 📦 Technologies Used

+ n8n Automation

+ OpenAI DALL·E 3

+ AI Agent Node

+ OpenRouter / OpenAI models

+ n8n Form Trigger

# 🤝 Contributing

Feel free to submit issues, improvements, or pull requests!

# 📜 License

This project is open-source and available under the MIT License.




