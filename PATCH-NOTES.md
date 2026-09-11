# What changed in this patch

1. `.github/workflows/snake.yml` — NEW. Generates an animated contribution
   snake and pushes it to an `output` branch, same pattern already working
   on jxjwilliam/jxjwilliam.
2. `README.md` — the "GitHub Analytics" section's broken
   `github-readme-activity-graph.vercel.app` image (503 / paused as of
   Sep 2026) is replaced with the self-hosted snake graph. The Followers /
   Total Stars / Status badges above it were already shields.io-based and
   are untouched — they were never broken.

# How to apply

cd williamjxj              # your local clone of williamjxj/williamjxj
# copy README.md and .github/workflows/snake.yml from this patch over your local files
git add README.md .github/workflows/snake.yml
git commit -m "fix: replace paused activity-graph widget with self-hosted snake graph"
git push

Then, same as for jxjwilliam:
- Settings → Actions → General → Workflow permissions → "Read and write permissions" → Save
- Actions tab → "Generate contribution snake" → Run workflow (first run, to create the output branch)
