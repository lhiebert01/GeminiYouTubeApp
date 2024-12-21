# Gemini Flash YouTube Video Insights Pro

🎥 ⚡ 🤖 A powerful YouTube video analysis tool that leverages Google's Gemini AI to provide comprehensive insights, summaries, and interactive Q&A for any YouTube video with available transcripts.

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://geminiyoutubeapp.streamlit.app)

## Features

- **Comprehensive Video Analysis**: Generate detailed summaries, key points, and insights from YouTube videos
- **Multiple Analysis Types**:
  - Summary & Key Points
  - Title Suggestions
  - Quotes with Timestamps
  - Key Terms & Definitions
  - Full Analysis (all of the above)
- **Interactive Q&A**: Ask questions about the video content and get AI-powered responses
- **Export Options**: Download analysis results in both Word and Text formats
- **Full Transcript Access**: View and download complete video transcripts
- **Large Context Window**: Utilizes Gemini's 1M token input capacity for comprehensive analysis

## Installation

1. Clone the repository:
```bash
git clone https://github.com/lhiebert01/GeminiYouTubeApp.git
cd GeminiYouTubeApp
```

2. Create and activate a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

## Configuration

1. Create a `.env` file in the project root with your API keys:
```env
GEMINI_API_KEY=your_gemini_api_key
YOUTUBE_API_KEY=your_youtube_api_key
```

2. For Streamlit deployment, configure secrets in your Streamlit dashboard:
   - Navigate to your app settings
   - Add the above environment variables in the Secrets management section

## API Keys Setup

1. **Gemini API Key**:
   - Visit [Google AI Studio](https://makersuite.google.com/app/apikey)
   - Create a new API key
   - Copy the key to your `.env` file or Streamlit secrets

2. **YouTube API Key**:
   - Go to [Google Cloud Console](https://console.cloud.google.com/)
   - Create a new project or select an existing one
   - Enable the YouTube Data API v3
   - Create credentials (API key)
   - Copy the key to your `.env` file or Streamlit secrets

## Usage

1. Run the application locally:
```bash
streamlit run app.py
```

2. Enter a YouTube URL in the sidebar
3. Select your desired analysis type
4. Click "Run Analysis" to generate insights
5. Use the Q&A interface to ask specific questions about the video
6. Download results in your preferred format

## Features in Detail

### Analysis Types

1. **Summary & Key Points**
   - Comprehensive summary (2-3 paragraphs)
   - Key points in table format

2. **Title Suggestions**
   - 3-5 alternative titles with explanations
   - Based on video content and themes

3. **Quotes with Timestamps**
   - 5-10 significant quotes
   - Context and significance explanations

4. **Key Terms & Definitions**
   - Important concepts and jargon
   - Clear, organized definitions

5. **All Analysis**
   - Complete analysis including all above features

### Export Options

- **Word Document**: Complete analysis with formatting
- **Text File**: Plain text version of analysis
- **Transcript**: Raw video transcript

## Development

- Built with Streamlit and Google's Gemini AI
- Uses YouTube Data API v3 for video information
- Implements smart text truncation for long videos
- Maintains session state for seamless user experience

## Deployment

The application is deployed on Streamlit Cloud. For deployment:

1. Push your changes to GitHub
2. Connect your repository to Streamlit Cloud
3. Configure your environment variables in Streamlit Cloud
4. Deploy!

## Security Notes

- Never commit `.env` file or secrets to the repository
- Use environment variables for all sensitive information
- Implement rate limiting and error handling for API calls

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.


## Documentation

- [Architecture Overview](docs/ARCHITECTURE.md) - Detailed application structure and flow
- [Technical Details](docs/TECHNICAL.md) - In-depth technical implementation details

For a complete understanding of the application architecture and flow, please see the [Architecture Documentation](docs/ARCHITECTURE.md).

## Credits

Developed by [Lindsay Hiebert](https://www.linkedin.com/in/lindsayhiebert/) using Google's Gemini AI and Streamlit.

## Contact

For questions or collaboration, please reach out through [LinkedIn](https://www.linkedin.com/in/lindsayhiebert/).