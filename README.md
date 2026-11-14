# new-project

## Step-by-step instructions

```bash
mkdir new-project && cd new-project
git init                                   # steps 1–3
echo "# new-project" > README.md           # step 4
git add README.md                          # step 5
git commit -m "init"                       # step 6
git checkout -b development                # step 7 (or git switch -c development)
# add step-by-step instructions to README.md (these same commands)
git add README.md                          # step 8
git commit -m "PROM-42164 #comment Add step-by-step instructions to README"   # step 9, Smart Commit
git checkout main && git merge development # step 10
git status                                 # step 11
# create a PUBLIC GitHub repository new-project, then:
gh repo create new-project --public --source=. --remote=origin
git push -u origin main development        # step 12 / publish
```
