# How to edit Epigraphy.info website
**Petra Hermankova**

**Contact:** [petra.janouchova@gmai.com](mailto:petra.janouchova@gmail.com) / [petra.hermankova@cas.au.dk](mailto:petra.janouchova@gmail.com) 

[@petrifiedvoices](https://github.com/petrifiedvoices) on GitHub

**Website:** static website using [GitHub pages infrastructure](https://guides.github.com/features/pages/) (Jekyll), pages written in markdown and then automatically transformed to html

If you are planning to do a major change (adding new pages, instead of editing the existing ones, changing layout and the design etc.), please contact Petra.

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
1. be added to the epigraphy-info Github organization (in order to work independently)
1. or you can commit your changes and someone from within the organisation has to approve your changes


There are two modes of editing the website:

### ONLINE 

- only when editing one document and changing small things such as typos or hyperlinks
- potentially unsafe, should be used only for small edits within one file; not for large development

1. Go to the website repo.
1. Find your document.
1. Make edits.
1. Commit changes.
1. Go to the GithubPages and wait for the server to process the change.

### LOCALLY on your computer

- safer option; steep learning curve but great for tracking changes anc collaboration between multiple people
- preferred mode!
- the easiest way is to use command line (Terminal) on your computer, but if you prefer there are several GUI Clients/softwares that you can use on Windows and Macs such as [GitHub Desktop](https://desktop.github.com/)
	
#### First time working with repo

1. Clone the repo to your local computer. `git clone “address of your repo” `
1. Make edits to all your files.
1. Add changes. `git add “file” `
1. Commit changes. `git commit -m “my commit message” `
1. Push changes to Github. `git push origin “name of branch” `
1. Go to the GithubPages and wait for the server to process the change.

#### Second time working with repo

1. Go to the folder containing website docs on your computer.
1. Pull all new changes from Github to your local computer. `git pull ` 
1. Make edits to all your files.
1. Add changes. `git add “file” `
1. Commit changes. `git commit -m “my commit message” `
1. Push changes to Github. `git push origin “name of branch” `
1. Go to the GithubPages and wait for the server to process the change.

#### Major changes

If you are planning major changes, or want to see how they look on the website before committing them to GitHub, you can run Jekyll server locally on your computer and test locally.

1. Go to the folder containing website docs on your computer.
1. Pull all new changes from Github to your local computer.
1. Using the command line, start the Jekyll server `bundle exec jekyll serve`. You may need to install [Jekyll prerequisites](https://jekyllrb.com/docs/) to your 1. computer first.
1. Make edits to all your files.
1. Type ‘http://localhost:4000’ in your browser and check the changes you have made on the website. 
1. Once you are happy with your changes, add them, commit and push them to Github.
1. Go to the online GithubPages and wait for the server to process the change.

#### Alternative branches and pull requests

If you are making a lot of changes at the same time, you may consider creating a new branch instead of making the changes directly to the main branch where the website is stored. Once you are happy with your changes, you can merge the branch with the main by pull request. How to create a pull request is best summarized on this link [https://guides.github.com/activities/hello-world/](https://guides.github.com/activities/hello-world).
