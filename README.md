# Call_Quality_Analyzer

# Call Quality Analyzer - Internship Assignment

## About The Project
This project analyzes a sales call recording to assess call quality by extracting key metrics such as talk-time ratio, number of questions asked, longest monologue duration, and overall call sentiment. It uses energy-based voice activity detection for speech segmentation, Google Speech Recognition for transcription, and VADER for sentiment analysis. The system is optimized to run within 30 seconds on the free tier of Google Colab.

## Features
- Processes audio from YouTube sales call recording
- Detects speech segments through energy-based voice activity detection
- Transcribes segments to text and counts questions asked
- Calculates talk-time ratio and longest uninterrupted monologue duration
- Analyzes sentiment of the entire call (positive, neutral, or negative)
- Generates actionable insights to improve call engagement

## Tech Stack
- Python 3.x
- Google Colab (Cloud Execution)
- Libraries: librosa, pydub, speechrecognition, vaderSentiment, numpy

## Getting Started

### Prerequisites
- Access to Google Colab
- Hugging Face token (only if using advanced diarization, optional here)

### How to Run
1. Open the notebook in Google Colab.
2. Run all cells sequentially—each cell contains comments explaining the approach.
3. The notebook downloads the audio, processes speech segments, transcribes, and performs analysis.
4. View final metrics and actionable insights printed at the end.

## Approach Summary
The audio is segmented using simple energy thresholds to detect voice activity robustly in poor-quality audio. Segments are merged to form longer chunks that improve transcription accuracy through Google’s speech recognition API. Transcriptions provide counts of questions asked, while durations yield talk-time ratios and longest monologue times. Sentiment analysis via VADER gives overall call tone. Actionable insights help the sales team improve conversation balance and engagement.

## Bonus
Identifying sales rep vs customer was approached by heuristics on talk duration and speech patterns (not fully implemented).

---

Feel free to clone or download the notebook from GitHub for details.

## License
This project is for educational purposes and internship submission only.
