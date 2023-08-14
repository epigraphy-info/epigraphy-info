# How to edit Epigraphy.info website
Author: **Petra Hermankova**, [@petrifiedvoices](https://github.com/petrifiedvoices) on GitHub

**Website:** static website using [GitHub pages infrastructure](https://guides.github.com/features/pages/) (Jekyll), pages written in markdown and then automatically transformed to html

If you are planning to do a major change (adding new pages, instead of editing the existing ones, changing layout templates and the design etc.) and need help, please contact Petra.

You can easily change the contents of the existing pages, add photos, documents etc.

---

## Tutorials
[Markdown cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) on Github - examples of how Markdown works

[Markdown interactive tutorial](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet), to test your knowledge and to practice

GitHub and version control: [https://guides.github.com/](https://guides.github.com/), 

Best to start with [https://guides.github.com/activities/hello-world/](https://guides.github.com/activities/hello-world/)

## Get started

**In order to edit the website, you will need to:**
1. create a GitHub Account
1. ask to be added to the epigraphy-info Github organization (in order to work independently)
1. or you can commit your changes and someone from within the organisation has to approve your changes (as merge request, but you will still need to have your own GitHub account)


There are two modes of editing the website:

### ONLINE 

- only when editing one document and changing small things such as typos or hyperlinks
- potentially unsafe, should be used only for small edits within one file; not for large development

1. Go to the website repo.
1. Find your document.
1. Make edits.
1. Commit changes.
1. Go to the GithubPages and wait for the server to process the change.

### LOCALLY on your computer (preferred mode)

- safer option; steep learning curve but great for tracking changes and collaboration between multiple people
- the easiest way is to use command line (Terminal) on your computer, but if you prefer there are several GUI Clients/softwares that you can use on Windows and Macs such as [GitHub Desktop](https://desktop.github.com/)
	
#### First time working with repo

1. Clone the repo to your local computer. In terminal: `git clone “address of your repo” `
1. Make edits to your files and save them.
1. Add changes. Terminal: `git add “file” `
1. Commit changes. Terminal: `git commit -m “my commit message” `
1. Push changes to Github. Terminal: `git push origin “name of branch” `
1. Go to the GithubPages and wait for the server to process the change. It may take up to 10 minutes.

#### Second time working with repo

1. Go to the folder containing website docs on your computer.
1. Pull all new changes from Github to your local computer. Terminal: `git pull ` 
1. Make edits to your files and save them.
1. Add changes. Terminal: `git add “file” `
1. Commit changes. Terminal: `git commit -m “my commit message” `
1. Push changes to Github. Terminal: `git push origin “name of branch” `
1. Go to the GithubPages and wait for the server to process the change. It may take up to 10 minutes.

#### Major changes

If you are planning major changes, or want to see how they look on the website before committing them to GitHub, you can run Jekyll server locally on your computer and test locally. You have to have installed Jekyll and all dependencies on your local computer.

1. Go to the folder containing website docs on your computer.
1. Pull all new changes from Github to your local computer.
1. Using the command line, start the Jekyll server by typing into the Terminal `bundle exec jekyll serve`. You may need to install [Jekyll prerequisites](https://jekyllrb.com/docs/) to your computer first.
1. Make edits to all your files.
1. Type ‘http://localhost:4000’ in your browser and check the changes you have made on the website. 
1. Once you are happy with your changes, add them, commit and push them to Github.
1. Go to the online GithubPages and wait for the server to process the change.

#### Alternative branches and pull requests

If you are making a lot of changes at the same time, you may consider creating a new branch instead of making the changes directly to the main branch where the website is stored. Once you are happy with your changes, you can merge the branch with the main by pull request. How to create a pull request is best summarized on this link [https://guides.github.com/activities/hello-world/](https://guides.github.com/activities/hello-world).


### Structure of the pages

* Main page lives in `index.html` document
* Other pages live in markdown files with the file extension .md
* Configuration files live in YAML files with the file extension .yml, or in folders `_data`, `_includes`, `_layouts`, `_sass`, `css`, `js`
* The static website lives in the folder `_site` - do not change anything here manually
* Photos live in the folder `assets`
* Posts in the News section live in the folder `_posts` - please use the provided template post
* PDFs, presentations and other documents live in the folder `documents`
* For better organisation and navigation between files, some of the pages live in separate folders, such as `meeting_pages` or `working_groups`

### Templates

**News**

The template post/news lives in the folder `_posts` >>> [Template post](../_posts/2021-01-01-Template_post.markdown)

**Photos**

The image has to exist locally / on GitHub in the folder `assets`

```photos
<img src='{{site.baseurl}}/assets/XXX.jpg' style="width:100%;" alt="Provide a description of your XXX image" align="middle">
```

**Hyperlink**
```
[This is my public name for the link](https://en.wikipedia.org/wiki/Epigraphy)
```

**Hyperlink to document on this page**

The documents has to exist locally / on GitHub in the folder `documents`

```
[This is my public name for the document, e.g. the 5th Epigraphy info programme]({{ site.baseurl }}{% link documents/Epigraphy.info_V_Programm.pdf %})
```

### Adding new pages

If you add a new page, e.g. a new workshop page, you need to do the following steps:
1. create a new file with `.md` extension in the `meeting_pages` folder (or in the corresponding folder for working groups, or in the main directory if there is no corresponding folder). You can use existing files with past workshops as a template.
2. In order to create a record in the navigation dropdown, you need to add the new page in the `_data/` folder in the file `samplelist.yml` following the already existing structure. Mind the indents, as the indentation creates a hierarchy of the dropdown. Make sure you provide a title and correct url, e.g. `title: Workshop 1 (Heidelberg)`, `url: workshop_1/` as provided in the `samplelist.yml` file.
3. Once you have added the existing website to the `samplelist.yml` file, commit to Github, wait few minutes and your changes should apprear on the website.
4. If you are unsure on how to do this, or your changes did not get through, feel free to contact Petra, either via email or [GitHub Issues](https://github.com/epigraphy-info/epigraphy-info/issues)
