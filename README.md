# Hume Anansi

<div align="center">
  <img src="https://storage.googleapis.com/hume-public-logos/hume/hume-banner.png" alt="Hume AI Banner">
  <h3>Empathic Voice Interface with Next.js App Router</h3>
  <p>A modern implementation of Hume's EVI using React SDK and Next.js</p>
</div>

## 🎯 Overview

Hume Anansi is a sample implementation of Hume's [Empathic Voice Interface (EVI)](https://hume.docs.buildwithfern.com/docs/empathic-voice-interface-evi/overview) built with Next.js App Router and Hume's React SDK. This project demonstrates how to integrate emotional AI capabilities into modern web applications.

## ✨ Features

- **Empathic Voice Interface**: Real-time voice interaction with emotional intelligence
- **Next.js App Router**: Modern React framework with server-side rendering
- **Hume React SDK**: Seamless integration with Hume's AI services
- **Responsive Design**: Works across desktop and mobile devices
- **Real-time Processing**: Live voice analysis and response generation

## 🚀 Quick Deploy

Deploy this project instantly with Vercel:

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Fpreetam-90%2Fhume_anansi&env=HUME_API_KEY,HUME_SECRET_KEY)

## 📋 Prerequisites

- Node.js 18+ 
- npm or yarn package manager
- Hume AI account with API access

## 🛠️ Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/preetam-90/hume_anansi.git
   cd hume_anansi
   ```

2. **Install dependencies**
   ```bash
   npm install
   # or
   yarn install
   ```

3. **Set up environment variables**
   
   Create a `.env.local` file in the root directory:
   ```env
   HUME_API_KEY=your_api_key_here
   HUME_SECRET_KEY=your_secret_key_here
   ```

4. **Start the development server**
   ```bash
   npm run dev
   # or
   yarn dev
   ```

5. **Open your browser**
   
   Navigate to [http://localhost:3000](http://localhost:3000)

## 🔑 Getting API Keys

To obtain your Hume API credentials:

1. Visit [Hume AI Portal](https://beta.hume.ai/)
2. Create an account or log in
3. Navigate to [API Keys page](https://beta.hume.ai/settings/keys)
4. Generate your API Key and Secret Key
5. Copy the keys to your `.env.local` file

## 📁 Project Structure

```
hume_anansi/
├── app/                    # Next.js App Router pages
├── components/             # Reusable React components
├── lib/                    # Utility functions and configurations
├── public/                 # Static assets
├── styles/                 # CSS and styling files
├── .env.local.example      # Environment variables template
└── README.md              # Project documentation
```

## 🔧 Configuration

### Environment Variables

| Variable | Description | Required |
|----------|-------------|----------|
| `HUME_API_KEY` | Your Hume API key | ✅ |
| `HUME_SECRET_KEY` | Your Hume secret key | ✅ |

### Customization Options

- Modify voice settings in `lib/hume-config.js`
- Customize UI components in `components/`
- Adjust styling in `styles/` directory

## 🎨 Usage Examples

### Basic Voice Interaction
```javascript
import { useVoice } from '@humeai/voice-react';

function VoiceComponent() {
  const { connect, disconnect, status } = useVoice();
  
  return (
    <button onClick={status === 'connected' ? disconnect : connect}>
      {status === 'connected' ? 'Disconnect' : 'Connect'}
    </button>
  );
}
```

## 🚢 Deployment

### Vercel (Recommended)

1. Fork this repository to your GitHub account
2. Connect your Vercel account to GitHub
3. Import the project in Vercel
4. Add environment variables in Vercel dashboard
5. Deploy!

### Other Platforms

This Next.js application can be deployed on various platforms:
- **Netlify**: Use the Next.js build adapter
- **Railway**: Direct deployment from GitHub
- **AWS/GCP/Azure**: Use containerized deployment

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🆘 Support

- **Documentation**: [Hume AI Docs](https://hume.docs.buildwithfern.com/)
- **Discord Community**: [Join our Discord](https://link.hume.ai/discord)
- **Issues**: [GitHub Issues](https://github.com/preetam-90/hume_anansi/issues)
- **Email**: support@hume.ai

## 🙏 Acknowledgments

- [Hume AI](https://hume.ai/) for the amazing EVI technology
- [Next.js](https://nextjs.org/) team for the excellent framework
- [Vercel](https://vercel.com/) for seamless deployment platform

---

<div align="center">
  <p>Built with ❤️ using <a href="https://hume.ai/">Hume AI</a> and <a href="https://nextjs.org/">Next.js</a></p>
</div>
