# PyData NYC 2017

This is all the material for my talk titled "R for Pythonistas" for PyData NYC 2017.

## Setup

To setup and run the notebook(s) and slides, you'll first need to create your virtual environment. I used Anaconda to create my environment and I've included my environment.yml file in this repository. Even if you're relatively comfortable with Anaconda/conda environments, I would still recommend that you read my post on [Setting up a Working R Environment][r-environment] first before creating your environment since there are a few tricks to getting the setup just right for R development.

## Viewing the Slides

To view the slides, you'll need to make sure you have a copy of the [reveal.js][revealjs] presentation framework on your local system. I have added the version of reveal.js that I used in my presentation as a submodule of this repository. So, to get everything you need, you can simply update this repo's submodules.

```
$ git submodule update --init --recursive
```

Once you have your environment set up and a local copy of reveal.js downloaded, you can view the slides by running the `jupyter nbconvert` command.

```
$ jupyter nbconvert --config nbconvert_offline_slides.py
```

This command will convert the `Talk.ipynb` notebook into an HTML file that can be viewed as a [slideshow presentation][jupyter-slides]. The resultant HTML file will be saved to `./slides/pydata_nyc_2017.slides.html`. To view the slides, simply open the newly created file in a browser of your choosing.


[r-environment]: http://christopherroach.com/articles/r-environment/
[revealjs]: http://lab.hakim.se/reveal-js/
[jupyter-slides]: https://medium.com/@mjspeck/presenting-code-using-jupyter-notebook-slides-a8a3c3b59d67
