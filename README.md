# AI Inference Cost Calculator

A comprehensive web application for comparing AI model deployment costs across different providers and infrastructure options. Compare SaaS APIs (OpenAI, Anthropic), managed models (AWS Bedrock), and self-hosted GPU deployments with detailed cost projections and growth modeling.

🔗 **Live Demo**: https://inference-calc.web.app/

## ✨ Features

- **Multi-Provider Comparison**: OpenAI, Anthropic Claude, AWS Bedrock, Azure OpenAI, Google Vertex AI
- **Self-Hosted GPU Analysis**: Complete infrastructure cost breakdown
- **Growth Modeling**: Multi-year projections with customizable growth rates
- **Use Case Scenarios**: Pre-configured templates for different deployment types
- **HIPAA Compliance**: Healthcare-specific filtering and requirements
- **Engineering Overhead**: Realistic cost estimation including operational expenses
- **Shareable Calculations**: URL-based configuration sharing
- **PWA Support**: Installable as a Progressive Web App

## 🚀 Quick Start

### Prerequisites

- Web browser with JavaScript enabled
- (Optional) Node.js 16+ for local development server
- (Optional) Firebase CLI for deployment

### Local Development

#### Option 1: Simple HTTP Server (Recommended)

```bash
# Clone the repository
git clone git@github.com:sudeshmu/inference-calc.git
cd inference-calc

# Serve using Python (built into most systems)
python3 -m http.server 8000

# Or using Node.js
npx http-server . -p 8000

# Or using PHP
php -S localhost:8000
```

Open your browser to `http://localhost:8000`

#### Option 2: Firebase Local Emulator

```bash
# Install Firebase CLI globally
npm install -g firebase-tools

# Login to Firebase (one-time setup)
firebase login

# Start local development server
firebase serve
```

Open your browser to `http://localhost:5000`

### 📁 Project Structure

```
inference-calc/
├── index.html              # Main calculator application
├── comparison.html         # Side-by-side comparison view
├── help.html              # Documentation and help
├── usecase-*.html         # Pre-configured scenario templates
├── firebase.json          # Firebase hosting configuration
├── manifest.json          # PWA configuration
├── robots.txt             # SEO directives
├── sitemap.xml            # Search engine sitemap
├── favicon.svg            # Application icon
├── icon-*.svg             # PWA icons
└── .htaccess              # Apache server configuration
```

## 🎯 Use Cases

The calculator includes pre-configured scenarios for common deployment patterns:

- **Startup/MVP** (`usecase-startup.html`) - Budget-conscious early-stage deployments
- **Enterprise Scale** (`usecase-enterprise.html`) - Large-scale production workloads
- **Healthcare** (`usecase-healthcare.html`) - HIPAA-compliant medical applications
- **Real-time** (`usecase-realtime.html`) - Low-latency interactive applications
- **Batch Processing** (`usecase-batch.html`) - High-throughput batch workflows
- **Cost-Sensitive** (`usecase-cost-sensitive.html`) - Maximum cost optimization

## 🔧 Tech Stack

- **Frontend**: Vanilla HTML5, CSS3, JavaScript (ES6+)
- **Styling**: Tailwind CSS (CDN)
- **Charts**: Chart.js for cost visualization
- **Hosting**: Firebase Hosting
- **PWA**: Service Worker, Web App Manifest
- **SEO**: Structured data, comprehensive meta tags

## 🚢 Deployment

### Firebase Hosting (Production)

```bash
# Install dependencies
npm install -g firebase-tools

# Login to Firebase
firebase login

# Initialize project (one-time setup)
firebase init hosting

# Deploy to production
firebase deploy
```

### Alternative Hosting Options

The application is a static web app and can be deployed to any web server:

- **Netlify**: Drag and drop the project folder
- **Vercel**: `npx vercel --prod`
- **GitHub Pages**: Push to `gh-pages` branch
- **Apache/Nginx**: Copy files to web root directory

## ⚙️ Configuration

### Firebase Setup

1. Create a Firebase project at https://console.firebase.google.com
2. Update `.firebaserc` with your project ID:
   ```json
   {
     "projects": {
       "default": "your-project-id"
     }
   }
   ```

### Custom Domain (Optional)

1. In Firebase Console, go to Hosting
2. Add custom domain
3. Follow DNS configuration instructions

## 🔍 SEO & Analytics

The application includes:

- Comprehensive meta tags for social sharing
- Structured data markup for search engines
- XML sitemap for search indexing
- Optimized for Core Web Vitals
- Mobile-responsive design

## 🛠️ Development

### Adding New Providers

1. Update the provider data in `index.html`
2. Add pricing information in the JavaScript configuration
3. Update comparison logic if needed

### Customizing Scenarios

1. Copy an existing `usecase-*.html` file
2. Modify the pre-filled form values
3. Update the scenario description and title

### Performance Optimization

- All external dependencies are loaded from CDN
- Images are optimized SVG format
- Aggressive caching headers configured
- Minimal JavaScript bundle size

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📞 Support

For questions or support:
- Create an issue on GitHub
- Check the help documentation at `/help.html`
- Review the use case examples

---

**Built with ❤️ for the AI community**