# Condon Research Group Docs
This is a repository for holding all things documentation that might be helpful. It has been created using [mkdocs](https://www.mkdocs.org).

## Contributing
To contribute first you need to be added to the repo. Reach out to [Laura](https://github.com/lecondon) to be added. 

--- 
## First Time Setup 
**Step 1** - Clone and install

Clone this repo
`git clone git@github.com:condon-lab/Condon_Lab_Docs.git`

Then you'll need to install the `mkdocs` package by running 
`pip install mkdocs`

**Step 2** - Create a new branch 

Checkout a new branch where you can add/edit docs
`git checkout -b <branch-name>`

Then edit docs to your heart's content!

---
## Routine Updates

**Step 1** - Sync with main

To update your local repo with any changes on `main` since your last work, run the following: </br>
`git checkout main` </br>
`git fetch origin` </br>
`git reset --hard origin/main`</br>

This ensures your local `main` matches the remote exactly, a clean slate to start from. 

**Step 2** - Create/update your branch 

Create new branch </br>
`git checkout -b <branch-name>`

Or update existing brach </br>
`git checkout <existing-branch>`

Then edit docs as needed. 

--- 
If you prefer to write documentation using google docs, you can convert a google doc to a markdown file easily using [this chrome extension](https://workspace.google.com/marketplace/app/docs_to_markdown/700168918607).
Additionally, [here are some helpful markdown tips and tricks](https://www.markdownguide.org/cheat-sheet/).

If you want to add an image to your documentation simply add the image you want to the `./images` directory and then reference the image using the relative path. e.g.
```
[alt text for your image](../../images/my_image.png)
```
If you remove an image from an existing doc, please remove the image file also. 

You can then run `mkdocs serve` to see a local version of your new and updated docs in you browse at `http://127.0.0.1:8000/`

When everything looks good open a pull request to `main` and either ping in slack or assign [Laura](https://github.com/lecondon) to review.

After your PR has been appoved, merge it in and go check out your new docs over at [https://condon-lab.github.io/Condon_Lab_Docs/](https://condon-lab.github.io/Condon_Lab_Docs/).