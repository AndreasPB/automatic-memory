---
title: Git
theme: blood  # beige, black, blood, league, moon, night, serif, simple, sky, solarized, white
highlightTheme: nord  # https://github.com/highlightjs/highlight.js/tree/main/src/styles
revealOptions:
  transition: none
---
<!-- .slide: data-background-color="#4287f5" -->

# Git

### ☁️ 👉😎👉☁️

---

### What is Git?
<!-- .slide: data-background="https://media.giphy.com/media/ZaJtnTY8tFZz0PvmW9/giphy.gif" data-background-opacity="0.7" -->
- version control
- show useful commands when working together using git
- no so much theory, but more practical usage of git

---

### Commands

A quick overview of some commands:

```bash
git pull    # from remote to local
git push    # to remote from local
git add     # stage changes to a commit
git commit  # commit staged changes
git rebase  # rebase commits
git reset   # reset HEAD
git reflog  # view your git history
```

---

### Git history 📜

---

### Create/fork a repo
```bash
git init (smth?? kan ikke huske)
```
or use [GitHub](https://github.com/)

---


### Clone a repo

Clone the repository using https or ssh

```bash
# SSH
git clone git@github.com:<username>/<repository>.git

# HTTPS
git clone https://github.com/<username>/<repository>.git
```

---

### Merge < Rebase 💢

Keep a maintainable commit history

```bash
git rebase development
```

<!-- > ![](https://www.bitsnbites.eu/wp-content/uploads/2015/12/1-nonlinear-vs-linear.png) -->
> <img src="https://www.bitsnbites.eu/wp-content/uploads/2015/12/1-nonlinear-vs-linear.png" alt="linear vs. non-linear" width="400"/>

---

### Write some awesome code

<!-- .slide: data-background="https://c.tenor.com/z4_HKSF6Nx8AAAAC/typing-jim-carrey.gif" data-background-opacity="0.4" -->

---

### Diff 🥐

*look at the improvements*

```bash
git diff
```

```diff
-const someList = [1, '2', 3, '4']
-for (x of something) {
-    console.log('how to javskript?', x)
-}
+some_list = [1, '2', 3, '4']
+for x in something:
+    print('python > javascript', x)
```
<!-- .slide: data-background="https://c.tenor.com/OWrqUWuNRHEAAAAC/thumbs-up-internet.gif" data-background-opacity="0.4" -->
<!-- 

---

### Puuush

Push your new changes to the remote

```bash
git push origin <branch-name>
```

---

### Pull

Get new remote changes to your machine

```bash
git pull
```

<!-- .slide: data-background="https://c.tenor.com/6iq8JGtbYZ8AAAAd/cat-drag.gif" data-background-opacity="0.4" -->
---

### Conflict 

```diff
<<<<<<< HEAD
const someList = [1, '2', 3, '4']
for (x of something) {
    console.log('how to javskript?', x)
}
=======
some_list = [1, '2', 3, '4']
for x in something:
    print('python > javascript', x)
>>>>>>> Incomming
```

---


### Reflog 📓
```bash
git reflog
```
Good for CTRL - Z when you messed up locally.
---

### Assignment 👷
Linear history (to and from master)  
15 minutes

1. Create a repository from template
2. Clone the repository
3. Push and pull changes
4. Edit the same lines (create a conflict)
5. Solve conflict

---

### Assignment 2 👷
Semi-linear (using feature branches)  
15 minutes

1. Create a feature branch
2. Push feature
3. Review and merge feature
