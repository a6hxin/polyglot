# 🌐 Polyglot Developer Hub

A multi-language code editor and analyzer built with vanilla JavaScript, Monaco Editor, HTML, and CSS — with a FastAPI Python backend and Next.js dashboard.

## What it does

Polyglot Developer Hub lets developers write, analyze, and get feedback on code across multiple programming languages — all in one place. It uses the Monaco Editor (the same engine powering VS Code) for a professional in-browser coding experience.

## Features

🖊️ Monaco Editor** — full VS Code-like editing experience in the browser
🔍 Code Analyzer** — analyze your code and get instant feedback
📊 Dashboard** — view your analysis history and insights
🌍 Multi-language support** — TypeScript, Python, JavaScript, and more
⚡ Fast API backend** — Python/FastAPI powers the analysis engine
🎨 Clean UI** — responsive design with custom CSS

### Prerequisites
- Node.js 18+
- Python 3.11+

### Installation

**1. Clone the repo**
```bash
git clone https://github.com/a6hxin/polyglot.git
cd polyglot
```

**2. Setup backend**
```bash
cd backend
pip3 install -r requirements.txt
cp .env.example .env
# Add your GROQ_API_KEY to .env
python3 -m uvicorn app.main:app --reload --port 8000
```

**3. Setup frontend**
```bash
cd frontend
npm install
cp .env.local.example .env.local
# Add your GROQ_API_KEY to .env.local
npm run dev
```

***4. Open the editor**

Just open `index.html` directly in your browser — or visit `http://localhost:3000` for the full dashboard.

## Environment Variables

```
GROQ_API_KEY=your-groq-api-key-here
NEXT_PUBLIC_API_URL=http://localhost:8000
```

Get a free Groq API key at [console.groq.com](https://console.groq.com)

## Contributing

Pull requests are welcome! Feel free to open an issue for bugs or feature requests.

## License

MIT
