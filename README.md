# 🍳 Cooking Timers

Smart, step-by-step cooking timers that coordinate complex recipes with multiple parallel tasks.

## Timers

| Recipe | Source | Time | Link |
|--------|--------|------|------|
| [Baby Back Ribs](./ribs-timer.html) | Alton Brown / Good Eats | ~4.5 hrs | [View](./ribs-timer.html) |

## Features

- ⏱️ **Elapsed + Remaining time** with estimated finish time
- 🔔 **Audio alerts** when steps trigger (Web Audio API)
- 📱 **Push notifications** for background alerts
- 🔒 **Wake Lock** keeps phone screen on while cooking
- ✅ **Checkboxes** to mark steps complete manually
- ⏩ **±5 min adjust** if you're ahead or behind schedule
- 📊 **Progress bar** showing overall completion
- 🍖 **Doneness cues** so you know what to look for
- 🔧 **Equipment list** so you're prepared
- 🖨️ **Print view** for paper backup
- 💾 **Persists through refresh** via localStorage

## Usage

1. Download or clone this repo
2. Open any timer HTML file directly in your browser
3. Hit **START COOKING**
4. Follow along!

> **Note:** Wake Lock only works when opening the file directly in your browser, not in iframes.

## How These Are Made

1. Take a photo of a recipe card
2. Upload to Claude
3. Claude extracts steps, estimates times, adds doneness cues
4. Download the generated HTML timer

## Adding New Timers

Each timer is a self-contained HTML file with:
- Embedded CSS
- Embedded JavaScript
- Hardcoded `steps` array with timing data

To add a new timer:
1. Copy an existing timer as a template
2. Update the `steps` array with your recipe
3. Update ingredient lists and equipment
4. Test the timing flow

## License

MIT — use freely for your own cooking adventures.

## Credits

Timer UI inspired by [Simon Willison's tools](https://github.com/simonw/tools) — a collection of single-file HTML tools.
