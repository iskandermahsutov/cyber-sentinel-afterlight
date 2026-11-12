# AI Gesture Control – Functional Test Plan

1. Open local HTML in Chrome with internet. Main menu, 16 missions and shop still available.
2. Click **AI ЖЕСТЫ · ВКЛЮЧИТЬ**. Browser must request camera permission only now.
3. Deny camera: show error, keyboard continues working.
4. Allow camera: mirrored preview appears, recognizer loads, recognitions display label and confidence.
5. Open palm move left/right -> BYTE position changes correspondingly. Center -> stops. Without hand -> stops.
6. Closed fist -> shooting while holding, release -> stops.
7. Pointing up -> single jump, without rapid accidental repeat.
8. V sign -> switch BYTE/NOVA, anti-spam cooldown.
9. Thumb up while near terminal -> interacts; when not near -> original interaction rules apply.
10. I-love-you sign -> triggers Q ability with normal cooldown.
11. Open palm (one hand) + fist (second) -> moving while firing.
12. Stop camera -> physical camera indicator turns off, video tracks end; keyboard works.
13. Test mission 4 boss, pause, shop and checkpoint reload with gestures enabled and disabled.
14. Upload to itch.io HTML5 ZIP (HTTPS). Confirm browser permission prompt and actual gesture classification; note embedding restrictions if any.

**Pending:** Tests with a real webcam and the public itch.io deployment cannot be executed in this build environment. Passing simulated JS integration tests is not evidence of live camera recognition.
