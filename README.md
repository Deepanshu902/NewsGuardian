# NewsGuardian – AI Credibility Analyzer

<p align="center">
  <img width="450" src="./images/news.png" alt="NewsGuardian">
</p>

A Chrome extension that provides real-time credibility analysis of any selected text using Large Language Models. Highlight text on any webpage, click the icon, and get an instant breakdown with a credibility score and reasoning.

During evaluation, flagged ~30% of sampled news content as potentially unreliable or biased.

---

## Tech Stack

- **Frontend:** HTML, CSS, JavaScript  
- **Browser API:** Chrome Extension Manifest V3 (Service Worker)  
- **AI Integration:** OpenRouter API  
- **Core Logic:** Async Fetch API, structured prompt engineering for reliable JSON outputs

---

## Getting Started

### Prerequisites
- Google Chrome  
- An API key from [OpenRouter.ai](https://openrouter.ai/)

### Installation

1. Clone the repo
```sh
   git clone https://github.com/Deepanshu902/NewsGuardian.git
   cd NewsGuardian
```

2. Set up your API key  
   Copy `background.example.js` → rename to `background.js`  
   Replace the placeholder with your OpenRouter key:
```javascript
   const OPENROUTER_API_KEY = "YOUR_API_KEY_HERE";
```

3. Load in Chrome  
   - Go to `chrome://extensions`  
   - Enable **Developer mode**  
   - Click **Load unpacked** → select the project folder

---

## Usage

1. Go to any news article or webpage  
2. Highlight the text you want to check  
3. Click the NewsGuardian icon in your toolbar  
4. Hit **"Analyze Selected Text"**  
5. View the credibility score and reasoning in the popup

---

## License

MIT License — see `LICENSE` for details.