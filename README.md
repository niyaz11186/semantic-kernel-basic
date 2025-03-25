# Semantic Kernel Text Summarizer

This project demonstrates the use of Microsoft's Semantic Kernel to create an AI-powered text summarization tool. It takes long text input and generates concise summaries using Azure OpenAI services.

## Features

- Text summarization using Azure OpenAI
- Configurable summary length (50-70 words)
- Easy-to-use interface
- Environment-based configuration

## Prerequisites

- Python 3.12 or higher
- Azure OpenAI API access
- Semantic Kernel package (semantic-kernel==1.16.0)
- python-dotenv package

## Setup

1. Clone this repository
2. Install the required packages:
   ```bash
   pip -r install requirements.txt
   ```
3. Create a `.env` file in the project root with the following variables:
   ```
   AZURE_OPENAI_DEPLOYMENT=your_deployment_name
   AZURE_OPENAI_ENDPOINT=your_endpoint
   AZURE_OPENAI_API_KEY=your_api_key
   ```

## Project Structure

- `main.ipynb`: Main Jupyter notebook containing the summarization logic
- `.env`: Configuration file for Azure OpenAI credentials (not included in repository)

## Usage

1. Open the `main.ipynb` notebook
2. Run all cells in sequence
3. The last cell contains an example text that you can modify with your own content
4. The summary will be generated automatically

## Example Output

Input:
```
In a quiet corner of the city, tucked between towering buildings, stood an old bookstore named Timeless Tales...
```

Output:
```
In a quiet city corner stood Timeless Tales, an old bookstore with a wooden sign and a soft jingling bell. Mr. Kapoor, the owner, welcomed visitors warmly while sipping chai. One rainy evening, a young girl named Anaya found refuge there, returning daily until she eventually took over from the aging Mr. Kapoor. Under Anaya, the store remained a haven for lost travelers and curious dreamers.
```

## Configuration

The summarization settings can be modified in the notebook:
- Maximum tokens: Currently set to 500
- Summary length: Configured for 50-70 words
- Service ID: "azure-completion"

## License

This project is open source and available under the MIT License. 