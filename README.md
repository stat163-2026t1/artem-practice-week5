# STAT163 — Practice 5: tidy data from two publishers

One notebook across your two practice sessions. The Task cells carry the grade.

## Get your own copy

Open the course hub, https://classroom-hub.oleh-omelchenko.workers.dev, sign in with
GitHub, and click **Accept** next to *week5-practice*. You get your own private copy and
its address.

Then clone it:

```bash
git clone <your-repository-url>
cd <repository-folder>
```

Because the copy is private, Git has to know who you are before it will hand the files
over. If `git clone` asks for a password and then fails, that is what is missing. Set it
up once, either way:

- [GitHub CLI](https://cli.github.com): install `gh`, then run `gh auth login`.
- [SSH keys](https://docs.github.com/en/authentication/connecting-to-github-with-ssh).

## Set up and run

You need [`uv`](https://docs.astral.sh/uv/) and Git installed.

```bash
uv sync              # creates .venv/ with the packages the notebook needs
uv run jupyter lab   # opens the notebook environment in your browser
```

If `uv sync` fails with `operation timed out`: the university Wi-Fi blocks a part of the
PyPI file server. The fix (a one-minute DNS change) is in the
[setup check README](https://github.com/stat163-2026t1/week1-setup-check#if-uv-sync-fails-with-a-timeout).

Then open `practice.ipynb` and work top to bottom.

**One thing the self-check does not do:** it never compares your answer with ours, so a ✅
does not mean the number is right.

## The data

Two files in `data/`: the population of every country from the World Bank, and the
unemployment rate in Europe from Eurostat. `data/README.md` names the sources and the
licences.

## Submit

Restart and re-run the whole notebook, check every cell runs, save, then commit and push:

```bash
git add -A
git commit -m "practice 5"
git push
```

Then paste your repository URL into the Week 5 practice assignment on Moodle. The deadline
is shown on the assignment.
