# code-societies
This is the super repository for all code societies sessions. Readme is currently a work in progress!

This website is hand-coded. There are no large libraries, frameworks or build processes. All pages are written with HTML and CSS and sometimes Javascript. There is one library that this website is relying on: a javascript library called Axios. With Axios this website can request data from are.na, a research platform which code societies students and teachers use to collaboratively add and share content throughout the session.

### preparation for contributing
- a personal GitHub account
- working knowledge of HTML (code societies organizers are here to guide you!)
- working knowledge of Terminal (optional!)

### if you are using git and github for the first time:
- Create a personal GitHub account
- Check if you already have git installed by running this in your terminal `$ git --version`
- If the terminal doesn't not return a response like `git version 2.20.01 ...` then you'll need to follow this [link](https://sourceforge.net/projects/git-osx-installer/files) to download and install it. If you are on a Windows computer follow this [link](https://git-scm.com/download/win)
- If it installed properly you should see the current git version when you run this command again in your terminal `$ git --version`
- Now lets connect the git software to your personal GitHub account
- git config --global user.name "Your Name"
- git config --global user.email "emailyouused@foryourgithubaccount.com"
- Now you will be able to use git prompts in your terminal like `git init` and `git clone`

### how to contribute
If you would like to contribute to this repository:
- you should currently be logged into your github account
- click the `fork` button in the upper right corner of this page
- this will create a copy of this repository under your account, you should be automatically taken this new page on your account

##### setting up Terminal for contribution
- clone your forked repository with `$ git clone https-url-of-github-repository`
- `$ cd code-societies`
- `$ git remote add upstream https://github.com/SFPC/code-societies.git`
- Check that you have added upstream correctly with `$ git remote -v`
- The terminal should print something like this:

        origin	git@github.com:yourusername/code-societies.git (fetch)
        origin	git@github.com:yourusername/code-societies.git (push)
        upstream	https://github.com/SFPC/code-societies.git (fetch)
        upstream	https://github.com/SFPC/code-societies.git (push)

##### contribution workflow, make sure to follow these steps BEFORE you add files or change code!
- `$ cd code-societies`
- Follow the next three steps every time you want to make a new contribution to the blog!
- 1. Fetch from upstream remote with `$ git fetch upstream `
- 2. Checkout master branch and merge the code from the SFPC repo into yours with `$ git checkout master`
- 3. Then `$ git merge upstream/master`
- Now create a new branch `$ git branch whatever-you-want-to-name-your-branch`
- Switch over to your new branch `$ git checkout whatever-you-named-your-branch`
- Now you can open the code-societies repo in your preferred code editor and create your new post! This will probably look something like duplicating the blog post base HTML file, adding your writing, ensuring HTML tags are added etc etc. More details on post formatting are [here](http://sfpc.io/code-societies/blog/post-template-guide.html)
- Once you have added all of your changes and files you can follow these steps to push your new files up to GitHub:
- To ensure that any new files you added are pushed up run `$ git add -A`
- Now you will "commit" your work by running `$ git commit -m "adding my new post and some images"` The message inside of the quotes can be whatever you want but should be a succinct description of the work you have done.
- Finally, push your code up to GitHub with `$ git push origin whatever-you-named-your-branch`

##### creating a pull request, aka officially adding your new post to the SFPC code societies blog
- In a browser go to the forked code societies repository page under your GitHub account
- Click on the `branch` link near the top of the page, in between where it says the number of commits and the number of packages
- You should see your branch listed here. Click the `New pull request` button.
- This will take you to a new page. Feel free to add comments then click the green `Create pull request` button.
- THATS IT! One of the organizers will see your pull request and will review it. If everything looks good they will merge your code into the SFPC repo and it will be live!
