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

```text
You are an AI image generator.

Take user input from the form ({{ $json.title }}) and convert it into a detailed image prompt including:
- main subject
- background
- lighting
- mood
- style (realistic / 3D / anime etc.)
- camera angle

# 📷 Screenshots


