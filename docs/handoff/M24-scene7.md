# Handoff: M24 scene, round 7: three faces for Mary, side by side (second account, branch `other/M24-scene`)

You continue the porch scene. Run `git merge main` first, then read:
- `mockups/mary/round12/NOTES.md`: the files, the switches, the render recipe, and what's still open;
- `docs/handoff/done/M24-scene6.md`: the last round;
- the **M24** section of `docs/mary-roadmap.md`;
- `mockups/mary/concepts/README.md`, and look at `04-lineup-pairs-sam-picked.webp` and `05-mary-faces-rejected.webp` in that folder.

**Andy, 2026-11-05:** "I'm still pretty sure we're going to redo her entire face." And: "as long as we can get that stuff right and we can get it pushed in on her right and we get her face a little better, as long as her conversations are good, then everything else can be overlooked." Earlier: he isn't sold on how human her face looks. "It needs to be a character of some sort. It don't need to be a childish little character, but it needs to be a character." And "if I really want this to work and take off, we're gonna have to nail the character."

**The job:** build three really different faces for Mary on the same body, in the same light, so Andy can pick one. This is the most important picture in the project. Take your time with it.

**What each face has to be:**
- Clearly a robot's face, and clearly a character, not a human face painted on a ball.
- Warm and kind, and easy to read from across a room by someone with weak eyes.
- Visibly female without a doll face.
- Grown-up: for an 80-year-old, not a child.
- Able to do what the scene needs: blink, look where `setGaze` sends it, raise and lower its brows, shut its eyes for asleep (`?lantern=asleep`), and move its mouth with one loudness value. Her voice drives the mouth in the app, so the mouth needs a clear closed-to-open range. No hinged jaw.

**Already rejected or ruled out. Don't come close to these:**
- Lens eyes ("look like a camera"; a robot face that reads as a camera watching residents is the fastest way to lose them).
- A gauge face ("a gas mask"), and a clock face ("a human face on an object").
- Anything like stitching, seams or a zipper around the mouth ("looks like stitching around the mouth like Frankenstein… the whole vibe is just dead"), and "the rusty rivets on her forehead." Try each face without the little rivet now on her helmet's forehead.
- A grille over the mouth (it "reads as a gag").
- A glowing-eyed machine. Any glow is low and warm, like a coal, never a lit-up stare.
- A carved human shape (it reads as "a mannequin or puppet"), and anything photo-real.
- Gloss, huge eyes, sparkle catchlights, blush, or a head too big for her body.

**Three directions to start from.** Push each one as far from the others as it will go. You may replace any of them with a better idea of your own, as long as it stays inside the rules above:
1. **The sign painter.** A flat enamel plate with a few confident painted shapes, like a hand-lettered 1950s sign or an old advertising character. Simple dark oval eyes, a single-stroke brow, almost no nose, and a painted mouth that changes shape.
2. **The warm lamp.** Eyes are two softly warm glass discs behind simple metal lids, kin to the lantern on her porch, with no rings, irises or apertures. Small enamel bars for brows. Her mouth is a soft line of low light that widens as she talks.
3. **The whittled face.** Her face plate shaped in shallow planes, the way a porch carver cuts a brow and cheek, in matte milk paint over the enamel. Painted almond eyes and a soft mouth. This is the closest to a face, so keep it plainly made by hand.

You may reshape the helmet's opening to suit each face. Keep her robin's-egg and cream family, her shawl and her body as they are.

**Do, in this order:**
1. Add a `?face=` switch, with `a`, `b` and `c` for the three faces and the current face staying as the default. All three must work with every existing pose and `?lantern=` mood.
2. Build and refine them one at a time, looking at a close-up render of each as you go. Faces are where a blind guess goes wrong, so keep looking and keep fixing.
3. Make the sheets Andy will judge from, night light, same framing, one image each:
   - `shots/r7-three-faces.jpg`: the three faces side by side at rest, head and shoulders, with a plain-words name under each;
   - `shots/r7-faces-grid.jpg`: three columns (the faces) by four rows (rest, talking with the mouth open, listening with brows up, asleep).
4. Render each face once in the full resting shot (`shots/r7-rest-a.jpg`, `-b`, `-c`), so he can see it at the size it'll really be.
5. **Only if your context allows, two small leftovers from round 6:** the lantern's painted cheeks read as big orange patches at a low wick, so soften or remove them; and her hands get cut off at the bottom of the talk framing when they come up, so keep them lower or in frame.

**Memory:** the laptop runs low. Render one shot at a time with a fresh Edge profile, delete each profile after its shot, and keep no more than one server running.

**Rules:**
- Touch only `mockups/mary/round12/` and `docs/handoff/done/M24-scene.md`.
- No app changes, no Gemini calls, and nothing about her brain (D26).
- NOTES.md holds facts and task state only, never rules.
- Commit on `other/M24-scene` after each face. Never push, and never merge into `main`.
- If your context passes about 200K, commit `WAITING: context full`, with NOTES.md updated first.

**Models:** you do all of it yourself, at extra-high effort, with no helpers.

**Finish:** commit `DONE: M24 scene round 7`. The message carries:
- three plain lines for Andy, one about each face, with its name;
- which one you'd pick, and why, in one line;
- the sheets' file names;
- what's still not right.

Then stop.
