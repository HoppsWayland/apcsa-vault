# 🏠 AP Computer Science A
### Your Interactive Reference & Notebook

Welcome! This vault is your companion for the entire AP CSA course. Everything you need is here — explanations, examples you can actually run, and space for your own notes. Think of it as a textbook that talks back.

---

## ⚙️ First-Time Setup

Before you dive into the notes, you need to do two things: install Obsidian, and install the Execute Code plugin. This only takes a few minutes.

### Step 1 — Install Obsidian

> [!WARNING] Chromebook Users — Read This First
> Obsidian must be installed as a **`.deb` file** through your Linux environment. Do **not** use the AppImage version — it runs in an isolated container and won't be able to run Java code.

1. Open your **Linux terminal**
2. Download the latest Obsidian `.deb` package:
   ```bash
   wget https://github.com/obsidianmd/obsidian-releases/releases/latest/download/obsidian_amd64.deb
   ```
3. Install it:
   ```bash
   sudo apt install ./obsidian_amd64.deb
   ```
4. Launch Obsidian from your app drawer, or type `obsidian` in the terminal
5. When prompted, choose **Open folder as vault** and navigate to where you saved this vault folder

### Step 2 — Enable Community Plugins

Obsidian has "safe mode" on by default which blocks third-party plugins. You need to turn it off first:

1. Open **Settings** (gear icon, bottom-left)
2. Click **Community plugins** in the left sidebar
3. Click **Turn on community plugins**
4. Click **OK** to confirm

### Step 3 — Install Execute Code

This plugin adds a **Run** button to Java code blocks so you can execute code right inside your notes.

1. In Settings → Community plugins, click **Browse**
2. Search for **Execute Code**
3. Click the plugin by *timo-weike* (it should be the top result)
4. Click **Install**, then **Enable**
5. Close the plugin browser

### Step 4 — Configure Execute Code for Java

The plugin needs to know where Java is installed on your system.

1. Go to Settings → **Execute Code** (in the left sidebar under "Community plugins")
2. Scroll down to the **Java** section
3. Set the Java path. In your Linux terminal, find it by running:
   ```bash
   which java
   ```
   It will print something like `/usr/bin/java` — paste that path into the Execute Code settings
4. Close Settings

### Step 5 — Test It

Open any note with a `run-java` code block, switch to **Reading view** (`Ctrl+E`), hover over a code block, and click the **Run** button that appears. You should see output appear below the block.

> [!TIP] Reading vs Editing Mode
> - **Editing mode** (`Ctrl+E` to toggle) — for writing your notes and answers
> - **Reading mode** (`Ctrl+E` to toggle) — for reading notes and running code
> Code blocks only show the Run button in **Reading mode**.

---

## 📖 How This Vault Works

- **Read** the notes like a textbook — concepts are explained with examples
- **Run** the embedded code snippets using the Execute Code plugin
- **Answer** the Check for Understanding questions — write your answers right in the file (in Editing mode)
- **Take notes** in the `My Notes/` folder for your own scratch space

---

## 🗺️ Course Topics

| # | Topic | Description |
|---|-------|-------------|
| 00 | [[00 - Getting Started/0.1 Welcome|Getting Started]] | Vault guide & environment setup |
| 01 | [[01 - Java Fundamentals/1.0 Java Fundamentals Index|Java Fundamentals]] | Variables, types, operators, Math class, input |
| 02 | [[02 - Strings/2.0 Strings Index|Strings]] | String methods, comparisons, common traps |
| 03 | [[03 - Objects and Classes/3.0 Objects and Classes Index|Objects & Classes]] | OOP, writing classes, constructors, methods |
| 04 | [[04 - Control Flow/4.0 Control Flow Index|Control Flow]] | Boolean logic, if/else, while, for, nested loops |
| 05 | [[05 - Arrays/5.0 Arrays Index|Arrays]] | 1D arrays, traversal, for-each loops |
| 06 | [[06 - 2D Arrays/6.0 2D Arrays Index|2D Arrays]] | Nested loops, row/column traversal |
| 07 | [[07 - ArrayLists/7.0 ArrayLists Index|ArrayLists]] | ArrayList methods, traversal, wrapper classes |
| 08 | [[08 - Searching and Sorting/8.0 Searching and Sorting Index|Searching & Sorting]] | Linear/binary search, selection/insertion sort |
| 09 | [[09 - Recursion/9.0 Recursion Index|Recursion]] | Tracing recursion, recursive algorithms |
| 10 | [[10 - File IO/10.0 File IO Index|File I/O]] | Scanner, reading data files |
| 11 | [[11 - AP Exam Prep/11.0 AP Exam Prep Index|AP Exam Prep]] | FRQ walkthroughs, exam strategies |

---

## 📋 Quick Reference

- [[11 - AP Exam Prep/11.2 Java Quick Reference|☕ Java Quick Reference Sheet]]
- [[11 - AP Exam Prep/11.1 FRQ Overview|📝 FRQ Types & Strategies]]
- [[11 - AP Exam Prep/11.3 Common Mistakes|⚠️ Common Mistakes]]

---

## ✅ My Progress

Check off topics as you feel confident with them!

- [ ] Java Fundamentals
- [ ] Strings
- [ ] Objects & Classes
- [ ] Wrapper Classes
- [ ] Control Flow
- [ ] Arrays
- [ ] 2D Arrays
- [ ] ArrayLists
- [ ] Searching & Sorting
- [ ] Recursion
- [ ] File I/O
- [ ] AP Exam Prep

---

## 📓 My Notes

[[My Notes/My Notes Home|Head to My Notes →]] for your own scratch space.

---

*AP Computer Science A — 2025-26*
