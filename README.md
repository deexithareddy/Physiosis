# Physiosis

Physiosis is an AI-powered physiotherapy rehabilitation assistant that uses a standard webcam and computer vision to analyze exercise movements in real time. It tracks body landmarks, estimates joint movement, detects repetitions and movement limitations, and compares actual performance with exercise-specific reference movements.

The system provides real-time visual feedback, movement quality analysis, corrective guidance, and session-based progress tracking to help users perform rehabilitation exercises more consistently and safely.

## Key Features

- 🎥 Real-time webcam-based pose estimation
- 🦴 Human body landmark tracking using MediaPipe Pose
- 📐 Joint-angle and range-of-motion estimation
- 🔄 Automatic repetition and movement-phase detection
- 🎯 Reference-vs-actual movement comparison
- ⚠️ Detection of limited or incomplete movement
- 📊 Movement quality and session analytics
- 🧑‍⚕️ Exercise-specific corrective guidance
- 📈 Progress tracking across rehabilitation sessions
- 🔒 Local processing approach to reduce unnecessary transmission of raw video

## Technology Stack

- **Frontend:** React, TypeScript, Vite
- **Computer Vision:** MediaPipe Pose
- **Visualization:** Canvas / Real-time Animation
- **Backend:** FastAPI *(planned/scalable architecture)*
- **Database:** MongoDB *(planned/scalable architecture)*

## Core Pipeline

```text
Webcam
   ↓
Pose Estimation
   ↓
Landmark Smoothing
   ↓
Biomechanical Analysis
   ↓
Rep Detection
   ↓
Reference Comparison
   ↓
Feedback
   ↓
Session Analytics
