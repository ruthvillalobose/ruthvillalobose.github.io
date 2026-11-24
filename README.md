# ruthvillalobose.github.io

Personal portfolio of Ruth Villalobos, Data Scientist, AI Engineer & Technical Writer.

Live at **https://ruthvillalobose.github.io**

| Page | File to edit |
|---|---|
| Home | `index.html` |
| Projects | one Markdown file per project in `_projects/` (images in `assets/projects/`) |
| Notes | one Markdown file per note in `_posts/` |

## Add a study note

Create `_posts/YYYY-MM-DD-short-title.md`:

```markdown
---
layout: note
title: My note title
description: One-line summary shown in the list
tags: [statistics, python]
---

Write your note here in Markdown.
```

Then publish:

```
git add -A && git commit -m "New note" && git push
```

It appears at https://ruthvillalobose.github.io/notes/ about a minute later.

## Add or fill in a project

Each project is a file in `_projects/`, for example `_projects/churn-model.md`:

```markdown
---
title: Churn Prediction Model
order: 1                # position in the list
category: Data Science   # Data Science, Data Analysis or Documentation
description: One-line summary   # optional
tags: [Python, XGBoost]         # optional
code: https://github.com/ruthvillalobose/churn-model   # optional
---

Explain the project here in Markdown.

![Feature importance](/assets/projects/churn-feature-importance.png)

```python
model.fit(X_train, y_train)
```
```

A project with no text below the `---` shows in the list as **In progress**
(not clickable). As soon as you add text, it becomes a clickable page.
Save charts (e.g. `plt.savefig(...)` from matplotlib) into `assets/projects/`.
