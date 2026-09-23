# Jazz Jackrabbit · Remastered

My dad, Arjan Brussee, co-created Jazz Jackrabbit with Cliff Bleszinski back in 1994. Arjan wrote the code in the Netherlands, Cliff designed it, and Epic MegaGames put it out on MS-DOS: a green rabbit in a red bandana, carrying a gun roughly his own size, fighting a turtle named Devan Shell.

Opus 5.5 came out on September 22, 2026, and that same day I asked it, through Claude Code, for a modern Jazz that still plays like the old one. This repo is what came back. It's a single HTML file of about 180KB, roughly the size of one of the screenshots below, and there isn't one image, sound or font file anywhere in it; every sprite, tile, backdrop, song and level gets drawn or composed by code when the page loads.

**[Play it in your browser →](https://juliusbrussee.github.io/jazz-jackrabbit-remastered/)** Keyboard or gamepad. You can also download `index.html` and open it offline.

![Gameplay preview](media/gameplay-preview.gif)

🎬 [Watch 77 seconds of gameplay with sound](https://juliusbrussee.github.io/jazz-jackrabbit-remastered/media/jazz-gameplay.mp4). Don't blame me for the gameplay, I had Opus 5.5 play for me: it wrote a little autopilot, pointed it at the levels and recorded the result frame by frame.

## What's in it

Five worlds named after planets from the original: Diamondus, Tubelectric, Medivo, Letni and Technoir. Medivo ends with an armoured knight turtle who throws axes and sends shockwaves along the floor, and Technoir ends with Devan Shell himself, hovering over the rooftops in a saucer and dropping bombs on you.

Jazz can sprint, hover with his helicopter ears, butt-stomp through cracked floors and pick up four guns (Blaster, Bouncer, Toaster and RF missiles). Most levels hide a secret room or two behind blocks you can shoot, and if you eat enough junk food you get a sugar rush and become briefly unkillable.

## How it was made

One prompt, then a few follow-ups asking for the GitHub repo, the screenshots and the video.

Nothing in the game is a picture. Jazz is a rig of shapes (ears, bandana, belly, gun) posed differently for each animation frame; every frame gets snapped to hard pixels, lit from the top left and outlined at load, which is why he reads as pixel art rather than a vector drawing. The rock with gems in it, the neon city and the castle bricks are all textures computed pixel by pixel, and the music is a tiny tracker running through Web Audio, with chord progressions, drum patterns and a lead melody for each world.

The levels are built from hand-written scripts of pieces like hills, tunnels, spring ledges, zig-zag towers and hidden rooms. A checker walks every level as a jump graph to make sure the exit can be reached. During the build it caught a real dead end in Letni, where a tunnel ceiling stopped you jumping onto the next wall.

## Controls

| Key | What it does |
|---|---|
| Arrows / WASD | Move, look up, crouch |
| Space / Z | Jump (hold it to go higher, press again in the air to hover) |
| Down in mid-air | Butt-stomp |
| X / J / Ctrl | Fire (hold Up to shoot upward) |
| Shift | Run |
| Q / E / 1-4 | Switch weapon |
| Down + Jump | Drop through a platform |
| Esc / P · M · F | Pause · Mute · Fullscreen |

If you want to skip ahead, `index.html?level=3&x=120` starts you in level 3 at column 120.

## Screenshots

![Title screen](screenshots/title.png)

| | |
|---|---|
| ![Level intro card](screenshots/intro.png) | ![Diamondus: blasting turtle goons over a spike pit](screenshots/diamondus.png) |
| Every world opens with a title card. | Diamondus, where the gems are set right into the rock. |
| ![Helicopter ears over a pit](screenshots/copter.png) | ![Secret area revealed](screenshots/secret.png) |
| Helicopter ears get you over most pits. | Shoot the cracked blocks and a hidden room opens up, 1-UP included. |
| ![Sugar rush](screenshots/sugar-rush.png) | ![Tubelectric boost pad](screenshots/boost.png) |
| Sugar rush: 60 snacks and nothing can touch you for a while. | Tubelectric's boost pads throw you across bottomless gaps. |
| ![RF missiles](screenshots/rf-missiles.png) | ![Medivo swinging platform](screenshots/medivo-swing.png) |
| RF missiles against a robo-turtle, with the dark worlds lit in real time. | Medivo at night, riding a swinging platform past torches and bats. |
| ![Toaster flamethrower](screenshots/toaster.png) | ![Boss: Sir Shellington](screenshots/boss-knight.png) |
| The Toaster is a flamethrower, and knights hate it. | Sir Shellington, the Medivo boss, mid axe-throw. |
| ![Letni sunset dunes](screenshots/letni.png) | ![Technoir rooftops](screenshots/technoir.png) |
| Letni's sunset dunes, with afterimages once you hit top speed. | Technoir: rain, neon signs and a lot of rooftop gaps. |
| ![Boss: Devan Shell](screenshots/boss-devan.png) | ![Level results](screenshots/results.png) |
| Devan Shell. Aim up, keep moving. | The tally screen after each world. |

![Ending](screenshots/ending.png)

## Credits

The original Jazz Jackrabbit (1994) was made by Arjan Brussee and Cliff Bleszinski and published by Epic MegaGames. This remake is an unofficial fan project that isn't affiliated with or endorsed by Epic Games, and Jazz Jackrabbit is a trademark of its owner.
