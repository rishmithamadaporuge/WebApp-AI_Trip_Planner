# 🌍 AI Trip Planner WebApp

<p align="center">
  <img src="path/to/your/logo.png" alt="AI Trip Planner Logo" width="200"/>
</p>

An intelligent, full-stack web application that generates travel itineraries using the OpenAI API. Users supply destinations, travel dates, and preferences, and the app returns a personalized travel plan—complete with daily schedules, points of interest, and optional maps.

---

## 🚀 Features

- **Intelligent itinerary generation** using the OpenAI GPT model  
- **Interactive search UI** for destinations, dates, and travel preferences  
- **Customizable user inputs**: accommodation type, pace, budget, interests  
- **Attractive itinerary display** with map embeds and list views  
- **Downloadable itinerary** (e.g., PDF or JSON export)  
- **Responsive layout** for both desktop and mobile  
- **Backend API** built with Node.js + Express  
- **Secure API key handling** using environment variables  
- **Modular, maintainable codebase** with clear separation of concerns

---

## 🧠 Tech Stack

| Layer             | Technologies                             |
|------------------|-------------------------------------------|
| Frontend         | React.js (+ Hooks), Axios, Bootstrap/Tailwind |
| Backend          | Node.js, Express, OpenAI SDK              |
| Database (optional) | MongoDB / PostgreSQL                  |
| Deployment       | Heroku / Vercel / AWS                     |
| Environment      | `.env` for OpenAI API key and config      |

---

## 🎯 Getting Started

### Prerequisites

- Node.js v14+
- npm or Yarn
- OpenAI API key (from [OpenAI Dashboard](https://platform.openai.com/account/api-keys))

### Installation

1. **Clone the repo:**
   ```bash
   git clone https://github.com/rishmithamadaporuge/WebApp-AI_Trip_Planner.git
   cd WebApp-AI_Trip_Planner
   ```

2. **Install dependencies:**
   ```bash
   cd client && npm install && cd ../server && npm install
   ```

3. **Create environment variables:**

   - In the **server** folder:
     ```bash
     cp .env.example .env
     # Fill in your OPENAI_API_KEY, and other settings if needed
     ```

4. **Start the app in development mode:**
   - In one terminal (frontend):
     ```bash
     cd client
     npm start
     ```
   - In another (backend):
     ```bash
     cd server
     npm run dev
     ```

5. **Open your browser:**
   Navigate to `http://localhost:3000` and begin planning your trip!

---

## 🛠️ How It Works

1. The **frontend** collects user input: destination, dates, preferences.
2. On “Plan My Trip,” the frontend hits the **backend API** (e.g. `POST /api/plan`) with the payload.
3. The **backend** uses OpenAI’s GPT-4 or GPT-3.5 model, with a structured prompt instructing:
   - Break the trip down by day
   - List must-see attractions, dining options, transit tips
   - Stay within user’s pace, budget, and preferences
4. The **response** is parsed and returned to the frontend.
5. Frontend **renders** a visually appealing itinerary with days, times, map markers, etc.
6. Users can **export** or print their itinerary for offline use.

---

## 📦 Production Build & Deployment

1. In each of the `client/` and `server/` directories, run:
   ```bash
   npm run build
   ```
2. Deploy your **server build** to Heroku, AWS, or Vercel serverless functions.
3. Serve your **frontend static build** (from `client/build/`) via Netlify, Vercel, or an S3 bucket + CloudFront.
4. Set environment variables for production:
   - `OPENAI_API_KEY`
   - any other secrets (e.g. database URLs)

---

## 🧪 Testing

- **Unit tests:** Mocha/Chai or Jest (server-side)
- **Component tests:** React Testing Library (frontend)
- Add test scripts in `package.json` and run via `npm test`.

---

## 💡 Customization Ideas

- Support **multiple-stop trips** or multi-city routes
- Add **user authentication** and save past trips
- Integrate with **flight/hotel search APIs** for live pricing
- Optimize prompts with **advanced OpenAI features** like embeddings
- Add a **downloadable PDF generator** powered by Puppeteer

---

## ✍️ Contributing

Pull requests and issue reports are welcome!

1. Fork the repo  
2. Create a feature branch (`git checkout -b feature/YourIdea`)  
3. Commit your changes (`git commit -m "Add feature XYZ"`)  
4. Push (`git push origin feature/YourIdea`) and open a PR  
5. Be sure to follow existing code style and add tests where feasible

---

## 📝 License

MIT © [Your Name or Organization]

---

## 🙏 Acknowledgements

- Built using [OpenAI API](https://openai.com)
- Inspired by community‑driven travel planning tools

---

## 📬 Contact

- **Author**: Rishi Thamadapo<br/>
- **Email**: risham@example.com  
- **GitHub**: [@rishmithamadaporuge](https://github.com/rishmithamadaporuge)

Include a link to your website or demo here if available.

---

**Enjoy building your AI Trip Planner!** 🎉
```

---

### Tips for customization:

- Replace placeholder values (e.g. email, author).
- Add any extra **badges** (like build status, license, NPM version).
- Insert screenshots or GIFs inside the markdown after the logo section.
- Remove features you haven’t implemented yet, or expand sections that need more detail.

Let me know if you'd like help adding code snippets, prompt examples, or improved deployment guides!
