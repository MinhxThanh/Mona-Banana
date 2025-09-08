<div align="center">
  <img width="128" height="128" alt="Frame 2" src="https://github.com/user-attachments/assets/bf8324dd-871c-4423-8a1b-7fb48b662607" />

# Mona Banana - AI Try-On Chrome Extension
</div>

<div align="center">

https://github.com/user-attachments/assets/cd6a742d-d003-44ad-9c5c-2b52426066a8

</div>

<div align="center">
    <a href="https://chromewebstore.google.com/detail/chat-box-chat-with-all-ai/hhaaoibkigonnoedcocnkehipecgdodm" target="_blank">
       <img src="https://img.shields.io/badge/Chrome%20Web%20Store-Mona%20Banana-red?style=for-the-badge&logo=chromewebstore&logoColor=white" alt="Chrome Web Store" />
    </a>
    <a href="https://github.com/MinhxThanh/Mona-Banana" target="_blank">
       <img src="https://img.shields.io/badge/GitHub-Mona%20Banana-black?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" />
    </a>
    <a href="https://w404.net/">
       <img src="https://img.shields.io/badge/Web-W404.NET-purple?style=for-the-badge&logo=w404&logoColor=white" alt="W404" />
    </a>
</div>

## Overview
Mona Banana is a Chrome extension that brings AI-powered virtual try-on technology to your favorite e-commerce sites like Shopee, Lazada, Amazon, and more. Users can upload their photos and try on clothing items directly from product pages using advanced AI image generation.

## Features
- 🎯 **AI-Powered Try-On**: Generate realistic try-on images using Google's Gemini 2.5 Flash Image Preview model
- 🖱️ **Drag & Drop Interface**: Drag clothing images directly from Shopee product pages
- 📱 **Floating UI**: Draggable, resizable interface that doesn't interfere with browsing
- ⚙️ **Customizable Settings**: Configure API keys and preferences through an intuitive popup
- 💾 **Download & Share**: Save or share your try-on results instantly
- 🔒 **Privacy-First**: All processing happens through secure OpenRouter API

## Installation

### For Users (Recommended)
1. **Install from Chrome Web Store:**
   - **[Install Mona Banana from the official store](https://chromewebstore.google.com/detail/mona-banana/hbhcidbbomecikflbcolacgmfdhidhao)**
2. **Get OpenRouter API Key:**
   - Visit [OpenRouter](https://openrouter.ai/settings/keys) and create a free account to get an API key.
3. **Configure Settings:**
   - Click the Mona Banana extension icon in your browser.
   - Enter your OpenRouter API key and save.


## How to Use

1. **Visit a supported site**: Navigate to any product page on Shopee, Lazada, Amazon, etc.
2. **Upload Your Photo**: Click the floating UI and upload a photo of yourself
3. **Add Clothing**: Either upload a clothing image or drag one from the product page
4. **Generate Try-On**: Click "Generate Try-On" and wait for the AI to create your image
5. **Download/Share**: Save or share your virtual try-on result

## Features in Detail

### Floating UI
- **Draggable**: Move the interface anywhere on the page
- **Minimizable**: Collapse to save screen space
- **Responsive**: Adapts to different screen sizes

### AI Integration
- Uses OpenRouter API with Google Gemini 2.5 Flash Image Preview
- Supports both free and paid tiers
- Optimized prompts for realistic clothing try-on
- High-quality image generation

### Smart Drag & Drop
- Automatically detects Shopee product images
- Seamless integration with website browsing
- No need to save images manually

## Technical Details

### API Integration
The extension uses OpenRouter's API to access Google's Gemini 2.5 Flash Image Preview model for image generation. The API calls include:
- Multimodal input (text + images)
- Optimized prompts for clothing try-on
- Error handling and retry logic

### Permissions
- `storage`: Save user settings.
- `activeTab`: Access the current tab to apply settings changes instantly.
- `scripting`: Inject the floating UI onto supported websites.
- **Host Permissions**: Access `shopee.vn`, `lazada.vn`, `amazon.com`, etc., to enable the try-on feature, and `openrouter.ai` to connect to the AI service.

## Privacy & Security
- No images are stored locally or on servers
- All API communication is encrypted (HTTPS)
- OpenRouter API key is stored securely in Chrome's sync storage
- Images are processed in real-time and not cached

## Troubleshooting

### Common Issues
1. **"API Key Required" Error**
   - Make sure you've entered a valid OpenRouter API key in settings
   - Test the API connection using the "Test API" button

2. **Extension Not Showing**
   - Ensure you're on a supported page (Shopee, Lazada, etc.).
   - Check if "Auto-show floating UI" is enabled in settings
   - Try refreshing the page

3. **Images Not Loading**
   - Check your internet connection
   - Verify the image file format (JPG, PNG, WebP supported)
   - Ensure images are not too large (recommended < 5MB)

4. **Generation Failed**
   - Verify your OpenRouter API key has credits/quota
   - Check if the selected model is available
   - Try with different, clearer images

### Support
For technical support or feature requests, please create an issue in the project repository.

## Development

### Prerequisites
- Chrome browser
- Basic knowledge of JavaScript, HTML, CSS
- OpenRouter API key for testing

## Roadmap
- [ ] Support for more e-commerce sites
- [ ] Batch processing for multiple items
- [ ] Style transfer options
- [ ] Social sharing integration
- [ ] Mobile version (Chrome Mobile Extensions)
