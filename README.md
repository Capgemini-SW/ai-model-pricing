# AI Model Pricing Calculator

A comprehensive web application to compare pricing across major AI providers including AWS Bedrock, Azure OpenAI, Google Cloud Vertex AI, OpenAI, and Anthropic.

## Features

### 🧮 Pricing Calculator
- **Real-time token calculation** from input/output text
- **Provider-specific tokenization** for accurate pricing
- **47+ AI models** across all major providers
- **Interactive filtering** by provider (AWS, Azure, OpenAI, Anthropic, GCP)
- **Professional card design** with scrollable interface
- **Cost comparison** with live pricing updates

### 🚀 AI Services Hub
- **23+ AI services** comprehensively covered
- **Interactive filtering** by service type (Text AI, Image AI, Speech AI)
- **Modern card-based design** with provider badges
- **Direct links** to official documentation

## Live Demo

🌐 **[Visit AI Model Pricing Calculator](https://mohitmehral.github.io/ai-model-pricing/)**

## Tokenization Accuracy

Our calculator uses provider-specific tokenization methods for 85-95% pricing accuracy:

- **OpenAI/Azure**: tiktoken library with GPT-4 encoding (cl100k_base)
- **Anthropic**: ~3.8 chars/token (Claude-optimized approximation)
- **AWS Bedrock**: ~3.6 chars/token (mixed model families)
- **Google Cloud**: ~4.2 chars/token (Gemini/PaLM optimized)

*Different providers tokenize the same text differently, affecting actual costs. Hover over model cards to see provider-specific token counts.*

## Technology Stack

- **Frontend**: HTML5, CSS3, Vanilla JavaScript
- **Design**: Modern responsive design with CSS Grid/Flexbox
- **Deployment**: GitHub Pages
- **CI/CD**: GitHub Actions

## Local Development

1. Clone the repository:
```bash
git clone https://github.com/mohitmehral/ai-model-pricing.git
cd ai-model-pricing
```

2. Open `index.html` in your browser or serve with a local server:
```bash
# Using Python
python -m http.server 8000

# Using Node.js
npx serve .
```

3. Navigate to `http://localhost:8000`

## Project Structure

```
ai-model-pricing/
├── index.html          # Main pricing calculator page
├── services.html       # AI services hub page
├── styles.css          # Main stylesheet
├── services.css        # Services page stylesheet
├── script-new.js       # Pricing calculator logic
├── services.js         # Services page interactions
├── CODEOWNERS          # Code ownership configuration
└── .github/
    └── workflows/
        ├── auto-pr.yml # Auto PR from dev to main
        └── deploy.yml  # GitHub Pages deployment
```

## Contributing

1. Create a feature branch from `dev`:
```bash
git checkout dev
git checkout -b feature/your-feature-name
```

2. Make your changes and commit:
```bash
git add .
git commit -m "Add your feature description"
```

3. Push to `dev` branch:
```bash
git push origin dev
```

4. GitHub Actions will automatically create a PR from `dev` to `main`

## Code Owner

**Mohit Mehral** (@mohitmehral) - Project Owner & Maintainer

## License

MIT License - feel free to use this project for your own purposes.

## Acknowledgments

- Pricing data sourced from official provider documentation
- Modern UI/UX design principles
- Responsive design for all devices

---

**Built with ❤️ by Mohit Mehral**