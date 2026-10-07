# Pro Metronome

A professional-grade, browser-based metronome built with Vanilla JavaScript and the Web Audio API. 

Unlike basic JavaScript metronomes that rely on `setInterval` (which is prone to drifting and lag due to the single-threaded nature of JS), this project uses a **Lookahead Scheduling** architecture. By leveraging the Web Audio API's hardware clock, it ensures sample-accurate, drift-free timing essential for serious musical practice.

## ✨ Features

* **Precision Timing:** Utilizes Web Audio API and lookahead scheduling (`setTimeout` + `audioContext.currentTime`) for zero-latency, rock-solid rhythm.
* **Custom Time Signatures:** Includes standard presets (2/4, 3/4, 4/4, 6/8, etc.) and a modal interface to create any custom time signature up to 32 beats per measure.
* **High Pitch Mode:** A toggleable EQ setting that doubles the oscillator frequencies (from 800Hz/1200Hz to 1600Hz/2400Hz) to cut through heavy mixes or loud instruments.
* **Dynamic Visualizer:** Real-time visual feedback using an internal queue system (`requestAnimationFrame`) synced perfectly with the audio context.
* **Keyboard-Friendly BPM Input:** Adjust the tempo using the slider, the +/- buttons, or by directly typing the desired BPM. 

## 🛠️ Technologies Used

* **HTML5**
* **Tailwind CSS** (via CDN for UI styling)
* **Vanilla JavaScript** (ES6+)
* **Web Audio API** (Oscillators and Gain Nodes)
* **Google Material Symbols**
