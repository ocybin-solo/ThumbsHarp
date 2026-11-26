# ThumbsHarp

A two-thumb virtual harmonica that runs in your browser. One file, no install, no dependencies.

**Play it:** https://ocybin-solo.github.io/ThumbsHarp/

Best on a phone held in landscape. Raise the volume and tap to start.

## How it plays

- **Left thumb is your breath.** Slide along the left track. Up-left is draw, down-right is blow, and the middle is silent. The further you slide, the harder you breathe. Slide toward the middle of the screen for vibrato.
- **Right thumb is the harmonica.** Drag the ribbon of holes past the fixed playhead. Flick and let go and it keeps rolling like a trackball. Touch it to stop.
- **Push or pull for more holes.** Move the right thumb inward or outward to open onto the neighbouring holes, for up to four holes at once (chords, dyads and runs).

## Controls

- **Tuning:** Richter, Country, Natural minor, Harmonic minor, Gypsy (Hungarian minor)
- **Key:** G up to F♯
- **Tone:** Harmonica, Clarinet, Sax, Flute
- **Bright:** how much overtone the tone has
- **Swipe:** how far the ribbon moves per swipe
- **◐:** theme, cycling Auto, Light and Dark
- **ⓘ:** credits and license
- **⛶:** full screen

## Gamepad (experimental, untested on real hardware)

Gamepad support is built in but I haven't been able to test it yet, so feedback is very welcome.

- Left pad or stick works like the left thumb, and the right pad or stick works like the right thumb.
- D-pad moves along the top row of controls. A starts editing a control and accepts it, and B cancels.
- Back (or the G key on a keyboard) shows a raw readout of the axes and buttons the browser is receiving, which is useful for debugging a controller layout.

### Steam Controller

The idea is to use the touchpads as the two thumbs. The browser only sees them as joystick axes if Steam Input is set up for that:

1. Run the browser with a gamepad-style Steam Input layout (for example, by adding it to Steam as a non-Steam game).
2. Set both touchpads to **Joystick Move**, so finger position becomes stick position and lifting goes back to zero.
3. Set the touchpads' deadzone so that placing a finger doesn't nudge the controls.

I haven't gotten this working on my own setup yet. If you have, I'd love to hear what layout worked.

## Run it locally

Download `index.html` and open it in a modern browser. Chrome and Firefox are the browsers that I tested. The Gamepad API generally needs https or a local file, so a hosted copy like the link above works fine.

## Credits

- **Idea, design and testing:** Cybin
- **Code and suggestions:** Claude (Anthropic)
- **Extra-holes (push/pull) code:** first drafted by Gemini (Google), later refined with Claude. Gemini also helped shape the idea.
- **Crash fix:** ChatGPT (OpenAI)

## License

MIT. See the `LICENSE` file. Free to use, share and modify.
