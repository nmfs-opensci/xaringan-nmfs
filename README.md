:spiral_calendar: January 25, 2022 

# xaringan NMFS templates

### To use

Open one of the template Rmd files in the `docs` folder and save. Then edit with your material. Click knit to make the presentation. Note, the css files need to be in the same folder as your Rmd file; as the repo is set up, this means the css needs to be in the `docs` folder.

To host on GitHub, go to settings in your GH repo and turn on GitHub Pages (scroll to bottom). Select the main branch, root folder, and click save. Save the url that it tells you. The url to your slideshow will be something like `yourname.github.io/xaringan-nmfs/docs/slides.html`. Alternatively, you could select the `docs` folder and the url would be `yourname.github.io/xaringan-nmfs/slides.html` but you'd need to add a README.md to `docs` if you want `yourname.github.io/xaringan-nmfs` to be something otherthan a dummy page (which GitHub Pages makes for you).

**packages:** {xaringan}, {xaringanthemes}, [{xaringanExtra}](devtools::install_github("gadenbuie/xaringanExtra"))

### [`template.Rmd`](docs/template.Rmd)

This is a basic presentation. [Slides](https://nmfs-opensci.github.io/xaringan-nmfs/docs/template.html)

* The css used is at the top
* `slideNumberFormat:` specifies how to show the slide number
* See the slides for examples of different slide formats

### [`template-extra.Rmd`](docs/template-extra.Rmd)

This has a variety of extra bells and whistles. [Slides](https://nmfs-opensci.github.io/xaringan-nmfs/docs/template-extra.html)

* A progress bar at top
* A right side bar
* Special formating of sidebar text
* Boxes with text
* 3 and 4 column formats

### [`template-tufte.Rmd`](docs/template-tufte.Rmd)

This is a Tufte presentation. [Slides](https://nmfs-opensci.github.io/xaringan-nmfs/docs/template-tufte.html)

* Uses the Tufte style fonts
* Uses the Tufte line spacings and header styles
* Has a progress bar at the top

### Adapting

The files you need are in the `docs` folder. You need the `static` folder which has the background images. Then you need all the css files not in folders; probably cleaner to move those to a `css` folder... Lastly you need an Rmd template.

Once you have those things, you can edit the Rmd files for your presentation. To change the look, edit the css files or add new ones. See the `theme` folder for the `xaringan_template.Rmd` that has the code that produces `xaringan-themer.css`. Use that code to create the base css file which specs things like font and color. The `assets` and `libs` folders will be created by {xaringan} when you knit your presentation.

## Sharing your presentation

You need to enable GitHub Pages on your repo. Once you do that, the format of the URL you'll share will look something like
```
https://nmfs-opensci.github.io/xaringan-nmfs/docs/template-tufte.html
```
except of course the part in front of `github.io` will be your username and the `xaringan-nmfs` will be replaced with your repo name.

<hr>

This repo and the NMFS xargingan theme was adapted from [nmfs-fish-tools/presentations](https://github.com/nmfs-fish-tools/presentations) made by [Christine Stawitz](https://github.com/ChristineStawitz-NOAA). The Tufte fonts and css are from [tufte-css](https://github.com/edwardtufte/tufte-css). `slide-style.css` is adapted from An RStudio workshop on data science [design-ds-classroom](https://github.com/rstudio-conf-2020/design-ds-classroom) by [Mine Cetinkaya-Rundel](https://github.com/mine-cetinkaya-rundel). Slides created via the R package [{xaringan}](https://github.com/yihui/xaringan) and [{xaringanthemer}](https://pkg.garrickadenbuie.com/xaringanthemer/articles/xaringanthemer.html).
