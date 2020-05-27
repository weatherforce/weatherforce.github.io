# WeatherForce Tech blog

## How to edit this blog

Clone the repository and `cd` to your clone:

    $ git clone --recursive git@github.com:weatherforce/weatherforce.github.io.git
    $ cd weatherforce.github.io

Make sure you have [Anaconda](https://anaconda.org/) installed and create a conda env:

    $ conda env create --name blog --file environment.yml

Activate the conda environment:

    $ conda activate blog

Start a development server:

    $ make devserver

Optionnaly, if the port is already in use, you may specify a PORT environment variable:

    $ PORT=7000 make devserver

Now add content files in the `content` directory. You may add Jupyter notebooks ending in
`.ipynb` or Markdown files ending in `.md`.  Along with each notebook, you'll
have to create `.ipynb-meta`. See [pelican-ipynb](https://github.com/danielfrg/pelican-ipynb) for more info.

Your changes should be detected automatically in most cases but you may also force rendering of the site with:

    $ make html

Once your happy with the results, you may publish to the live site:

    $ make publish

## More information

* [Pelican documentation](http://docs.getpelican.com/)
* [pelican-ipynb](https://github.com/danielfrg/pelican-ipynb)
* [Jupyter](http://jupyter.org)
