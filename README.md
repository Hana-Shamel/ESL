# ESL
Egyptian Sign Language gesture detection using mediapipe and openCV
## Arabic Hand Gesture Recognition System
<p align="center">
  <img src="./a34057.gif" width="400" alt="Gesture Recognition Demo">
</p>

### Project Overview

This system extends Kazuhito00's Hand Gesture Recognition by adding support for:

- The complete 28-letter Arabic alphabet

- 3 functional gestures (Space, Delete, Clear)

- Real-time text output with Arabic script rendering

### Key Features
✋ 28 Arabic Letters: Custom-trained gesture models for all Arabic characters

🛠 Utility Gestures:

- 👉 Space: Insert space between words
- ❌ Delete: Remove last character
- 🧹 Clear: Reset entire text

📜 Arabic Text Rendering: Proper RTL display with glyph shaping

⚡ Adjustable Sensitivity: Control detection speed via frame threshold

### Training Protocol

For letter with index 23 in "keypoint_classifier_label.csv":

1. (shift + f) "number +"
2. Add 20 next to "+"  *index 0 to 9: add 0, index 10 to 19: add 10*
3. Run app
4. Press k to enter training mode
5. Press 2 (for 20 + 2 = 22) *Note: CSV uses 0-based indexing while labels start from 1*
6. Make the gesture 20+ times
7. Close app
8. Open "keypoint_classification_EN" in Jupyter notebook & run all cells
9. Training done ✅

Kazuhito00's Hand Gesture Recognition Repo: https://github.com/kinivi/hand-gesture-recognition-mediapipe
