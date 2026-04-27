# Huashu Design Studio Web UI

Local web interface for the `huashu-design` skill.

## Run

```bash
cd /Users/judeokun/Documents/GitHub/huashu-design/webui
npm install
npm run dev
```

Open:

```text
http://localhost:5177
```

## Providers

- Ollama: `http://localhost:11434/v1`
- OpenAI-compatible APIs: any `/v1/chat/completions` endpoint
- Anthropic: native `/v1/messages` endpoint

Local Ollama normally does not need a real API key. Some SDKs require a non-empty value, but Ollama ignores it. Hosted Ollama or proxy gateways may require a real key.

## Notes

The UI reads skill context from the parent repo and sends it to the selected model with your brief. Generated HTML appears in the preview iframe and editable code tab.
