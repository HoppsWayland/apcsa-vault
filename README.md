# AP Computer Science A — Course Vault

An interactive reference and student notebook for AP CSA, built with [Obsidian](https://obsidian.md) and published as a website using [Quartz 4](https://quartz.jzhao.xyz).

---

## 🌐 Website

The published website lives at: `https://YOUR-USERNAME.github.io/REPO-NAME`

It updates automatically every time a push is made to `main`.

---

## 📓 Student Notebook (Obsidian)

Students download the vault once at the start of the year (or per unit) and open it in Obsidian on their local machine. The vault contains:

- Explanations with runnable Java code examples (via the Execute Code plugin)
- Guided questions with space to write answers directly in the notes
- A tagging system for cross-topic review (`#gotcha`, `#pattern`, `#algorithm`, etc.)
- A progress checklist on the Home page

### Setting Up the Student Vault

1. Download this repository as a ZIP (green **Code** button → **Download ZIP**)
2. Unzip it — you'll find a `vault/` folder inside
3. Open Obsidian → **Open folder as vault** → select the `vault/` folder
4. Follow the setup instructions in `vault/Home.md` to install the Execute Code plugin

---

## 🛠 Repository Structure

```
/
├── vault/                  ← Obsidian vault (student content)
│   ├── Home.md
│   ├── 01 - Java Fundamentals/
│   ├── 02 - Strings/
│   ├── 03 - Objects and Classes/
│   ├── 04 - Control Flow/
│   ├── 05 - Arrays/
│   ├── 06 - 2D Arrays/
│   ├── 07 - ArrayLists/
│   ├── 08 - Searching and Sorting/
│   ├── 09 - Recursion/
│   ├── 10 - File IO/
│   ├── 11 - AP Exam Prep/
│   └── My Notes/
├── content/                ← Quartz reads from here (symlink or copy of vault/)
├── quartz.config.ts        ← Quartz site configuration
├── .github/
│   └── workflows/
│       └── deploy.yml      ← Auto-deploy to GitHub Pages on push
└── README.md
```

---

## ⚙️ First-Time Quartz Setup

This only needs to be done once when setting up the repo.

### Prerequisites
- Node.js v22+
- Git

### Steps

**1. Clone the Quartz base repo and set up your content:**

```bash
git clone https://github.com/jackyzha0/quartz.git
cd quartz
npm install
```

**2. Replace `quartz.config.ts`** with the one from this repo.

**3. Point Quartz at the vault:**

Quartz reads from a `content/` folder. The simplest approach is to symlink:

```bash
# From the repo root
ln -s vault content
```

Or on Windows, copy the vault folder to `content/`.

**4. Update `baseUrl` in `quartz.config.ts`:**

```typescript
baseUrl: "your-username.github.io/your-repo-name",
```

**5. Test locally:**

```bash
npx quartz build --serve
# Visit http://localhost:8080
```

**6. Commit and push:**

```bash
git add .
git commit -m "Initial Quartz setup"
git push origin main
```

**7. Enable GitHub Pages:**

- Go to your repo → **Settings** → **Pages**
- Under **Source**, select **GitHub Actions**
- The next push will trigger a build and deploy

Your site will be live at `https://your-username.github.io/your-repo-name` within a few minutes.

---

## 📝 Updating Content

Normal workflow after initial setup:

```bash
# Edit notes in Obsidian as usual, then:
git add .
git commit -m "Update: added examples to 5.4 Arrays of Objects"
git push
# Site rebuilds automatically — usually live within 2 minutes
```

You can watch the build progress in the **Actions** tab of your GitHub repo.

---

## 🏷 Tag System

Notes use a consistent tagging system for cross-topic review:

| Tag | Meaning |
|-----|---------|
| `#gotcha` | Common mistakes and traps |
| `#pattern` | Reusable code idioms |
| `#algorithm` | Named computational approaches |
| `#concept` | Definitional / conceptual bullets |
| `#syntax` | Pure Java syntax reminders |
| `#mc_only` | MCQ only — tracing required, not writing |
| `#static` | Static methods and class variables |

Topic tags: `#variables` `#strings` `#operators` `#math-class` `#scanner` `#objects` `#classes` `#constructors` `#methods` `#booleans` `#conditionals` `#loops` `#arrays` `#2d-arrays` `#arraylists` `#searching` `#sorting` `#recursion` `#file-io`

Narrowing tags: `#for` `#while` `#nested`

---

## 📄 License

Content is for classroom use. Java code examples are free to use and adapt.
