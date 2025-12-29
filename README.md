# 🎵 ShazamClone

A music recognition application that identifies songs from audio samples and provides YouTube links to potential matches.

## 🎯 Overview

ShazamClone is an open-source audio fingerprinting and song recognition system inspired by Shazam. Record or upload an audio snippet, and the application will analyze the audio fingerprint to identify the song and return YouTube links where you can listen to the full track.

## 🏗️ Tech Stack

| Layer | Technology |
|-------|------------|
| **Frontend** | React |
| **Backend** | Rust |
| **Database** | PostgreSQL |
| **Containerization** | Docker |

## ✨ Features

- 🎤 **Audio Recording** - Record audio directly from your browser
- 📁 **File Upload** - Upload audio files for recognition
- 🔊 **Audio Fingerprinting** - Generate unique fingerprints from audio samples
- 🔍 **Song Matching** - Match fingerprints against a database of known songs
- 🎬 **YouTube Integration** - Get YouTube links for identified songs
- ⚡ **Fast Recognition** - Rust-powered backend for high-performance audio processing

## 🚀 Getting Started

### Prerequisites

- [Docker](https://www.docker.com/get-started) & Docker Compose
- [Node.js](https://nodejs.org/) (for local frontend development)
- [Rust](https://www.rust-lang.org/tools/install) (for local backend development)

### Quick Start with Docker

```bash
# Clone the repository
git clone https://github.com/yourusername/ShazamClone.git
cd ShazamClone

# Start all services
docker-compose up -d

# The application will be available at:
# Frontend: http://localhost:3000
# Backend API: http://localhost:8080
```

## 📁 Project Structure

```
ShazamClone/
├── frontend/          # React application
├── backend/           # Rust API server
├── database/          # PostgreSQL migrations and seeds
├── docker-compose.yml # Docker orchestration
└── README.md
```

## 🔧 How It Works

1. **Audio Capture** - The frontend captures audio through the browser's Web Audio API
2. **Fingerprint Generation** - Audio is sent to the Rust backend which generates a unique acoustic fingerprint using spectral analysis
3. **Database Lookup** - The fingerprint is compared against stored fingerprints in PostgreSQL
4. **Match & Return** - Best matches are identified and corresponding YouTube links are returned to the user

## 🛠️ Development

### Frontend (React)

TBA

### Backend (Rust)

TBA

### Database

PostgreSQL runs in Docker. Migrations are applied automatically on startup.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Inspired by [Chigozirim](https://www.youtube.com/watch?v=a0CVCcb0RJM)

---

<p align="center">Made with ❤️ and 🦀</p>
