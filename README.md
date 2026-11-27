# Obikol-Plagiarism-checker

https://astounding-panda-69c019.netlify.app/

Obikol Plagiarism Checker (অবিকল প্লেজিয়ারিজম চেকার)

Obikol Plagiarism Checker is a 100% offline-first text, audio, and video plagiarism & AI forensics suite built in a single self-contained HTML application (obikol-plagiarism-checker.html). It analyzes Bengali and English text against pre-indexed and user-uploaded .zip archives, detects AI writing patterns and model signatures, inspects audio/video media locally in the browser, suggests human-sounding alternatives, reads guidance aloud with live transcripts, and triggers automated SMS report workflows via Zapier.

Key Features

1. 100% Offline Archive Indexing & Custom .zip Upload

Pre-loaded Reference Archives: Comes pre-configured with six bundled web archive datasets:

saveweb2zip-com-read-amazon-com.zip (Amazon Kindle Cloud Reader reading & note corpus)

saveweb2zip-com-www-turnitin-com.zip (Academic & research integrity corpus)

saveweb2zip-com-quillbot-com.zip (Paraphrasing & synonym replacement corpus)

saveweb2zip-com-www-grammarly-com.zip (AI detection, tone & proofreading corpus)

saveweb2zip-com-turboscribe-ai.zip (Audio transcription & speech corpus)

saveweb2zip-com-zapier-com.zip (Workflow automation & mobile SMS trigger corpus)

Local Archive Ingestion: Upload additional .zip, .txt, .html, or .json files in the জিপ ফাইল (ZIP Archives) tab to extract sentences locally without network calls.

2. Plagiarism & AI Stylometry Forensics

Sentence-Level & Phrase-Level Matching: Combines normalized token overlap (Jaccard similarity) and 3-word phrase matching against indexed archive sentences to flag copied passages and display the matching archive source.

AI Pattern & Model Attribution: Evaluates Bengali and English lexical cues, grammatical templates, sentence structure uniformity (burstiness), and lexical diversity to estimate AI likelihood and surface matching model signatures (such as OpenAI ChatGPT / GPT-4o, Google Gemini, Anthropic Claude, and DeepSeek / Llama).

Color-Coded Highlight View & Humanizer Alternatives: Highlights sentences as copied, AI-patterned, or human-authored, generates human-sounding rewrites, and lets users replace individual sentences or apply all rewrites in one click.

3. Pro Offline Audio & Video AI Forensics Studio

Audio Signal Analysis: Decodes uploaded or drag-and-dropped audio files (MP3, WAV, OGG, M4A, etc.) using Web Audio API (AudioContext) to render a dual-layer peak/RMS waveform canvas and inspect digital zero-noise floor, active loudness variation, prosody/pitch consistency, crest factor, silence ratio, and channel/sample-rate characteristics.

5-Frame Video Forensics: Extracts five timestamped frame thumbnails from uploaded or dropped videos (MP4, WEBM, MOV, etc.) and evaluates center-vs-border texture detail and inter-frame pixel changes.

4. Zapier Workflow & Mobile SMS Alert Simulation (Not available now)

3-Step Automation Pipeline (Trigger → Formatter → SMS by Zapier): Automatically formats scan scores, detected archives, and top rewrite suggestions upon scan completion (or on manual trigger).

Mobile Inbox Preview & Native SMS Link: Displays the formatted SMS inside an on-screen mobile inbox mockup, logs automation runs, and prepares an sms: launch link for opening the device's messaging app.

Project Structure

obikol-plagiarism-checker/
├── obikol-plagiarism-checker.html   # Self-contained offline application (UI, styles, and JS engine)
└── README.md                        # Repository documentation


Getting Started (Offline Usage)

Download or clone this repository containing obikol-plagiarism-checker.html.

Open obikol-plagiarism-checker.html directly in a modern web browser (Chrome, Edge, Firefox, or Safari).

Paste text, load a sample preset, dictate with your microphone, or open 🎬 অডিও / ভিডিও AI চেক to inspect an audio or video file.

Review results across the বিশ্লেষণ (Analysis), বিকল্প (Alternatives), জ্যাপিয়ার SMS (Zapier SMS) (N/A), and জিপ ফাইল (ZIP Files) tabs.

Technical Notes & Limitations

Client-Side Heuristics: All text similarity scoring, stylometric AI indicators, and audio/video checks run locally in the browser using client-side heuristics and signal metrics—not external cloud plagiarism databases or commercial AI detectors.

Browser API Support: Voice recognition (SpeechRecognition), speech synthesis (speechSynthesis), and local audio decoding (AudioContext) depend on browser support and microphone/media permissions.

SMS Delivery: The built-in Zapier tab simulates the 3-step workflow, updates the mobile inbox preview, maintains run logs, and builds an sms: URI; sending a real carrier SMS requires an active mobile messaging app or a live external Zapier webhook/SMS integration. This is not available now.

MIT License

Copyright (c) 2026 Obikol Plagiarism Checker Contributors

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
