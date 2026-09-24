# Open AI Path

A free, open-source curriculum from high-school math to reading and reproducing AI research.

12 modules and 77 lessons cover math, Python, classical ML, neural networks from scratch, PyTorch, training, vision, attention, LLMs, reinforcement learning, post-training and alignment, and MLOps. Each lesson has three parts:

- **Understand:** the idea you should come away with.
- **Build:** a small project that proves you understood it.
- **Resources:** free material from the original authors, such as papers, books, and lectures.

Progress and notes are saved in your browser's local storage. Nothing is sent to a server.

## Run it locally

The page loads `path.json` with `fetch`, so it needs a local server. Opening `index.html` directly won't work.

```bash
git clone https://github.com/affan-01/Open-AI-.git
cd Open-AI-
python3 -m http.server
# open http://localhost:8000
```

## Host it on GitHub Pages

1. Go to **Settings → Pages**.
2. Under *Source*, pick **Deploy from a branch**, then choose `main` and `/ (root)`.
3. The site will be live at `https://affan-01.github.io/Open-AI-/`.

## Edit the curriculum

All content lives in `path.json`:

```json
[
  {
    "module": "Module title",
    "short": "Label",
    "intro": "One-sentence description",
    "lessons": [
      {
        "title": "Lesson title",
        "understand": "What you'll understand",
        "build": "What to build",
        "resources": [{ "label": "Link text", "url": "https://..." }]
      }
    ]
  }
]
```

`short` is optional. It sets the label under each node in the progress path.

## How to use it

Do the build task before marking a lesson done. Reading about backprop is not the same as writing it.

## Contributing

Pull requests are welcome. Please keep resources free to access, and link to the original source.

## License

[MIT](LICENSE)
