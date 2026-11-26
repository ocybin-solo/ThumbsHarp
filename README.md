# Thumb Harmonica

A two-thumb virtual harmonica that runs in your browser. One file, no install, no dependencies.

**Play it:** https://ocybin-solo.github.io/ThumbsHarp/

Best on a phone held in landscape. Raise the volume and tap to start.

## How it plays

- **Left thumb is your breath.** Slide along the left track. Up-left is draw, down-right is blow, and the middle is silent. The further you slide, the harder you breathe. Slide toward the middle of the screen for vibrato.
- **Right thumb is the harmonica.** Drag the ribbon of holes past the fixed playhead. Flick and let go and it keeps rolling like a trackball. Touch it to stop.
- **Pull outward to widen.** Moving the right thumb outward adds holes one at a time around the middle hole, nearest side first (1, 2, 3, 4, then 5 holes) for dyads, chords and runs.
- **Push inward to split.** Like tongue-blocking on a real harp, this plays the middle hole plus a partner above it and skips the holes between. Pushing deeper steps from a third to a fifth to an octave, using whichever hole in the tuning has that interval (if there isn't one, it holds the previous interval).

## Controls

- **Tuning:** Richter, Country, Natural minor, Harmonic minor, Gypsy (Hungarian minor)
- **Key:** G up to F♯
- **Tone:** Harmonica, Clarinet, Sax, Flute
- **Bright:** how much overtone the tone has
- **Swipe:** how far the ribbon moves per swipe
- **Flip:** swaps draw and blow on the left track
- **◐:** theme, cycling Auto, Light and Dark
- **ⓘ:** credits and license
- **⛶:** full screen

## Gamepad

Tested with a Steam Controller (its pads and its sticks both work).

- **Left pad or stick** works like the left thumb (breath and vibrato), and the **right pad or stick** works like the right thumb (the ribbon).
- **Triggers** open neighbouring holes in analog stages: the left trigger opens up to three holes to the left of the one under the playhead, and the right trigger does the same on the right. The total stays capped at five holes.
- **D-pad** moves along the top row of controls. A starts editing a control and accepts it, and B cancels.
- **Back** (or the G key on a keyboard) shows a raw readout of the axes and buttons the browser is receiving, which is useful for debugging a layout.

### Steam Controller setup (what worked for me)

1. Add Chrome to Steam as a non-Steam game.
2. Open its properties and rename it to whatever you like (for example "Thumb Harmonica"). In the launch options, put `https://ocybin-solo.github.io/ThumbsHarp/`. Optionally add `--kiosk` before the link to start in full screen.
3. Open the controller configuration for it and set both pads to **Joystick Move**. A stick works too. I did not enable adaptive centering.

That's all it took. Other controllers should work if the browser recognises them as a gamepad, but I've only tried the Steam Controller.

## Run it locally

Download `index.html` and open it in a modern browser. Chrome and Edge are the best-tested. The Gamepad API generally needs https or a local file, so a hosted copy like the link above works fine.

## Credits

- **Idea, design and testing:** Cybin
- **Code and suggestions:** Claude (Anthropic)
- **Extra-holes (push/pull) code:** first drafted by Gemini (Google), later refined with Claude. Gemini also helped shape the idea.
- **Crash fix:** ChatGPT (OpenAI)

## License

MIT. See the `LICENSE` file. Free to use, share and modify.
