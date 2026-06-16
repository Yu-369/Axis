###  Axis

*A web-based Computer Vision interface that detects bad posture and recognises once the user leaves the frame*



**Main Architecture & Features:**

* **The Slouch Cop (Scale Invariance Mathematics):** This engine instead computes the 2D vertical drop of the user's head relative to the 3D shoulder width instead of an incorrect 3D Z-axis distance. This hybrid math makes the posture detection scale invariant (it works flawlessly at any distance of the user from the camera).

* **Auto-Lock Sequence:** Presence detection timer, asynchronous. If the MediaPipe `onResults` callback returns `null` for 5 seconds straight, the system goes into lockdown. (To be connected via `fetch()` to a local node.js `child_process` to trigger a native Windows `Win+L` lock when the user walks away from their desk).

**Observation:**
I am a prompt-native systems architect. I developed the hybrid 2D/3D spatial logic, scale-invariant mathematics, and event-trigger constraints. I accelerated the raw Vanilla JS and MediaPipe CDN integration using AI (Gemini 3.1 Pro) following my strict architectural prompts.
