# Hyunyoung2's sphinx practice for konlp

[![Documentation Status](https://readthedocs.org/projects/hyunyoung2s-sphinx-practice/badge/?version=latest)](http://hyunyoung2s-sphinx-practice.readthedocs.io/en/latest/?badge=latest)

Above all, let's make virtual environment 

> sudo apt install -y python3-venv  
> pyvenv env  
> source env/bin/activate

After it, follow things below.

First, in order to run sphinx, install them below:

> pip install sphinx

Then, Create a directory inside your project to hold your docs: 

> cd /path/to/project
> mdkir docs

So, Run **sphinx-quickstart**

> sphinx-quickstart

This quick start will walk you through creating the basic configuration; When it's done, you'll have **index.rst**, **conf.py** and some other files. 

build your project like this:

> make html

Then check 

> open /path/to/\_\_build/index.html

After that if you want to host on the html files with github page. 

There ars wo simple way like this:

> mv /path/to/\_build/html/* /path/to/your_git_repository/  

Then push your local repository to your remote repository. 

**Keep in mind, you should add \.nojekyll in remote repository for github page to render your html generated on python code.**

The following is screencast of how to utilize sphinx : 


[![](/img/Image/NaturalLanguageProcessing/NLPLabs/Konltk_NLP/2018-05-06-How_TO_Use_Sphinx_For_documentation/sphinx_image.png)](https://www.youtube.com/embed/oJsUvBQyHBs)

### add a \.nojekyll file

The last thing you have to do is add an empty file called **\.nojekyll** in your repository. This te


# Reference 

 - [Readthedocs's getting started](https://docs.readthedocs.io/en/latest/getting_started.html) 
 - [sphindoc-test v0.1 documentation](https://daler.github.io/sphinxdoc-test/includeme.html)
