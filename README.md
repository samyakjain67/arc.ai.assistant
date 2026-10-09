# Arc — Personal AI Assistant (Vercel)

## Deploy
1. Upload all files in this folder to the root of your GitHub repository (including `index.html`, `api/`, `package.json`, and `vercel.json`).
2. Import that repository into Vercel and deploy it.
3. In Vercel Project Settings → Environment Variables, add:
   - Key: `OPENAI_API_KEY`
   - Value: your OpenAI API key (keep it private)
   - Environment: Production (and Preview if needed)
4. Save, then redeploy the project.
5. Open the website and send a test message.

The `index.html` file is at the repository root so the homepage is served directly. The `/api/chat` endpoint is a Vercel serverless function in `api/chat.js`.

## Important
- Never put your API key in `index.html` or any public file.
- ChatGPT subscriptions and OpenAI API billing are separate. The API account must have access/credit for responses.
- The default model is `gpt-4.1`; you can optionally set `OPENAI_MODEL` in Vercel to a model enabled for your API account.
