# One Pusher Conveyor System

**Simple single-pusher box diverter in CODESYS + Factory I/O**

**Author:** Ebuka Emmanuel Ajaegbu  
**Date:** 30 April 2026  
**Framework:** RAPID Engineer Framework v2.0

### Objective
Basic conveyor with one pneumatic pusher that diverts boxes when detected by a photoelectric sensor, with start debounce, safety stop, and alarm.

### Key Features
- Start button with 5 s TON debounce + 10 s TP alarm (Siren + WarningLight)
- Conveyor runs until box is detected
- Sensor triggers pusher for exactly 700 ms
- PusherBack limit switch ensures safe operation
- Immediate Stop/E-Stop resets everything
- Very short and clean ladder logic

### How It Works
1. Press Start → alarm sounds for 10 s, conveyor starts after 5 s.
2. Box passes Sensor → conveyor stops, pusher activates for 700 ms.
3. Pusher retracts → conveyor resumes.
4. Stop or E-Stop instantly halts everything.

### Technologies
- **PLC:** CODESYS (Ladder Diagram)
- **Simulator:** Factory I/O
- **Approach:** RAPID Engineer Framework v2.0

### RAPID Framework Execution
- Requirements: Clear single-pusher spec
- AI Generation: Initial drafts
- Peer Review: Simplified to minimum working logic
- Iterate & Simulate: Factory I/O tested
- Deploy & Document: Final clean code + this README

### What I Learned
Simple projects teach the most. Debounce timers and limit-switch feedback are essential for reliable pneumatic systems.

**Portfolio Piece** — Clean demonstration of basic conveyor control, safety interlocks, and timer-based actuation.

---

Made with the RAPID Engineer Framework  
Ebuka Emmanuel Ajaegbu — April 2026
