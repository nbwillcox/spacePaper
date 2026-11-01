# SpacePaper

A free, silly delivery game with a head nod to the classic paper-route arcade game: you are a kid on a **hoverboard** delivering *The Daily Nebula* to a floating **space suburb**. Land papers on welcome mats and in mailboxes, smash the windows of the grumpy neighbours, dodge hover-cars, space-dogs and meteors, and survive the weekly boss.

**Play it in your browser:** https://nbwillcox.github.io/spacePaper/

The title kid, the game-over kid and the three boss portraits are AI-generated pixel-art pictures (Z-Image Turbo via ComfyUI, pixelated and palette-reduced, in `assets/`). Everything in the street - the NES-style oblique view, houses, cars, dogs, bosses, effects - is drawn in code by a small software pixel renderer (480x270, no anti-aliasing, 5x7 bitmap font), and all sound and music is synthesized with Web Audio. No build step. A sibling of [SpaceDuckHunter](https://github.com/nbwillcox/SpaceDuckHunter), [SpaceJong](https://github.com/nbwillcox/spacejong) and the other Space games.

## How to play

- A week is seven routes, **Monday to Sunday**. The street scrolls diagonally with the houses on one side, like the original; steer across it, speed up or brake.
- **Subscribers** are the glowing yellow houses (the sign over the roof shows their state). Land a paper on the **welcome mat** (250), the **patio** (150) or in the **mailbox** (100). The door counts too.
- **Non-subscribers** are the dark, grumpy houses. **Smash their windows** (150 each), ding their mailbox (50), knock on the door (50). Do **not** break a subscriber's window - they cancel (-250).
- Any subscriber you miss by the end of the route cancels. Deliver everything for a **perfect route** bonus and two new subscribers. Lose every subscriber and you are fired.
- Hazards: oncoming and same-way hover-cars, cross-street traffic (from Tuesday), **space-dogs** (bonk them with a paper), skaters, robo-mowers, sprinklers, cones, black holes, UFO tractor beams, and meteors later in the week.
- **Hop** to clear low obstacles. Ride up a **ramp** for a stunt bonus.
- **Paper bundles** restock your bag. A **throw guide** (Settings) shows where a paper would land.
- Chain scoring hits for a **combo multiplier** (up to x5); a crash resets it.
- After each route (Monday-Saturday): the **Hover Academy** bonus course - targets, ramps and hoops, unlimited papers, crashes only cost time.
- **Sunday ends with a boss**, one per week: Rex-9000 the robo-bulldog (dodge the charge, hit him while he is dizzy), Postmaster Gorp (wait out the shield), Big Mower (hop the blade, hit the glowing grass bag). Then the next week starts, harder.

### Power-ups

| Icon | Effect |
| --- | --- |
| **S** | Super speed (and you smash small obstacles) |
| **2** | Double toss |
| **O** | Omni toss - every throw sprays papers in all directions |
| **I** | Invincible - cars, dogs and obstacles bounce off or get smashed |
| **8** | Infinite papers |
| 1UP | Extra life |

## Controls

| Action | Keyboard | Gamepad |
| --- | --- | --- |
| Steer / faster / brake | Arrows or `WASD` | Left stick or D-pad |
| Throw left | Left mouse button, `Z`, `Q` or `J` | `LB`, `X` or `LT` |
| Throw right | Right mouse button, `X`, `E` or `K` | `RB`, `B` or `RT` |
| Auto-throw at the nearest target | `C` or `Enter` | `Y` |
| Hop | `Space` | `A` |
| Pause | `P` or `Esc` | `Start` |

### On a phone or tablet

Play in landscape. A floating stick on the left steers the hoverboard (up = faster, down = brake); on the right, tap **THROW** to toss a paper to that side, **HOP** to jump over low things, and **AUTO** to throw at the nearest target. The pause button opens the menu. The on-screen controls appear on touch devices automatically; Settings has size, opacity and a left-handed layout. Use your browser's *Add to Home Screen* to install it as a full-screen app.

### Controller

Plug in a gamepad and it just works: the stick or D-pad steers (up = faster, down = brake), **LB / X** throws left, **RB / B** throws right, **A** hops, **Y** auto-throws at the nearest target, **Start** pauses. In menus the D-pad / left stick moves the highlight, **A** selects, **B** goes back and **Start** plays or resumes. **Settings -> Controller** has a dead-zone slider and lets you remap every button.

## Settings

Volumes (master / music / effects), difficulty (Cozy, Normal, Hard), throw guide, screen shake and reduced motion. Saved in your browser, as are the local top-10 high scores.

Debug URL flags: `?day=N` and `?week=N` (start there), `?phase=course|boss`, `?skip=1` (skip the newspaper), `?bot=1` (autopilot), `?god=1` (invincible), `?touch=1` (force the touch UI).

## License

[CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/) - free to play, share and remix for non-commercial use, with a link back to this repository.
