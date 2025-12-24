# 🥁 Rok Drummer

**© TrojanNemo, 2015–2025**  
*Dedicated to the rhythm gaming community*

![Rok Drummer](https://nemosnautilus.com/drums/drumrokkerv130.jpg)

---

## About

**Rok Drummer** began as a proof of concept created to answer a simple question:

> *Could I interpret signals from my Xbox 360 Rock Band drum kit on a PC and make it behave like an electronic drum kit?*

Everything beyond that was largely an afterthought — so don’t take it too seriously.

Rok Drummer is first and foremost a **fun experimental project**. Expect quirks, some latency, and a limited feature set — but also a surprisingly flexible way to play drums outside the game.

---

## Supported Hardware

Rok Drummer is currently confirmed to work with:

- 🎮 **Xbox 360 Rock Band 1 wired drums**
- 🎮 **Xbox 360 Rock Band 2 / Rock Band 3 / The Beatles: Rock Band wireless drums**  
  (via Microsoft’s Xbox 360 Wireless Adapter)
- 🥁 **Electronic drum kits**  
  connected via Xbox 360 or PlayStation 3 **MIDI Pro Adapter (MPA)**
- 🎮 **PlayStation 3 Guitar Hero 5 wireless drums**

If you can confirm support for other kits, please let me know.

If you have a drum set that *almost* works, I may be able to add support with your help — send me a message and let’s experiment.

---

## Drum Kits

Rok Drummer includes **five drum kits**, matching those found in **Rock Band 3 Practice Mode**.

### Custom Drum Kits

You can use your own kit sounds:

1. Create a folder under `/kits/`
2. Place your samples inside
3. Follow the naming format of existing kits

Rok Drummer detects all kits at runtime.

You can switch kits:
- Using the **dropdown menu**, or
- By pressing **Left / Right** on your drum kit

---

## How to Play

Rok Drummer supports **three input methods**.

### 1️⃣ Drum Kit (Recommended)

Just play your drums like you normally would.

- Rok Drummer responds in real time
- Supports a **separate flam sample**
  - Activated by hitting **Snare + Yellow Tom** simultaneously

### 2️⃣ Mouse

- Click any pad, cymbal, or pedal to trigger its sound

### 3️⃣ Keyboard

- Play the entire kit using keyboard bindings
- Key bindings can be customized by editing:

drummer.config

(located in the `/bin/` folder)

> 💡 With key remapping tools, it may be possible to use a Wii drum kit mapped to keyboard input — try it and see!

While using **any** input method, you can scrub forward or backward in time using the mouse scroll wheel.

---

## Default Key Bindings

| Component | Key |
|--------|-----|
| Snare | A |
| Flam | W |
| Yellow Tom | S |
| Blue Tom | D |
| Green Tom | F |
| Yellow Cymbal | K |
| Blue Cymbal | L |
| Green Cymbal | ; |
| Bass Pedal | Space |
| Hi-Hat / 2nd Bass | J |
| Previous Kit | Page Up |
| Next Kit | Page Down |
| Drum Volume Up | Numpad + |
| Drum Volume Down | Numpad - |

---

## 🎼 Play-Along Mode

Enable Play-Along Mode by:

- Clicking `Options → Play-along mode`
- Pressing **F5**
- Dragging a **CON / LIVE** file onto Rok Drummer

### Features

- Plays song audio
- Displays the **Expert drum chart**
- Supports:
- Expert
- Hard
- Medium
- Easy  
*(if charted)*

> ⚠️ Chart visualization is best-effort and **not accurate enough for testing songs** — always test in-game.

Charts update **in real time** without stopping playback.

### Visual Styles

- Default: vertical scrolling
- Rock Band–style highway:
- Right-click the track
- Select **Style → Rock Band**

---

## Options

- **Double bass pedal** — Converts hi-hat pedal into second bass pedal
- **Force closed hi-hat** — Forces closed hi-hat sound on yellow cymbal
- **Hit velocity controls volume** — Volume based on strike strength
- **Play-along mode** — Enables chart playback
- **Silence drums track** — Mutes original drum audio if multitrack
- **Show chart selection**
- **AutoPlay with chart** — Rok Drummer plays the chart automatically
- **Show metronome**
- Tempo controls included
- Replace `metronome.wav` in `/res/` to customize sound

---

## Volume Controls

- **Track Volume** — Controls song playback volume
- **Drum Volume** — Controls sample volume
- Click label
- Use **Numpad + / -**
- Use **Up / Down** on drum kit

---

## Layouts

Rok Drummer includes several preset layouts and supports **fully custom layouts**.

- Layouts affect **visual appearance only**
- Input mapping is controlled separately under:

Controllers → Select drum kit


### Custom Layouts

- Click `Layouts → Customize layout`
- Drag components to reposition
- Replace layout images following existing naming conventions

> ⚠️ Due to .NET transparency limitations, the background image must contain the full drum kit image.

See the **Tron layout** for an example of a radically different design.

---

## 🎆 Stage Kit Support

Rok Drummer can drive your **Rock Band Stage Kit** for a full light show.

### Setup

1. Click **Stage Kit**
2. Select the controller number

That’s it — the Stage Kit responds to:
- Live playing
- Keyboard input
- AutoPlay charts

### LED Mapping

- **Snare** → Red LEDs
- **Yellow Tom / Hi-hat** → Yellow LEDs
- **Blue Tom / Ride** → Blue LEDs
- **Green Tom / Crash** → Green LEDs
- **Kick / Hi-hat (double bass)** → Strobe

**Fog machine:**  
Press the **Back** button on your drum kit.

---

## Customization

Almost everything Rok Drummer uses lives in the `/res/` folder.

You can:
- Replace images (keep names, formats, dimensions)
- Modify or create layouts
- Customize drum kit sounds

### Custom Drum Sounds

- Replace `.wav` files inside an existing kit folder
- Rename the folder to rename the kit
- Add unlimited new kits as long as naming conventions are followed

---

## Background Mode

When minimized, Rok Drummer lives in the **system tray** and continues responding to drum input.

You don’t need to keep it visible — just play.

---

## Final Notes

This is a **fun experimental project**, not a professional drum engine.

Expect:
- Some latency
- Rough edges
- Limited features

But also:
- A lot of fun

Enjoy.

---

## Credits

- **DJ Shepherd** — X360 library  
- **raynebc** — MIDI expertise  
- **Mark Heath** — NAudio.MIDI  
http://naudio.codeplex.com/  
- **Ian Luck** — BASS audio library  
http://www.un4seen.com/  
- **Bernd Niedergesaess** — BASS.NET API  
http://bass.radio42.com/  
- **David** — drum velocity research  
http://www.dwsk.co.uk/  
- **Racer_S** — original X360 controller emulator  
http://tocaedit.com  
- **max13004** & **ludox** — Xinputemu v3.1  

