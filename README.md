Here's a clean and well-formatted `README.md` file based on your steps:

```markdown
# RAG-PDF: PDF-based Retrieval-Augmented Generation

This project allows users to upload PDFs and ask questions based on their content using RAG (Retrieval-Augmented Generation) with vector search and LLMs.

---

## 🛠 Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/SyedAbdullahAhmed/RAG-PDF.git
```

---

## 📁 Project Structure

- `client/` – Next.js frontend
- `server/` – Node.js backend with LangChain, Google GenAI, and Qdrant

---

## 🔧 Install Dependencies

### In **Terminal 1**:
```bash
cd RAG-PDF
cd server
npm install
```

### In **Terminal 2**:
```bash
cd RAG-PDF
cd client
npm install
```

---

## 🔑 Environment Setup

1. Create a `.env` file in the `server/` directory.
2. Add your **Gemini API key**:
   ```
   GEMINI_API_KEY=your_api_key_here
   ```

---

## 🐳 Docker Setup (Valkey, BullMQ, Qdrant)

Make sure you have Docker Desktop installed.

### In **Terminal 3**:
```bash
docker compose up -d
```

> This will start the required services in the background.

---

## 🚀 Run the App

Open **3 separate terminals** and run:

### Terminal 1 (Frontend):
```bash
cd client
npm run dev
```

### Terminal 2 (Backend API):
```bash
cd server
npm run dev
```

### Terminal 3 (Worker):
```bash
cd server
npm run dev:worker
```

---

## 🌐 Usage

1. Open your browser and go to [http://localhost:3000](http://localhost:3000)
2. Upload a PDF file.
3. Ask questions based on the content of the uploaded PDF.

---

## 📦 Tech Stack

- **Frontend:** Next.js, Tailwind CSS
- **Backend:** Node.js, LangChain, Google GenAI
- **Database:** Qdrant (vector DB), Valkey (Redis fork for queues)
- **Queue:** BullMQ
- **Deployment:** Docker Compose

---

## 📄 License

MIT
```

Let me know if you want badges, screenshots, or contribution guidelines added too.
