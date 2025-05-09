```markdown
# RAG-PDF

A PDF-based Retrieval-Augmented Generation (RAG) project using Node.js (backend) and Next.js (frontend), with Google Gemini API and Clerk for authentication.

---

## 🔧 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/SyedAbdullahAhmed/RAG-PDF.git
```

---

### 2. Install Dependencies

#### Terminal 1 (Backend)

```bash
cd RAG-PDF
cd server
npm install
```

#### Terminal 2 (Frontend)

```bash
cd RAG-PDF
cd client
npm install
```

---

### 3. Set Up Environment Variables

#### Backend (`server/.env`)
Create a `.env` file and add your **Gemini API key**:

```env
GEMINI_API_KEY=your_gemini_api_key_here
```

#### Frontend (`client/.env.local`)
Create a `.env.local` file and add your **Clerk project keys**:

```env
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key_here
CLERK_SECRET_KEY=your_clerk_secret_key_here
```

---

### 4. Install Docker Desktop

Download and install [Docker Desktop](https://www.docker.com/products/docker-desktop/) for your system. It is used to run:
- Valkey (for BullMQ queue)
- Qdrant (for vector DB)

---

### 5. Start Docker Containers

Open a **new terminal** and run:

```bash
docker compose up -d
```

This will start all services in the background.

---

### 6. Run the App (in 3 Terminals)

#### Terminal 1 (Frontend)

```bash
cd RAG-PDF/client
npm run dev
```

#### Terminal 2 (Backend)

```bash
cd RAG-PDF/server
npm run dev
```

#### Terminal 3 (Worker)

```bash
cd RAG-PDF/server
npm run dev:worker
```

---

### 7. Open in Browser

Go to: [http://localhost:3000](http://localhost:3000)  
Upload your PDF and start asking questions!

---

## 🧠 Features

- Upload PDFs and ask context-aware questions.
- Uses Google Gemini API for embeddings and chat.
- Clerk integration for user authentication.
- Vector search powered by Qdrant.
- Job queue with BullMQ and Valkey (Redis alternative).

---

## 🐳 Docker Containers Used

- `valkey` – For BullMQ jobs
- `qdrant` – For vector storage and retrieval

---

## 📦 Tech Stack

- **Frontend:** Next.js, Clerk, TailwindCSS
- **Backend:** Node.js, Express, LangChain, Google Generative AI
- **Queue & DB:** BullMQ, Valkey, Qdrant

---

Feel free to contribute or raise issues in the repository.
```


![image](https://github.com/user-attachments/assets/f4e8f742-7a94-475c-a746-dd69f654d37a)
