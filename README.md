

# 🎬 Pikuchoice - AI-Powered Movie Recommendation App 🍿

Pikuchoice is a smart movie recommendation web app that suggests movies based on user preferences. It leverages **OpenAI embeddings** and **Supabase vector search** to find the best matching movies.

## 🚀 Features
- ✅ AI-powered movie recommendations
- ✅ Vector search using **Supabase**
- ✅ Clean and user-friendly UI
- ✅ Works with any framework or library

## 📜 Requirements
- **Node.js** (for backend API requests)
- **Supabase account** (with a `movie_embeddings` table)
- **OpenAI API Key**
- **Supabase API Key & URL**

## 🛠️ Setup & Installation
1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/pikuchoice.git
   cd pikuchoice
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Set up environment variables**  
   Create a `.env` file in the root directory and add:
   ```
   OPENAI_API_KEY=your_openai_api_key
   SUPABASE_URL=your_supabase_url
   SUPABASE_API_KEY=your_supabase_api_key
   ```

4. **Run the app**  
  https://pikuchoice.vercel.app/

## 🎯 How It Works
1. The user inputs their movie preferences (favorite movie, mood, fun/serious).
2. The app generates an **AI embedding** of the input using OpenAI.
3. The **Supabase vector database** finds the most similar movies.
4. The best-matched movies are displayed as recommendations.

## 🏗️ Tech Stack
- **Frontend**: React
- **Backend**: OpenAI API, Supabase Vector DB
- **Database**: Supabase (`movie_embeddings` table for storing movie vectors)

## 📌 Supabase Table Structure (`movie_embeddings`)
| Column   | Type     | Description |
|----------|---------|-------------|
| id       | UUID    | Unique ID |
| title    | Text    | Movie title |
| year     | Integer | Release year |
| genre    | Text    | Movie genre |
| embedding | Vector | OpenAI-generated vector |

## 🎥 Screenshots
![Pikuchoice UI](screenshot.png)

## 💡 Future Enhancements
- 🔹 Improve search accuracy with better embeddings
- 🔹 Add more filters (e.g., genre, language)
- 🔹 Create a mobile-friendly UI

## 🤝 Contributing
1. Fork the repo
2. Create a feature branch (`git checkout -b feature-name`)
3. Commit your changes (`git commit -m "Added new feature"`)
4. Push to the branch (`git push origin feature-name`)
5. Open a **Pull Request**

## 📜 License
This project is licensed under the **MIT License**.

---
💡 *Made with ❤️ for movie lovers!* 🍿🎬
```
