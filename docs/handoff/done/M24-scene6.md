# Handoff: M24 scene, round 6: the layout and the light (second account, branch `other/M24-scene`)

You continue the porch scene. Run `git merge main` first, then read:
- `mockups/mary/round12/NOTES.md`: the files, the switches, the render recipe, and what's still open;
- `docs/handoff/done/M24-scene5.md`: the last round;
- the **M24** section of `docs/mary-roadmap.md`, especially "Andy, on round 5" and "Andy's calls (2026-11-05)".

**Andy, on round 5 (2026-11-05), in his words:**
- The glint on the side of her head "kind of takes you out of it… You're just going to have to cut the glow down."
- The lantern "is sitting right up against the window. Side of the house that doesn't seem very safe."
- The table: "If it doesn't show her doing that [reaching the radio without leaning around it], then the physics are broken."
- The camera: "when she's talking, it might move in a little closer on her. And when she's not, it backs up. And when she reaches for something, it backs up a little more."
- What matters most: "as long as we can get that stuff right and we can get it pushed in on her right and we get her face a little better, as long as her conversations are good, then everything else can be overlooked."

**Do, in this order:**
1. **Move the lantern off the wall.** It hangs on its chain from the porch ceiling beam, a little in front of the swing and to her right (the viewer's left), above the side table and well away from the house wall. It should light her face from the front side, kindly. Keep its face, its moods (`?lantern=`) and the `?lamp=` levels.
2. **Put the table beside the swing.** Move the swing farther from the house, and set the table with the radio right beside the swing's arm on the viewer's left, not in front of it. Her radio reach (`?pose=radio`) must land on the dial without leaning around anything, and her lantern reach (`?pose=lamp`) must reach the hanging lantern's wick knob naturally. If a reach can't look natural, move the object, not her shoulder.
3. **No glint.** Make her helmet enamel satin, so no bright highlight sits on the side of her head in any shot. The new lantern place should help. Keep a soft sheen; nothing should read as wet or plastic.
4. **Push the camera in.** The resting framing is closer on her than round 5. She's the subject, with the lantern and radio in frame.
5. **The gentle moving camera.** Three framings: talking (a little closer on her), resting (backed up), and reaching (backed up a little more). Moves are slow and eased, several seconds each, never a cut, so no one gets dizzy. Add a switch for each framing, and one that plays a short sequence (rest, talk, rest, reach) so it can be watched live. In the app these become gentle zooms of the whole picture (the hybrid plan in the roadmap), so keep the moves simple: in and out, a little drift, no swings around her.
6. **The leftovers from round 5:** the turned-down lantern glass stays a bit pale; re-render the radio and point poses with the lantern in its new place. The sky is evening and night only now (Andy's call), so spend nothing more on `?time=day`.

**Don't touch her face** beyond what the satin helmet needs. A face round, with three faces side by side, comes next with its own brief.

**Shots to render and check** (night unless noted): the resting main shot, the evening resting shot, the three camera framings, the radio reach, the lantern reach, the point pose, and a close-up of her head from the side the glint was on. Look at each one yourself before you call it done.

**Memory:** the laptop runs low. Render one shot at a time with a fresh Edge profile, delete each profile after its shot, and keep no more than one server running.

**Rules:**
- Touch only `mockups/mary/round12/` and `docs/handoff/done/M24-scene.md`.
- No app changes, no Gemini calls, and nothing about her brain (D26).
- NOTES.md holds facts and task state only, never rules.
- Commit on `other/M24-scene` after each step. Never push, and never merge into `main`.
- If your context passes about 200K, commit `WAITING: context full`, with NOTES.md updated first.

**Models:** you do all of it yourself, at extra-high effort, with no helpers.

**Finish:** commit `DONE: M24 scene round 6`. The message carries:
- three plain lines for Andy;
- which shots you checked, with their file names;
- what's still not right.

Then stop.
