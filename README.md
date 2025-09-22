# Myntra Expressway – Smart Fashion Assistant 🚀

Myntra Expressway is an AI-powered **fashion planner and shopping companion** that helps users stay **event-ready, budget-friendly, and socially stylish**.  
It combines **event-based outfit planning**, **wardrobe matching**, and **group shopping** into one seamless experience.  

---

## 🔥 Features

---

### 1. 🗓️ Style Scheduler  
The **Style Scheduler** acts as your **personal stylist calendar**.  
- Sync or add events (wedding, birthday, office party, interview, festival).  
- AI curates **complete outfits** tailored to the occasion.  
- Smart reminders (T-10, T-5, T-2 days) so you never miss an event look.  
- Expressway-eligible suggestions ensure delivery before the event.  
- Optional AR try-on to preview the look.  

📸 *Screenshot / UI Mockup Placeholder*  
![Style Scheduler Screenshot](./screenshots/style-scheduler.png)  

---

### 2. 👕 Wardrobe Matcher  
The **Wardrobe Matcher** ensures **cost-friendly shopping** by using what you already own.  
- Upload your wardrobe (photos) or auto-sync past Myntra purchases.  
- AI suggests only **missing pieces** to complete the look.  
- Smart mix-and-match recommendations to reuse clothes.  
- Three tiers of suggestions:  
  - Budget-friendly (reuse more)  
  - Mid-range  
  - Premium (fresh new look)  

📸 *Screenshot / UI Mockup Placeholder*  
![Wardrobe Matcher Screenshot](./screenshots/wardrobe-matcher.png)  

---

### 3. 👯 Group Shopping  
The **Group Shopping** feature enables **social styling** for events.  
- Create groups with friends, colleagues, or family.  
- AI suggests **coordinated outfit sets** (themes, colors, styles).  
- Great for weddings, parties, team functions, or festive events.  
- Shared cart and optional **cost-split checkout**.  
- Enhances engagement and builds community around fashion.  

📸 *Screenshot / UI Mockup Placeholder*  
![Group Shopping Screenshot](./screenshots/group-shopping.png)  

---

## 🌟 Advantages

### Customer Benefits
- Proactive fashion planning with event alerts.  
- Cost-efficient → buy only missing items.  
- Confidence with AR try-on and curated looks.  
- Social engagement through group shopping.  

### Business Benefits
- Higher user engagement and retention.  
- Increased Average Order Value (AOV).  
- Seasonal trend insights via event data.  
- Competitive advantage in fashion e-commerce.  

---

## 🛠️ Tech Stack

- **Frontend**: React.js, Tailwind CSS, Figma (UI design)  
- **Backend**: Node.js,FastAPI + Uvicorn  
- **Database**: MongoDB / PostgreSQL  
- **AI Models**:  
  - [CLIP](https://huggingface.co/openai/clip-vit-base-patch32) for outfit embeddings  
  - [Sentence-Transformers](https://www.sbert.net/) for NLP-based search & event analysis  
- **Vision & Color**: PIL + NumPy + custom color matching 

---

## ⚙️ Installation / Setup

```bash
# Clone repository
git clone https://github.com/yourusername/myntra-expressway.git
cd myntra-expressway

# Install backend dependencies
cd backend
npm install

# Install frontend dependencies
cd ../frontend
npm install

# Run backend server
cd ../backend
npm start

# Run frontend
cd ../frontend
npm start

#Setup for AI Layer

cd Recommendation_Model
pip install -r requirements.txt
python extract_data.py
uvicorn app:app --reload --host 0.0.0.0 --port 8000



