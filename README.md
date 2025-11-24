# Lipi AI

Lipi AI is a mobile application that helps researchers and language communities digitize text from low-resource scripts like Tibetan. It lets users capture text from challenging physical surfaces (stone, wood, paper), extract it using computer vision and OCR, and then send it to an AI translation backend for further processing and analysis.

This repo contains the Flutter application that serves as the front end for the Lipi AI pipeline.

---

## Features

- Capture images of text directly from a mobile device  
- Handle text on irregular and noisy surfaces (stone, wood, paper, etc.)  
- Preprocess captured images to improve readability before OCR  
- Send processed images and text to an AI backend for recognition and translation  
- Simple, clean interface designed for researchers and field work  

---

## Project Overview

Lipi AI was built to reduce the amount of manual transcription required when working with historical or low-resource scripts.

At a high level:

1. The Flutter app lets users capture or upload images of text.  
2. Images go through a computer vision pipeline that denoises, crops, and enhances text regions.  
3. Extracted text is passed to a backend model based on Meta’s No Language Left Behind (NLLB), fine tuned for Tibetan and related scripts.  
4. The result can be used for research, translation, or archiving.

The goal is to make it easier for researchers to work with physical inscriptions and documents without having to manually retype everything.

---

## Tech Stack

**Mobile app**

- Flutter  
- Dart  
- Targets Android, iOS, and Web  

**Backend and AI (separate service)**

- Python  
- PyTorch for model fine tuning and inference  
- OpenCV for image preprocessing and text region extraction  
- NLLB (No Language Left Behind) model adapted for Tibetan script

**Tooling**

- Git and GitHub for version control  
- Flutter tooling for builds and emulator / device testing  

**-----------------------------------------------------------------**
