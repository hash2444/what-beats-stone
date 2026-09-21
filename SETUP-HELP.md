# What Beats Stone? - Setup help

Everything you need to get **What Beats Stone?** running, step by step. If something goes wrong, check *Troubleshooting* at the end.

## What you need

- Windows 10 or Windows 11 (64-bit)
- [Ollama](https://ollama.com) installed and running (`ollama serve`, or simply the Ollama app in the tray)
- The referee model: open a terminal and run `ollama pull qwen2.5vl:7b` (about 6 GB)
- A graphics card is recommended but not required

## Install and start

1. Download **`WhatBeatsStone.exe`** from the [Releases page](../../releases) - or directly from the file list of this repository.
2. Put it anywhere you like, for example in its own folder. There is **no installer**.
3. Double-click it.
4. Windows may show a blue **SmartScreen** window ("Windows protected your PC"), because the file is not code-signed. Click **More info**, then **Run anyway**. Your antivirus may also scan the file for a few seconds on the first start.

## First start

1. Make sure Ollama is running (its icon is in the system tray).
2. Start `WhatBeatsStone.exe`. The game starts with a random first thing (Stone, Fire, Water, Paper or Sun).
3. Type something that beats it and press **Enter** or **GO**. Wait a moment while the AI thinks.
4. If the answer counts, it becomes the new thing. If not - or if you repeat a word - it is game over. *new game* starts again.

## Troubleshooting

**It says Ollama is not reachable**

Start the Ollama app (or run `ollama serve` in a terminal) and try again.

**It says the model was not found**

Run `ollama pull qwen2.5vl:7b` once. Any other model works too if you change the name in the source; this build uses `qwen2.5vl:7b`.

**The AI takes very long**

The first answer loads the model into memory (up to a minute). Later answers are faster.

**Nothing happens when I double-click it**

Wait 10-20 seconds on the very first start (antivirus scan / first-time unpacking). If it still does not appear, right-click the file -> *Properties* -> tick *Unblock* -> *OK*, then start it again.

**SmartScreen or my antivirus complains**

The file is unsigned, which triggers warnings for every small tool. Use *More info* -> *Run anyway*. If your antivirus quarantines it, add the folder to its exclusions or re-download.

## Uninstall

Delete the `.exe`. If the program stored settings (see above), delete that folder too.

## Still stuck?

Open an **Issue** on this repository and tell me your Windows / Minecraft version and what you see (a screenshot helps).

---

Made by **dev:#2444** - [github.com/hash2444](https://github.com/hash2444)
