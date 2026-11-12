# CYBER SENTINEL 8.1 – Gesture Integration Test Results

Environment: headless Chromium, local HTML loaded as document content, deterministic synthetic gesture classifier result injection. These are integration tests of **gesture-to-game mechanics**, not evidence that a physical hand was detected by the ML model.

## Passed

- 8.0 cosmetics store accessible.
- Current campaign stage retained.
- Confidence below 0.65 rejected.
- Open-palm x coordinate changes character position.
- Closed fist holds automatic shooting key.
- No tracked hand releases held controls.
- Two consecutive V-sign detections switch BYTE/NOVA.
- Stopping camera releases gesture controls without resetting mission.
- Keyboard movement still works with gesture feature present.
- JavaScript syntax validation passed; no uncaught JS errors in the above scenarios.

## Pending physical-camera verification

- Chrome/Edge webcam permission prompt and real hand classification.
- Correct gesture classification in variable lighting and with different camera mirrors.
- Real model and WASM download from external CDN.
- Camera access on public itch.io embedded HTML5 deployment (HTTPS/camera permission delegation).
- Frame rate and responsiveness on user laptop.

**Result**: Game integrated and smoke-tested; live camera and hosting test must be completed before announcing the AI feature fully verified.
