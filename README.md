# Wikipedia Article Generator

![Python](https://img.shields.io/badge/Python-3.7%2B-blue)
![License](https://img.shields.io/badge/License-MIT-green)

A powerful tool that combines Weaviate, Cloudflare AI, and OpenAI to generate Wikipedia-style articles on any topic.

## Features

- Semantic search using Weaviate for context retrieval
- Article generation with Cloudflare AI's Llama model
- Enhanced content quality via OpenAI's language models
- Customizable article structure
- Scalable and efficient content generation pipeline

## Technologies

- [Weaviate](https://weaviate.io/): Vector database for semantic search
- [Cloudflare AI](https://www.cloudflare.com/products/workers-ai/): Text generation (Llama 3.1 model)
- [OpenAI](https://openai.com/): Additional language processing
- [Python](https://www.python.org/): Core programming language

## Prerequisites

- Python 3.7+
- Weaviate account and API key
- Cloudflare account and API key
- OpenAI API key

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/joiscode121/Wikipedia_article_generator.git
   cd Wikipedia_article_generator
   ```

2. Install required packages:

   ```bash
   pip install -r requirements.txt
   ```

3. Set up environment variables:
   Create a `.env` file in the project root:
   ```env
   WCD_DEMO_URL=YOUR_WEAVIATE_URL
   WCD_DEMO_RO_KEY=YOUR_WEAVIATE_API_KEY
   OPENAI_APIKEY=YOUR_OPENAI_API_KEY
   CLOUDFLARE_AUTH_TOKEN=YOUR_CLOUDFLARE_AUTH_TOKEN
   CLOUDFLARE_ACCOUNT_ID=YOUR_CLOUDFLARE_ACCOUNT_ID
   ```

## Usage

1. Open `wikipedia_article_generator.ipynb` in Jupyter Lab or Notebook.

2. Run the cells to set up the environment and define functions.

3. Generate an article:

   ```python
   topic = "Artificial Intelligence"
   article = create_wikipedia_article(topic)
   print(article)
   ```

4. The generated article will include these sections:
   - Introduction
   - History
   - Types
   - Applications
   - Current State of Research
   - Benefits and Limitations
   - Ethical Considerations
   - Future Prospects

## Customization

Modify the `prompt` variable in the `generate_content` function to customize the article structure or add specific instructions.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Weaviate for providing powerful vector search capabilities
- Cloudflare for their AI text generation services
- OpenAI for their language models and API

## Disclaimer

This tool is for educational and research purposes. Always verify the generated content for accuracy and comply with relevant terms of service when using third-party APIs.
