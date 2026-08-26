# New Business Concept Planner

This project helps someone plan a new local business idea before launch. It works well for:

- restaurants
- clinics
- gyms

The notebook generates a practical concept summary that includes:

- business overview
- services
- target audience
- strengths
- marketing suggestions
- early website and brand direction

## Recent updates

The project has recently evolved from a simple notebook example into a more interactive AI assistant experience:

- Moved from a blocking JSON-only response to a streaming markdown output.
- Added a Gradio chat-style interface so the user can answer questions conversationally.
- The app now asks for the business details in a chat flow and returns the business plan directly inside the interface.
- The bot is designed for local business concept generation, launch planning, and early brand direction.

## Files

- `insight.ipynb` – main notebook and app for planning a new local business concept
- `README.md` – project overview and recent changes

## Requirements

Before running the notebook, make sure you have:

- Python installed
- a `.env` file in the project folder
- an OpenAI API key in the `.env` file as:

```env
OPENAI_API_KEY=your_key_heres
```

You may also need these Python packages installed:

```bash
pip install python-dotenv openai ipython gradio
```

## How to use

1. Open `insight.ipynb` in VS Code.
2. Run the setup/import cell.
3. Launch the Gradio chat app with:

```python
demo = launch_gradio_app()
demo.launch()
```

4. Enter the details in the chat interface:
   - business name
   - business type
   - location
   - target audience
   - brand idea
5. The assistant will generate a local business launch plan in the chat output.

## Example chat flow

The app asks questions in this style:

- Business name: FitNest
- Business type: gym
- Location: Gurgaon, Haryana
- Target audience: beginners and active adults
- Brand idea: community-first coaching with accountability

The response is generated directly in the chat interface as a streamed output.

## Notes

- The notebook is designed for a new business concept, not an existing company.
- It does not need an existing website or live URL to be useful.
- You can later extend it with pricing, competitor analysis, location strategy, and homepage sections.
- The project has been updated recently to better support interactive, user-friendly launch planning.
