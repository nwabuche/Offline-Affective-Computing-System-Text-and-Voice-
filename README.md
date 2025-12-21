# Offline-Affective-Computing-System-Text-and-Voice-
This project implements an offline affective computing system capable of analyzing both typed text and spoken voice.
this is the link sir to the project python codes i can not upload it to github becaude is too large
https://drive.google.com/file/d/18E5HlhTPL2LJFVxaOJULecw-oRA8i9Pw/view?usp=sharing
Overview
System Requirements

Operating System: Windows 10

Python: Python 3.9 or higher

Environment: Anaconda (recommended)

Hardware: Microphone (built-in or external)

Required Libraries

The following Python libraries are used:

vosk – offline speech recognition

pyaudio – microphone audio capture

numpy – numerical processing and acoustic feature extraction

Project Structure
affective_project/
├─ main.py
├─ app/
│  ├─ text/
│  │  ├─ text_app.py
│  │  └─ typo_simple.py
│  ├─ voice/
│  │  └─ voice_app.py
│  └─ assets/
│     └─ vosk_model/
│        └─ vosk-model-small-en-us-0.15/

Step-by-Step Instructions to Run the Project

Step 1: Open Anaconda Prompt

Open Anaconda Prompt from the Windows Start menu.

Step 2: Navigate to the Project Folder

Example path (adjust if necessary):

cd "C:\Users\david\OneDrive\Dokument\affective_project"

Step 3: Activate Python Environment

If a virtual environment is provided:

conda activate affective_env
If no environment is provided, the base Anaconda environment may be used

Step 4: Verify Vosk Model Location

Ensure the offline speech model exists at:

app/assets/vosk_model/vosk-model-small-en-us-0.15

The folder must contain model files (e.g., am, conf, graph).

Step 5: Run the Application

python main.py


Using the System (Demo Instructions)

After running main.py, the system prompts for a mode:

Press t → Text analysis mode

Press v → Voice analysis mode

Press q → Quit the program



Text Analysis Demo

Select t

Type any sentence (with or without spelling errors)

Example:of typo corrected sentences

i am a studant and i dont like programing
thier adress is wierd and enviroment is noisy
the peoples are angry becuase of the delay

Other Examples:


word examples for the project

Nicole rides her bike in the afternoon

I don't know when I am going to travel unfortunately.

Fortunately, not all the students failed.
 
I am very happy today.

Voice(speech examples)

 i am very happy today.

i am feeling very sad today


this makes me very angry right now


I feel afraid right now

Output includes:

Corrected sentence

Polarity

Subjectivity

Emotion

Sentence type

Voice Emotion Explanation (High Level)

Emotion from voice is inferred using simple, interpretable acoustic features:

Energy (loudness)

Pitch

Speaking rate

Offline Operation Guarantee

No internet connection required
No cloud services
No external APIs
All processing performed locally





