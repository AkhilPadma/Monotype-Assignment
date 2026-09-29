# NORVIA Logo Tampering Detection

Take-home submission for Monotype Solutions India — Research Engineer (CV).

See `Learnings_documentation.docx` for the write-up.

## Files

```
norvia_notebook.ipynb          # Full pipeline
Learnings_documentation.docx   # Write-up
requirements.txt
README.md
data/uploads/images/           # 001.jpg … 050.jpg ( remove 5,13,16,17)
data/uploads/reference/        # ref_1.jpg, ref_2.jpg (remove ref3)
```

## Setup

```bash
python -m venv .venv
source .venv/bin/activate       # Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

Python 3.10+. GPU recommended (~15 min vs ~45 min on CPU).

## Run

```bash
jupyter notebook norvia_notebook.ipynb
```

**Cell → Run All.** First run downloads ~3 GB of models; cached after.

Final ranking: `outputs/scores/real_ranked.csv`.

---

Akhil — Sep 2026
