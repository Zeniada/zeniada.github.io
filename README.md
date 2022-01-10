# zeniada
Zeniada is an intercollegiate poetry/art magazine based at Johns Hopkins
University. This repository is for its website, which was last
re-designed on 2020 May 13
with simplicity and minimal upkeep in mind.

## favicon
Favicons were generated using [favicon.io](https://favicon.io/favicon-generator/)
(color `#181913`, background `#fffff71`) and can be found under the `img`
folder.

## adding a new zeniada issue
### setup
First, make sure you have the repository [cloned](https://help.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository#cloning-a-repository-using-the-command-line)
on your computer. (This gives you a copy of the repository, so you can
edit existing files and add new files accordingly.)

### adding files
The minimal items needed to add a Zeniada issue:
1. A thumbnail preview (typically the cover of the issue, ratio 5:8).
Add this to the `thumbnails` folder.
2. A pdf version of the issue. Add this to the `issues` folder.

### adding a section
To add the Zeniada issue, open `index.html` and add a new `div class='issue'`
under the `Issues` section (currently starting on line 34).

Here's what that would look like for Spring 2020 (with a thumbnail
named `sp20.jpg` and a pdf named `ZENIADA-sp20.pdf`):
```
<div class="issue">
    <img class="thumbnail" src="thumbnails/sp20.pdf"/>
    <h3>Spring 2020</h3>
    <a class="link" href="issues/ZENIADA-sp20.pdf" target="_blank">read</a>
    <span class="link link-disabled">buy</span>
</div>
```

Feel free to copy/paste existing issue divs, then change file names
and edit links necessary.

### saving/pushing changes
To check on your progress, use `git status`.
This will show you everything you've added/edited.

To add all your changes, use `git add -A`.

Next, commit them with a helpful commit message in the quotes
(example below for adding the Spring 2020 issue):
```
git commit -m "Add Spring 2020 issue"
```

Finally:
```
git push origin main
```

All done!
