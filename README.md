# zeniada
Zeniada is an intercollegiate poetry/art magazine based at Johns Hopkins
University. This repository is for its website, which was last
re-designed on 2020 May 13 with simplicity and minimal upkeep in mind.

## favicon
Favicons were generated using [favicon.io](https://favicon.io/favicon-generator/)
(color `#181913`, background `#fffff71`) and can be found under the `img`
folder.

## adding a new zeniada issue
### adding files
The minimal items needed to add a Zeniada issue:
1. A thumbnail preview (typically the cover of the issue, ratio 5:8).
2. A pdf version of the issue

#### adding the thumbnail
To add your thumbnail to `thumbnails`, navigate to
[the folder](https://github.com/Zeniada/zeniada.github.io/tree/main/thumbnails)
and use the `Upload files` option to upload your image.

![readme-add-thumbnail](https://user-images.githubusercontent.com/21047909/150021352-6f811d70-1cfa-4589-b3f6-d3084d2359cc.jpg)

Then, at the bottom of the page, write a helpful commit message
and click `Commit changes`.

![readme-commit-thumbnail](https://user-images.githubusercontent.com/21047909/150021680-a93a9eac-9d84-4117-95af-c2aa5f217ea0.jpg)

#### adding the pdf
Using the same steps as above, upload your pdf
to the `issues` folder.

### update the home page
To link the new Zeniada issue on the home page, open `index.html`
and click the `Edit this file` option (top right).

![readme-edit-file](https://user-images.githubusercontent.com/21047909/150021959-9d156d2d-24fc-4e61-9d1d-a7a97a032b03.jpg)

Add a new `div class='issue'` under the `Issues` section
(currently starting on line 34).

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
and edit links as necessary.

Finally, at the bottom, add a helpful message and commit your changes (see above).
