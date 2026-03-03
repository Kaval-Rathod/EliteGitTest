# Git Collaboration Chain Challenge

## 🔒 Rules (Read Carefully)

- Do NOT push directly to `main`
- Do NOT merge your own Pull Request
- Do NOT rewrite shared history
- Do NOT delete someone else's work
- Keep commits clean and meaningful
- Work independently unless instructed otherwise

⚠️ If you face difficulty, try solving first.  
Only open the hints section if you're truly stuck.

---

# 👤 Person 1 — Foundation Builder

## 🎯 Objective

- Get the latest project version.
- Create a new isolated working branch.
- Add your name inside the `<ul>` list in the HTML file.
- Update the footer version from `1.0` to `1.1`.
- Push your work and open a Pull Request.
- Do NOT merge it yourself.

## 🧪 What Is Being Tested

- Proper branching discipline  
- Clean commit practice  
- Not touching `main` directly  

<details>
<summary>⚠️ Trap</summary>

If you work directly on `main`, you automatically fail.

If your commit message is vague like "update file", you lose points.

</details>

<details>
<summary>💡 Hint (Open Only If Needed)</summary>

You should always start from the latest main branch before creating your feature branch.

</details>

---

# 👤 Person 2 — Parallel Contributor

(Assume Person 1’s PR is merged.)

## 🎯 Objective

- Sync with the latest `main` branch.
- Create your own feature branch.
- Modify the `<h1>` heading text to something new.
- Add one more `<li>` entry in the log section.
- Push and create a Pull Request.

## 🧪 What Is Being Tested

- Pull before branch  
- Working independently  
- Clean integration  

<details>
<summary>⚠️ Trap</summary>

If you forget to sync with main first, your branch may be outdated and create unnecessary conflicts later.

</details>

<details>
<summary>💡 Hint (Open Only If Needed)</summary>

Always make sure your base branch is up to date before creating a new feature branch.

</details>

---

# 👤 Person 3 — Conflict Resolver

(Person 2 is merged before you.)

## 🎯 Objective

- Sync with `main`.
- Create a branch.
- Modify the SAME `<h1>` heading but with different text.
- Push and create a PR.
- After Person 2 is merged, update your branch.
- Resolve the merge conflict properly.
- Keep a meaningful final heading.
- Complete the merge safely.

## 🧪 What Is Being Tested

- Conflict handling  
- Understanding conflict markers  
- Not deleting someone else's work blindly  

<details>
<summary>⚠️ Trap</summary>

If you panic and re-clone the repository instead of resolving the conflict, you fail.

If you delete the other developer’s work without reasoning, you fail.

</details>

<details>
<summary>💡 Hint (Open Only If Needed)</summary>

When a conflict happens, Git will show special markers in the file.  
You must manually decide what the final correct version should be.

</details>

---

# 👤 Person 4 — Mistake Fixer

(A wrong commit changed the footer version to `9.9`.)

## 🎯 Objective

- Correct the version number to `1.2`.
- Do NOT rewrite history.
- Do NOT delete previous commits.
- Fix using a clean new commit.
- Create PR and merge.

## 🧪 What Is Being Tested

- Understanding safe correction  
- Not using destructive history rewriting  
- Respecting shared history  

<details>
<summary>⚠️ Trap</summary>

If you attempt to modify or delete previous commits in shared history, you fail.

</details>

<details>
<summary>💡 Hint (Open Only If Needed)</summary>

In collaborative repositories, corrections are usually done with new commits, not by editing old ones.

</details>

---

# 👤 Person 5 — Production Crisis Scenario

(A `.env` file containing secrets was pushed.)

## 🎯 Objective

- Remove the sensitive file properly.
- Prevent it from being tracked again.
- Explain what must be done about exposed secrets.
- Explain how repository history should be cleaned.
- Explain the risk of force pushing.
- Provide a safe recovery plan.

## 🧪 What Is Being Tested

- Production-level Git understanding  
- Security awareness  
- Crisis handling maturity  

They must clearly explain:

- Credential rotation  
- History rewrite tools  
- Why deleting the file alone is not enough  

<details>
<summary>⚠️ Trap</summary>

If you only delete the file and commit again, you fail.

The secret still exists in Git history.

</details>

<details>
<summary>💡 Hint (Open Only If Needed)</summary>

Removing sensitive data from Git requires cleaning commit history and rotating compromised credentials immediately.

</details>

---

# 🏁 Final Evaluation Criteria

Each participant will be evaluated on:

- Branch discipline  
- Conflict handling  
- Commit clarity  
- Respect for shared history  
- Crisis response thinking  

If the team completes this without chaos, confusion, or unsafe actions —  
they are ready for real collaborative development.

If not, weaknesses are exposed early — which is the purpose of this challenge.
