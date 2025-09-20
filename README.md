# Minimal Light Academic Theme

[![LICENSE](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](https://github.com/harryrichman/minimal-light-academic/blob/main/LICENSE)

This is an academic website template.

\[[Demo the theme](https://harryrichman.github.io/minimal-light-academic/)\]  
 
*This is the source code of my homepage. I build this website based on [minimal](https://github.com/orderedlist/minimal).*
<br>


**Features**:  
- Simple and elegant personal homepage theme
- Jekyll theme, automatically deployed by GitHub Pages
- Basic search engine optimization
- Mobile friendly
- Supporting Markdown 
- Supporting dark mode

## Step-by-step instructions

### 1. Make a copy of this repository in your github account

Known as "forking" the repository.

See instructions from GitHub [here](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo#forking-a-repository).
Just follow steps 1.-7. there.
You can ignore everything from "Cloning your forked repository" and afterwards.

Then, do the following steps to the files in *your* version of the repository.

### 1.1. Make your copy viewable online

The easiest way is to publish it as your GitHub Pages website.

See [instructions here](https://docs.github.com/en/pages/quickstart).

There are additional options if you have purchased your own domain name, or have access to a domain name through your school / department / institution.

Once you have finished this step, your website is *publically* viewable by *anyone on the internet*!
Yay! 
Also, this means you need to finish the rest of these steps ASAP to make the website accurate and presentable.

### 2. Edit the `_config.yml` file

This contains basic data such as your name, institution, and some contact info.

Add a photo to the folder `assets/img/` directory.

### 3. Edit the `index.md` file

This contains the main content of your website, other than the publications and notes.
These are handled separately by a "fancier" process (by default).

Decide which sections you want to keep, which you want to delete, and which you want to reorder.
You can add new sections too, if desired.

Optionally, you could choose to write everything in the `index.md` file, but the tradeoff is you lose some built-in features.

### 4. Edit the `publications.yml` file

This contains the data of your publications.

Some data may require you to add files to the `assets/files/` directory.
If you want to include thumbnails next to your publications, include these in the `assets/img/` directory.

### 5. Edit the `notes.yml` file

This contains the data of your expository notes, presentation slides, posters, etc.

Some data may require you to add files to the `assets/files/` directory.

### 6. Decide on other optional configuration parameters

???

To modify the appearance of the website, edit `_layouts/homepage.html` and / or `_sass/minimal-light.scss`.

To modify the appearance of the publications and notes, edit the `_includes/publications.html` and `_includes/notes.html` files, respectively.



## Project Architecture

```
.
├── _data                    
|   └── publications.yml                      # the data for your publications
├── _includes                    
|   ├── publications.html                     # the formatting for publications
|   └── services.html                         # the formatting for services
├── _layouts                  
|   └── homepage.html                         # the html template for the homepage 
├── _sass
|   ├── minimal-light.scss                    # compiled into a CSS file to control the style of the page              
|   └── minimal-light-no-dark-mode.scss       # similar to minimal-light.scss with the dark mode disabled
├── assets                                    # some files
├── .gitignore                                # this file specifies intentionally untracked files that Git should ignore
├── Gemfile                                   #  
├── LICENSE                                   # the license file
├── README.md                                 # readme file (English)
├── README_zh_Hans.md                         # readme file (Simplified Chinese)
├── README_zh_Hant.md                         # readme file (Traditional Chinese)
├── _config.yml                               # Jekyll configuration file, including some options of the page  
└── index.md                                  # the content of the index page, using Markdown
```

## Advanced options

If you know a bit how to use git, then you can edit and test your website locally rather than making every change directly on Github.

- **Using locally with Jekyll.** You may install Jekyll on your own computer and generate static web pages (i.e., HTML files) with this template. After that, you may upload the HTML files to your server.

The detailed instructions are available below.


### Using with the GitHub Pages Service

There are two ways to use this template on GitHub:

#### Fork this repository
- Fork this repository (or [use this repository as a template](https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/creating-a-repository-from-a-template)) and change the name to `your-username.github.io`.

- Enable the GitHub pages for that repository following the steps [here](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site#creating-your-site).

#### Using this repository as a remote theme
???

### Using Locally with Jekyll

First, install [Ruby](https://www.ruby-lang.org/en/) and [Jekyll](https://jekyllrb.com/). The install instructions can be found here: <https://jekyllrb.com/docs/installation/#guides>

Then, clone this repository:

```bash
git clone https://github.com/yaoyao-liu/minimal-light.git
cd minimal-light
```
Install and run:

```bash
bundle install
bundle exec jekyll server
```
View the live page using `localhost`:
<http://localhost:4000>. You can get the HTML files in `_site` folder.

### Using the HTML version

The compiled HTML files are available in the `html_source_file` folder. If you don't like Jekyll, you may directly edit and use the HTML version.

## Customizing

### Required customization

### Optional customization 




### Edit `index.md`

Create `index.md` and add your personal information. It supports **Markdown** and **HTML** syntax.

### Edit included files

There are two markdown files included in `index.md`. They are `_includes/publications.md` and `_includes/service.md`, respectively. These two files also support **Markdown** and **HTML** syntax. If you don't hope to include these two files, you may remove the following lines in `index.md`:
https://github.com/yaoyao-liu/minimal-light/blob/b38070cd0b6bce45d8a885f3828549af8f82b7cb/index.md?plain=1#L21-L23

If you hope to edit the publication list without changing the format, you may edit `_data/publications.yml`:
https://github.com/yaoyao-liu/minimal-light/blob/77b1b3b31d4561091bcd739f37a2e1880e8b5ca5/_data/publications.yml#L3-L11


### Stylesheet

If you'd like to add your own custom styles, you may edit `_sass/minimal-light.scss`.

### Layouts

If you'd like to change the theme's HTML layout, you may edit `_layout/homepage.html`.

## License

This work is licensed under a [Creative Commons Zero v1.0 Universal](https://github.com/haryrichman/minimal-light-academic/blob/master/LICENSE) License.

## Acknowledgements

Our project uses the source code from the following repositories:

* &#x21A2; [yaoyao-liu/minimal-light](https://github.com/yaoyao-liu/minimal-light)
  * -> [Xiao-chenguang/minimal-light](https://github.com/Xiao-Chenguang/minimal-light)
  * <- [pages-themes/minimal](https://github.com/pages-themes/minimal)

  * <- [orderedlist/minimal](https://github.com/orderedlist/minimal)

  * &#x21A2; [al-folio](https://github.com/alshedivat/al-folio)

