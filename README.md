Here’s a concise GitHub README draft for your project:
Hand Gesture Recognition-Based Whiteboard with Handwritten Captioning

This project integrates hand recognition technology to enable gesture-based interaction with a digital whiteboard. Users can draw, erase, and clear content using intuitive hand gestures, with an added feature of converting handwritten text to editable digital captions.
Features

    Gesture-Based Interaction:
        Draw: Index finger open.
        Erase: Index and middle fingers open.
        Clear Canvas: Thumb open.
    Handwritten Text Recognition: Converts handwritten input into digital text using a custom-trained CNN-based OCR model.
    Marker-Free Interaction: No physical tools required.

Methodology

    Hand Gesture Recognition:
        Uses Mediapipe to detect hand landmarks and calculate finger angles to determine gestures.
        Specific gestures trigger drawing, erasing, or clearing the canvas.

    Optical Character Recognition (OCR):
        Custom CNN model trained on 140,000 hand-drawn characters to recognize alphanumerics (0-9, A-Z).
        Architecture:
            4 Convolutional Layers with Pooling.
            2 Dense Layers.
        Achieved 94% training accuracy and 91.5% validation accuracy.

    Processing Pipeline:
        Captures handwritten input from the whiteboard.
        Segments characters and processes them through the OCR model.
        Outputs text in real-time.

Applications

    Presentations
    Classroom Learning
    Collaborative Meetings

Known Limitations

    Performance issues on lower/mid-range systems.
    Inconsistent gesture recognition due to hand tilt.
    OCR challenges in generalizing normal handwriting styles.
    Misclassification in ambiguous inputs.

Future Improvements

    Enhance gesture recognition reliability.
    Improve OCR accuracy for broader handwriting styles.
    Optimize performance for low-spec systems.
