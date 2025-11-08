  GestureSpeak

Speak with a wave. A touchless, AI-powered communication board that runs entirely in your browser, built to showcase the power of on-device AI for accessibility.

  About The Project

GestureSpeak is an accessible communication tool built for the  Arm AI Developer Challenge 2025 . It uses a standard webcam to recognize simple hand gestures, allowing users to navigate a customizable list of phrases and have them spoken aloud.

The core of this project is  on-device AI . Every calculation, from hand tracking to gesture recognition, happens 100% locally in your browser. This means:

  Privacy First:  No camera data ever leaves your computer.
  Zero Latency:  It's fast and responsive, with no need for an internet connection.
  Accessible:  It can run on low-power devices, including Arm-based hardware like a Raspberry Pi or a mobile phone.

  Key Features

   Real-Time Gesture Control:  Navigate a list of phrases using simple, reliable hand gestures.
    Customizable Phrase Board:  A "Settings" mode allows you to add your own custom phrases (e.g., "I'm hungry," "What's your name?") which are saved to your browser's local storage.
    Text-to-Speech:  Selected phrases are spoken aloud using the browser's native speech engine.
    100% On-Device AI:  Uses  MediaPipe  and  TensorFlow.js Lite  to run the gesture recognition model entirely in the browser. No cloud, no lag, no privacy concerns.
    Responsive UI:  The modal features a clear sidebar layout, allowing users to see their hand and the phrase list simultaneously.

  How to Use

Once the "Try Live Demo" modal is open, your camera will activate. The app uses a "cooldown" system, so you only need to hold a gesture for about 0.7 seconds for it to register.

   Point Up:  Move to the  Next  phrase in the list.
   Victory (Peace):  Move to the  Previous  phrase.
   Thumb Up:   Speak  the currently selected phrase.
   Open Palm:   Reset  the selection to the first phrase ("Hello").
   Settings Icon:  Pauses the camera and lets you  add or delete  custom phrases.

  Tech Stack

   Frontend:  React, TypeScript
    AI / Machine Learning: 
    MediaPipe  (for the `GestureRecognizer` task)
    TensorFlow.js  (as the web backend for MediaPipe)
    Styling:  Inline CSS-in-JS (React styles)
    Icons:  `lucide-react`
    Build Tool:  Vite

  Getting Started: Running Locally

To get a local copy up and running, follow these simple steps.

   Prerequisites

  Node.js (v18 or higher)
  `npm` or `yarn`

   Installation

1.   Clone the repo: 
     sh
    git clone https://github.com/your-username/gesturespeak.git
     
2.   Navigate to the project directory: 
     sh
    cd gesturespeak
     
3.   Install NPM packages: 
     sh
    npm install
     
4.   Get the AI Model: 
        You need the MediaPipe Gesture Recognizer model.
         Download the file here:  [gesture\_recognizer.task](https://www.google.com/search?q=https://storage.googleapis.com/mediapipe-models/gesture_recognizer/gesture_recognizer/float16/1/gesture_recognizer.task)
        Place the downloaded `gesture_recognizer.task` file inside the  /public  folder in your project.
5.   Run the development server: 
     sh
    npm run dev
     
   Your site will be running on `http://localhost:5173`.

  Author

Built with passion for the Arm AI Developer Challenge 2025.

   Nithyashree CS 


