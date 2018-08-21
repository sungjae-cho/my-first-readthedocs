# My first readthedocs practice

# How to start my readthedocs page on the internet.
1. Make a repository in your GitHub account.
2. Clone your repository to your local directory.
3. Make a directory named `docs` and change the directory the working directory.
4. Install `sphinx`.
5. With the `sphinx-quickstart` command, generate the default files and dicrectories.
6. Edit some files with initial settings.
7. Push the updated repository to GitHub.
8. Publish the documentation website in the [readthedocs.org](https://readthedocs.org/) page.

Make a repository in your GitHub account. In my case, the repository is [https://github.com/sungjae-cho/my-readthedocs](https://github.com/sungjae-cho/my-readthedocs).

Then, clone the repository in your working directory.
```bash
$ git clone https://github.com/sungjae-cho/my-readthedocs
```

Then, move to the `my-readthedocs` directory.
```bash
$ cd my-readthedocs
```

Make a directory named `docs` and change the directory the working directory.
```bash
$ mkdir docs
$ cd docs
```

Install `sphinx`.
```bash
$ sudo pip install sphinx sphinx-autobuild
```

With the `sphinx-quickstart` command, generate the default files and dicrectories.
```bash
$ sphinx-quickstart
```
Select the default choices except 
* separating build and source directories and 
* automatically adding doc strings.
And,
* Just type your project name on `Project name`.
* Just type your name on `Author`.

Move to the `source` directory.
```bash
$ cd source
$ ls
```
Then, you can see `conf.py` and `index.rst`.
* `conf.py`: A python file to set the configurations of the documentation.
* `index.rst`: a rst file of the homepage of the documnetation. You should know the rst syntax to edit this file.

To change the theme as you like, edit `html_theme` like `html_theme = "sphinx_rtd_theme"`. You can find the string of a particular theme in its official website. In my case, I found the string [here](https://sphinx-rtd-theme.readthedocs.io/en/latest/installing.html).

Then, push all the changes into the remote repository in GitHub.
```bash
$ cd ../..
$ git add .
$ git commit -a -m "Initial commit."
$ git push origin master
```

Then, you can find the update repository in your GitHub page. In my case, the respository is [https://github.com/sungjae-cho/my-readthedocs](https://github.com/sungjae-cho/my-readthedocs).

The next step is to publish the documentation website through [readthedocs.org](https://readthedocs.org/). Just follow [this vide](https://www.youtube.com/watch?v=4rAoOcxQKoYo). After getting throught all the instructions, you will get your own documentation page! This is [my first readthedocs documnetaiotn website](https://my-first-readthedocs.readthedocs.io)! 
