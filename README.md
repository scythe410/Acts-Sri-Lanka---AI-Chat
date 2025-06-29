# Acts of Sri Lanka - Assistant

A serverless AI chat application that answers questions about Sri Lankan legal acts and related documents using Retrieval-Augmented Generation (RAG) with LangChain.js and Azure.

Demo: [live app 😊](https://lively-meadow-0b6650b0f.1.azurestaticapps.net/).

## Features

- **Modern Chat UI** built with Lit and hosted on Azure Static Web Apps
- **Serverless API** using Azure Functions and LangChain.js
- **Document-grounded Q&A** over official Sri Lankan legal PDFs
- **GPT-4o mini** as the backend AI model for intelligent responses
- **Citations** in answers for transparency
- **Personal chat history**
- **Easy deployment** to Azure with `azd deploy`
- **Local development** supported with Ollama

## How it Works

1. **PDFs** in the `data/` folder are ingested, chunked, and embedded for semantic search.
2. **User questions** are matched to relevant document chunks using vector search.
3. **GPT-4o mini** generates intelligent answers grounded in the source documents and includes citations.
4. **All major Sri Lankan acts and amendments** are included as PDFs.

## Deployment

- Deploy to Azure with:
  ```sh
  azd deploy
  ```
- Or just the webapp:
  ```sh
  azd deploy --service webapp
  ```

## Local Development

- Run locally with Ollama or Azure OpenAI.
- See the full documentation for setup instructions.

## Data Sources

- All legal and policy PDFs are in the `data/` folder.

## License

MIT

---

_Built with ❤️ using Azure AI, LangChain.js, and a commitment to legal accessibility_
