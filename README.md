# EyeBlinkControllingCursor

**EyeBlinkControllingCursoror** is a Python-based project that allows users to control the computer cursor through eye blinks detected via a webcam. This tool is intended to improve accessibility by enabling hands-free computer interaction for users with limited mobility.

## Features

- Detects eye blinks using computer vision techniques
- Moves and controls the cursor based on blink patterns
- Can be used as an assistive technology solution

## How It Works

1. The system uses a webcam to capture real-time video of the user’s face.
2. Computer vision algorithms process the video feed to detect eye blinks.
3. When a blink (or a specific sequence of blinks) is detected, the program translates it into cursor movement or clicks.

## Example Pseudocode

```python
import cv2

# Initialize webcam
cap = cv2.VideoCapture(0)

while True:
    ret, frame = cap.read()
    # Detect eyes and check for blinks (using a pre-trained model)
    # If blink detected:
    #     Move cursor or perform a click
    if cv2.waitKey(1) & 0xFF == ord('q'):
        break

cap.release()
cv2.destroyAllWindows()
```

## Getting Started

1. Install dependencies (e.g., OpenCV, dlib, pyautogui).
2. Run the main Python script.
3. Allow webcam access.
4. Follow instructions to calibrate blink detection.

## Use Cases

- Hands-free computer control for users with physical disabilities
- Alternative input method for general users

## Contributing

Contributions are welcome! Please open issues or pull requests for improvements.

---

