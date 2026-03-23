#  Drishti-AI Vision Engine
> **Layer:** AI / Computer Vision

This is the core "Retina" of the system. It processes live video feeds to detect human presence and translates spatial coordinates into directional alerts.

## 🧠 Core Functionalities
- **Model:** YOLOv8 (Nano) for < 30ms inference latency.
- **Directional Mapping:** Divides the frame into 3 vertical sectors (Left, Center, Right).
- **Proximity Logic:** Calculates threat urgency based on Bounding Box height-to-frame ratio.
- **Persistence Filter:** Prevents false alarms by requiring 5+ consecutive frames of detection.

## 🛠️ Setup & Installation
1. Navigate to this directory: `cd ai_engine`
2. Create a virtual environment: `python -m venv venv`
3. Activate it:
   - Windows: `.\venv\Scripts\activate`
   - Mac/Linux: `source venv/bin/activate`
4. Install dependencies: `pip install -r requirements.txt`

## 🚦 How to Run
```bash
python src/detector.py