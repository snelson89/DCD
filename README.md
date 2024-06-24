# Syllabus & Introduction to Latex (6/12)

1. [Syllabus](files/syllabus.pdf)
2. [Intro to LaTeX handout](intro-to-latex.pdf)
3. [Overleaf Project](https://www.overleaf.com/read/qqqmjkskpkqq#810b0b)

# Meeting Cancelled (6/19)

# Introduction to git + GitHub Pages (6/26)

## git

1. What is git?
    - git is a version control system that allows you to keep track of how files change over time and access previous version of files. It also allows you to have multiple versions of the same directory on multiple computers at the same time and with multiple people.
2. Why git?
    - It's used a lot in higher level courses and research. So knowing how to use it will benefit you. It's also open-source and doesn't rely on any single file type. You can track changes in folders of all different file types (though it works best with plain text files).
3. How git?
    - Typically git is used through a command line interface (CLI) but today you will learn how to use it with a graphical user interface (GUI). While git itself is open-source, there are online services that host your repositories and allow you to share them with the dier world. The most popular service is **GitHub**. If you do not already have a GitHub account, [click here](https://www.github.com) and sign up for an account. Then, [click here](https://desktop.github.com) and download **GitHub Desktop** for your operating system. This is the GUI that will allow you to run git commands from your local machine.
  
### The Basics

1. Intializing a repository
    - Suppose you are starting a new project and want to keep track of all the files you will be using.
    - In this instance what you might want to do is first create a new directory on your local machine. Do that now and name it `[your name]_first_github_directory`.
    - Once you have done that, add a file to the directly called `notes.txt`. In the `notes.txt` file write a sentence or two about what you have learned so far today.
    - As of right now, this is just a "normal" folder on your machine. To make it a git-enabled folder and connect it with your GitHub account, open up GitHub Desktop and navigate to *Create New Repository...*. It will ask you for a few different things, but for now we only care about the **Name** and **Local Path**. For **Name** you can type "[your name]_first_github_directory" and for **Local Path** you should use the path to the folder you have just created. Make sure not to put the directory name itself, otherwise it will create a new directory within the one you just created.
    - Your repository is now set up. You have two options at this point:
         1. Keep adding/changing files
         2. Publish your repository  
    - Publishing your repository makes it "official" on GitHub and will allow you to share it with others. You don't need to publish it right away, though, as it will still keep track of all the changes you make.
     
2. Cloning a repository
    - Suppose someone else has started a new project and you would like to join their repository.
    - In this instance what you want to do is *clone* the repository. There are a few different ways this can be done, but I'll show you only one.
    - This can happen in two steps:
        1. Obtain the repository's https link (e.g. `https://github.com/snelson89/DCD.git`)
        2. In GitHub Desktop, click *Clone Repository...*, navigate to URL, paste the link, and add a local path  
    - To practice, clone my DCD repository to your local machine.
    - You now should have a folder on your computer called `DCD`
     
3. Tracking/Ignoring/Committing Files
    - Generally when using git, you need to specify which files should be tracked. When using GitHub Desktop (at least certainly when initializing a repository with GitHub Desktop) it automatically tracks every file that you add to the repository.
    - Add one new file `script.py` with the single line `print("Hello World") to the original directory that you made and a new directory `[Your Name]` with a file `favorites.txt` that lists your favorite food, music, movie, and city to the DCD repository.
    - Open GitHub Desktop and view the changes made in each repository.
    - Suppose in your repository you don't want to track any changes made to Python files (files ending in `.py`). You can systematically do so by using a `.gitignore` file. GitHub Desktop can create this automatically for you. In the **Changes** section you can right-click on a file and see a set of options. One of these options is *Ignore all [filetype] Files (Add to .gitignore). If you click this after clicking on `script.py`, you should see a new file change pop up that adds `*py` to `.gitignore`.
    - Now, create a file `script2.py` with the single line `print("Goodbye World")` to the repository. Notice that it does not show up on the **Changes** page of GitHub Desktop. If you want to go back to tracking Python files, you can open `.gitignore` and delete the line `*py`. Do so now and see that your two `.py` files show up again in **Changes**.
    - So far, all we've done is track files that have changed, but to make it perminent we still have to *commit* those changes. Commiting changes is basically telling the repository, "Ok, I made these changes on purpose and in this very moment I am happy about it."
    - On the **Changes** tab of GitHub Desktop and near the bottom, you will find a line that says *Summary (required)*. Here, you need to provide a short summary about the changes you made. For your repository you might put something like "added python files" and for the DCD repository you might put something like "added a folder with a file about some of my favorite things". Here, you want to be brief but informative. Recall that one of the advantages of git is that you can keep track of older versions of files. One way to easily find older versions is by using helpful commit messages!
    - Once you've added a commit message you can click *Commit to main*. Your changes have now been committed. Do so now for both repositories.
      
4. Pushing/Pulling Files
    -

And that's the basics. There is a lot more you can do with git but those features are beyond what we have time to discuss today. If you are interested in learning more, I have provided some links below.


### Further Resources

1. [Interactive git demo](https://git-scm.com/doc)
2. [GitHub documents/manual](https://docs.github.com/en/get-started)
3. [GitHub command line interface tutorial](https://docs.github.com/en/github-cli/github-cli/quickstart)
4. [GitHub git cheatsheet](https://education.github.com/git-cheat-sheet-education.pdf)


## GitHub Pages
