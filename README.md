# Construction Law Agent

A browser-based **AI legal assistant** that answers questions about the Building Standards Act. Type a natural-language question; get a structured, cited answer rendered as formatted Markdown.

**[▶ Live Demo](https://woodyhoko.github.io/construction_law_agent)**

---

## What It Does

The agent parses a local copy of the **Building Standards Act** (`building standards act.txt`) and answers user queries against that corpus. Responses are formatted in Markdown and rendered inline via the `marked.js` library.

Use cases:
- "What permits are required for structural modifications?"
- "What are the fire safety requirements for commercial buildings?"
- "Summarize the inspection obligations under Section 12."

---

## Stack

| Layer | Technology |
|---|---|
| Layout & Styling | Tailwind CSS |
| Markdown Rendering | [marked.js](https://marked.js.org/) |
| Typography | Merriweather (headings) + Open Sans (body) |
| Build | None — single HTML file + text corpus |

---

## Run Locally

```bash
# Serve locally (required — fetch() needs a server context)
python -m http.server 8000
# then open http://localhost:8000
```

---

## Files

| File | Description |
|---|---|
| `index.html` | App shell + UI + agent logic |
| `building standards act.txt` | Legal corpus used as the knowledge base |
