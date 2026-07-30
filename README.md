<div align="center">

<!-- Banner -->
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1a1a2e,50:16213e,100:0f3460&height=200&section=header&text=📖%20Word%20a%20Day&fontSize=52&fontColor=e0e0ff&fontAlignY=38&desc=Building%20vocabulary%20one%20commit%20at%20a%20time&descAlignY=58&descSize=18&descColor=a0a8d0" width="100%"/>

<!-- Badges -->
<br/>

![GitHub Actions](https://img.shields.io/badge/Powered%20by-GitHub%20Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)
![Free](https://img.shields.io/badge/100%25-Free-22c55e?style=for-the-badge)
![Daily](https://img.shields.io/badge/Runs-Every%20Day-f59e0b?style=for-the-badge&logo=clockify&logoColor=white)
![Contributions](https://img.shields.io/badge/Keeps-Streak%20Alive-e879f9?style=for-the-badge&logo=github&logoColor=white)

<br/>
<br/>

> *A new English word every single day — automatically fetched, defined, and committed via GitHub Actions.*
> *Learn something. Keep the streak. Repeat.*

<br/>

</div>

---

## 🌟 What is this?

**word-a-day** is a fully automated GitHub repository that:

- 🤖 **Runs every day at 6:00 AM UTC** using a GitHub Actions workflow
- 📖 **Fetches a new English word** from a free public dictionary API
- 💾 **Commits it to this repo** so it shows as a green square on your GitHub contribution graph
- 🧠 **Teaches you something new** every single day — completely passively

No manual work. No cost. Just open GitHub the next day and you've already learned a new word.

---

## 📋 What each entry includes

Every daily entry saved in [`WORD-OF-THE-DAY.md`](./WORD-OF-THE-DAY.md) contains:

| Field | Example |
|---|---|
| 📅 **Date** | `2025-07-30` |
| 📖 **Word** | `ephemeral` |
| 🔊 **Pronunciation** | `/ɪˈfem.ər.əl/` |
| 🏷️ **Type** | `adjective` |
| 📝 **Definition** | Lasting for a very short time |
| 💬 **Example sentence** | *"The ephemeral nature of social media trends surprises no one."* |

---

## 🗂️ Repo Structure

```
word-a-day/
│
├── 📁 .github/
│   └── 📁 workflows/
│       └── 📄 word-of-the-day.yml   ← The automation magic
│
├── 📄 WORD-OF-THE-DAY.md            ← All words logged here daily
└── 📄 README.md                     ← You are here
```

---

## ⚙️ How it works

```
Every day at 6 AM UTC
        │
        ▼
┌──────────────────────┐
│  GitHub Actions      │
│  workflow triggers   │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│  Fetches a random    │
│  word from free API  │
│  (dictionaryapi.dev) │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│  Parses: word, type, │
│  pronunciation,      │
│  definition, example │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│  Appends entry to    │
│  WORD-OF-THE-DAY.md  │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│  git commit & push   │
│  → 🟩 Contribution!  │
└──────────────────────┘
```

---

## 🚀 Set it up yourself (3 steps)

Want to run this on your own profile? It's completely free.

**Step 1 — Fork or clone this repo**

```bash
git clone https://github.com/vishal-git-dot/word-a-day.git
cd word-a-day
```

**Step 2 — Update the workflow with your details**

Open `.github/workflows/word-of-the-day.yml` and replace:

```yaml
git config user.name "your-github-username"
git config user.email "your-noreply@users.noreply.github.com"
```

> 💡 Find your no-reply email at **GitHub → Settings → Emails**
> It looks like: `123456789+username@users.noreply.github.com`

**Step 3 — Enable workflow permissions**

Go to your repo → **Settings** → **Actions** → **General** → scroll to **Workflow permissions** → select **Read and write permissions** → **Save**

That's it. The workflow runs automatically from the next scheduled time. ✅

---

## 🆓 APIs used (all free, no key needed)

| API | Purpose |
|---|---|
| [random-word-api.herokuapp.com](https://random-word-api.herokuapp.com) | Picks a random English word |
| [dictionaryapi.dev](https://dictionaryapi.dev) | Fetches definition, pronunciation, type & example |

Both are completely free with no signup or API key required.

---

## 🟩 Does this count as a GitHub contribution?

**Yes** — as long as:

- ✅ The repo is **public** (or private contributions are enabled on your profile)
- ✅ Commits are pushed to the **default branch** (`main`)
- ✅ The commit email **matches your GitHub account email**

Each daily commit = one green square on your contribution graph.

---

## 📖 Sample entry

```markdown
---
### 📅 2025-07-30
## 📖 serendipity
- 🔊 Pronunciation: /ˌser.ənˈdɪp.ɪ.ti/
- 🏷️ Type: noun
- 📝 Definition: The occurrence of events by chance in a happy or beneficial way
- 💬 Example: *"The serendipity of finding that book changed her entire career."*
```

---

## 📜 License

This project is open source and free to use, fork, and modify.

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f3460,50:16213e,100:1a1a2e&height=100&section=footer" width="100%"/>

*Made with ❤️ by [vishal-git-dot](https://github.com/vishal-git-dot) · Automated with GitHub Actions*

</div>
