# PySD Model Simulator API

This is a FastAPI-based REST API to run and interact with PySD-compatible system dynamics models (.mdl or .xmile files). It includes support for GPT action integration and deployment on Render.

---

## 🌐 Deployment on Render

### 1. Upload to GitHub
Push this repository to GitHub:
```bash
git init
git remote add origin https://github.com/your-username/your-repo.git
git add .
git commit -m "Initial commit"
git push -u origin main
```

### 2. Deploy on Render
1. Go to [https://render.com](https://render.com)
2. Create a **New Web Service**
3. Connect your GitHub repo
4. Render will detect `render.yaml` and auto-deploy the API

---

## 🤖 Use as a Custom GPT Plugin

### Plugin Files:
- `.well-known/ai-plugin.json`
- `static/openapi.yaml`

### Example Manifest URL:
```
https://your-app.onrender.com/.well-known/ai-plugin.json
```

### Steps to Integrate:
1. Open [ChatGPT > Explore GPTs > Create a GPT](https://chat.openai.com/gpts)
2. Under **"Actions"**, click **"Add"** and enter the Manifest URL above
3. Save your GPT and test it with prompts like:
   - "Upload a system dynamics model"
   - "Run the model with 10% higher birth rate"
   - "Show stocks and flows of the loaded model"

---

## 🛠️ Project Structure

```
render-api-deploy/
├── main.py
├── requirements.txt
├── Procfile
├── render.yaml
└── static/
    ├── openapi.yaml
    └── .well-known/
        └── ai-plugin.json
```

---

## 📧 Contact

- Email: your-email@example.com
- Website: https://your-website.com

