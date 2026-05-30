# Research Notes

## Project

Offline Hindi Voice Assistant for Raspberry Pi

---

## Research Goal

The objective of this research is to identify suitable hardware and software components required to build a privacy-preserving Hindi voice assistant that operates entirely offline on a Raspberry Pi.

---

## Raspberry Pi

### Overview

Raspberry Pi is a low-cost ARM-based single-board computer capable of running Linux operating systems and supporting embedded AI applications.

### Advantages

* Low power consumption
* Supports Python development
* Large developer community
* Suitable for edge AI applications
* Supports USB microphones and speakers

### Selected Board

Raspberry Pi 4 (Recommended)

Reason:
Provides sufficient processing power for offline speech recognition and text-to-speech tasks.

---

## Speech Recognition (ASR)

### What is ASR?

Automatic Speech Recognition (ASR) converts spoken language into text.

Example:

Speech Input:
"समय क्या है"

Output Text:
"समय क्या है"

---

## Vosk ASR

### Overview

Vosk is an open-source offline speech recognition toolkit that supports multiple languages including Hindi.

### Features

* Works completely offline
* Lightweight and efficient
* Supports Raspberry Pi
* Supports Hindi language models
* Low latency

### Reason for Selection

Vosk is suitable for embedded systems because it does not require cloud connectivity and can run efficiently on ARM-based hardware.

---

## Text-to-Speech (TTS)

### What is TTS?

Text-to-Speech converts text into spoken audio.

Example:

Input Text:
"अभी समय 5 बजे है"

Output:
Generated Hindi speech.

---

## Piper TTS

### Overview

Piper is an open-source offline text-to-speech engine optimized for local execution.

### Features

* Offline operation
* Fast inference
* Lightweight
* Good speech quality
* Raspberry Pi compatible

### Reason for Selection

Piper provides high-quality speech synthesis while maintaining low resource usage.

---

## Intent Processing

### Overview

Intent processing determines what action the user wants the assistant to perform.

Example:

User:
"आज तारीख क्या है"

Intent:
Date Query

Action:
Return current date.

---

## Initial Supported Intents

### Time Query

Example:
"समय क्या है"

Response:
Current system time.

---

### Date Query

Example:
"आज तारीख क्या है"

Response:
Current system date.

---

### Greeting

Example:
"नमस्ते"

Response:
Greeting message.

---

### Calculator Operations

Example:
"दो और तीन जोड़ो"

Response:
5

---

## Privacy Considerations

### Traditional Cloud-Based Systems

Voice Data
→ Internet
→ Cloud Server
→ Processing
→ Response

Potential concerns:

* Internet dependency
* User data leaves device

---

### Proposed System

Voice Data
→ Raspberry Pi
→ Local Processing
→ Response

Benefits:

* Offline operation
* Enhanced privacy
* Reduced latency

---

## Future Research Areas

### Wake Word Detection

Possible Tools:

* OpenWakeWord
* Porcupine

Example Wake Word:
"नमस्ते सहायक"

---

### Noise Reduction

Possible Tools:

* RNNoise

Purpose:
Improve speech recognition accuracy in noisy environments.

---

### Local LLM Integration

Potential Models:

* Phi
* Gemma
* Tiny language models

Purpose:
Enable more natural conversations while remaining offline.

---

## Current Research Status

Research Phase: Ongoing

Completed:

* Raspberry Pi evaluation
* Vosk ASR study
* Piper TTS study

Pending:

* Wake word evaluation
* Performance benchmarking
* Hardware testing

---

## Notes

This document will be continuously updated as additional research findings and implementation details become available during project development.
