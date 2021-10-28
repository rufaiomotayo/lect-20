# Lecture 20 Activity: Pull Request + Code Review
In this activity, you'll be practicing making a pull request, and then reviewing that same pull request (normally, a teammate would do that for you).

Note that ALL of this can be done locally, since you won't actually be running any code.

1) Copy down the materials (`app.py` and `index.html`) into a new folder in your development environment. Your directory structure should look like:
```
lect20_activity/
  base.py
  app.py
  templates/
    index.html
```

2) Now, in the `lect20_activity/` folder (or whatever you named it), run `git init`.
3) `base.py` is a placeholder file that just exists so we can create a dummy "main" branch before doing our feature work. Run the following:
```
git add base.py
git commit -m "main branch commit"
git branch -m main
```
4) Create a public GitHub repository and push your main branch to that repository.
5) Now commit the rest of your files to a "feature" branch:
```
git checkout -b feature
git add --all
git commit -m "feature commit"
git push origin feature
```
6) If you go to your GitHub repo now, you should have the option to create a Pull Request from `feature` to `main`. Do that, and add whatever comment you want to the Pull Request (this is fair game for the code review you're about to do).
7) If you click on the "Files Changed" tab on the new Pull Request page, you'll be taken to all the code changes in the Pull Request. Here, if you click on a line number, you'll be able to leave a comment (and the first time you do that, there will be a "Start Review" option). Use this view to do a code review of the code you just pushed. Remember to look for high-level, mid-level, AND low-level concerns.
8) Leave a link to your reviewed Pull Request in the Discord to receive participation credit.