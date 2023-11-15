# screenshot-to-code

This is a simple app that converts a screenshot to HTML/Tailwind CSS. It uses GPT-4 Vision to generate the code, and DALL-E 3 to generate similar looking images.


https://github.com/abi/screenshot-to-code/assets/23818/6cebadae-2fe3-4986-ac6a-8fb9db030045


## Getting Started

The app has a React/Vite frontend and a FastAPI backend. You will need an OpenAI API key with access to the GPT-4 Vision API.

In the root directory,

```bash
cd backend
echo "OPENAI_API_KEY=sk-your-key" > .env
poetry install
poetry run uvicorn main:app --reload --port 7000
cd ..
cd frontend
yarn
yarn dev
```

Open http://localhost:5173 to use the app.

If you prefer to run the backend on a different port, update VITE_WS_BACKEND_URL in `frontend/.env.local`

## Hosted Version

Hosted version coming soon at http://makewithpico.com
