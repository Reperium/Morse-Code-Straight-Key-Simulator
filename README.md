Open the static websites at these links:

Version 0.1: https://github.com/Reperium/Morse-Code-Straight-Key-Simulator/blob/main/Previous%20Versions/Version%200.1.html

Version 1.0: https://github.com/Reperium/Morse-Code-Straight-Key-Simulator/blob/main/Previous%20Versions/Version%201.0.html

Version 1.1: https://github.com/Reperium/Morse-Code-Straight-Key-Simulator/blob/main/Previous%20Versions/Version%201.1.html

Version 1.2: https://github.com/Reperium/Morse-Code-Straight-Key-Simulator/blob/main/Previous%20Versions/Version%201.2.html

Version 1.3: https://github.com/Reperium/Morse-Code-Straight-Key-Simulator/blob/main/Previous%20Versions/Version%201.3.html

Version 1.4: https://github.com/Reperium/Morse-Code-Straight-Key-Simulator/blob/main/Previous%20Versions/Version%201.4.html

Version 1.5: https://github.com/Reperium/Morse-Code-Straight-Key-Simulator/blob/main/Previous%20Versions/Version%201.5.html

Version 1.6: https://github.com/Reperium/Morse-Code-Straight-Key-Simulator/blob/main/Previous%20Versions/Version%201.6.html

Version 1.7: https://github.com/Reperium/Morse-Code-Straight-Key-Simulator/blob/main/Previous%20Versions/Version%201.7.html

Version 2.0: https://github.com/Reperium/Morse-Code-Straight-Key-Simulator/blob/main/Previous%20Versions/Version%202.0.html
⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯⎯
Morse Code Straight Key Simulator
~17,400 lines of Hypertext Markup Language, Cascading Style Sheets, and JavaScript using Google Fonts. This uses no other external dependencies and is a static website.

Core Simulator
The left panel hosts a straight key bar that responds to mouse, touch, and configurable keyboard input. An input generates a tone customizable in the settings section.
Tone controls include frequency (Hertz), waveform (sine, square, triangle, sawtooth), attack and decay envelopes (milliseconds), and optional background static noise. Transmission speed is adjustable from 1 to 50 WPM using the 50-unit PARIS word standard or 60-unit CODEX standard. This is modified by a frame rate slider ranging from 10 frames per second to 360 frames per second. A green highlight overlays the WPM slider, affected by the user's average transmission speed and their current error rates to suggest the best transmission speed.

Multi-Language Dictionaries
The right panel stores nine script dictionaries horizontally scrollable: Gerke, International, Cyrillic, Japanese Wabun, Greek, Hebrew, Arabic, and Korean Morse Code. A </> navigation system and arrow-key handler move between cards. Each card has its own notes section, custom rows, and error history. The colored rounded boxes store every instance and error for every input and release.

Each script shares numbers 0 through 9, their full set of punctuation, procedural signs, and Universal Q-Codes from QRA to QUZ. Therefore, inputting a full sequence overrides the previous Morse code for all scripts.

Hangul composition implements the standard Unicode Hangul Composition Algorithm (UAX #15) to merge consecutive jamo characters into precomposed Korean syllables in real time. Japanese Wabun supports yōon, dakuten, and handakuten multi-part characters that collapse from their component kana.

Error Tracking & Analytics
Every input and release is tracked for the dot (.), dash (-), unit space (➔), letter space (␣), and word space (/). Besides the quantity and the user's fist ratios, the metrics panel tracks the actual vs. ideal duration and error percentage. A color-coded error indicator is present besides the average error percentage in the dictionary for each row. It is blue when the error is ≤1%, green when the error is ≤2.5%, yellow when the error is ≤5%, red when the error is ≤10%, and black when the error is >10%.

Clicking the rounded colored boxes displays a numbered list of every attempt. This can be sorted from the newest first or the oldest first. Green outlines wrap dots, dashes, and unit spaces for each letter, while black outlines outline word letter spaces. Gray vertical lines flank unit-space chips. The character timings in units, milliseconds, and frames are placed in the header, alongside the script, Morse Code, and live transmission speed data. All error data, WPM history, and detailed per-symbol breakdowns persist to localStorage and survive page reloads.

Additional Features
Broadcast History: Session recording with timestamped messages
Callsign Generator: 20 country prefixes with authoritative restriction rules, numeral selection, and 3-letter suffix input
Conflict Toggle: For characters sharing the same morse code, a pill toggle selects the preferred decoding
Keybinds: Six actions can be configured to anything from a standard 60% keyboard visualized in the user interface.
Notes Section: A text box allowing specific language input to encode into Morse Code, along with audio playback, copying, line counters, and highlighting.
Miscellaneous Page: Archives previous versions to visit or download, my contacts, account data manager, credits, and notable websites.
