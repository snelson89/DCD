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
    - Commiting is not enough. All that committing files does is tell your local machine that you are happy with your changes. In order to interact with the remote repository you musth *push* your changes after committing.
    - In GitHub Desktop, there will be a button on the top right of the header bar that says "push origin". Once you click this your changes will be sent to the remote repository and become official.
    - Push your changes to both your newly created repository as well as the DCD repository.
    - After everyone has pushed their changes to DCD, GitHub Desktop should now show that you can *pull* other people's changes. When you are sharing a repository with others (and working on the same branch) you will be in a constant state of pushing and pulling with others. Because of this, it's always important that you push all of your changes/commits at the end of a working session (or many times within a working session) and pull other people's changes before starting to work. If the files get out of sync there are ways to fix them, but it's a hassle and best to avoid these types of problems by cutting them off at the source.
    - To end, pull all of the changes that everyone made and make sure your DCD repository is up to date.

And that's the basics. There is a lot more you can do with git but those features are beyond what we have time to discuss today. If you are interested in learning more, I have provided some links below. This includes how to use git with the command line. In general, the strategy is the same: track files in a repository, commit those files once you have made changes, push/pull your commits to work remotely with yourself or others.


### Further Resources

1. [Interactive git demo](https://git-scm.com/doc)
2. [GitHub documents/manual](https://docs.github.com/en/get-started)
3. [GitHub command line interface tutorial](https://docs.github.com/en/github-cli/github-cli/quickstart)
4. [GitHub git cheatsheet](https://education.github.com/git-cheat-sheet-education.pdf)


## GitHub Pages

1. You can use your GitHub account to make a personal website. Many people in computer science (and related fields) use this method for making a personal website.
2. Let's use [this startup guide] to start making our own personal websites.
3. Why is it good to have a personal academic website?
   - Makes you look professional!
   - ...


### IACS Faculty Websites
1. [Alan Calder](https://www.astro.sunysb.edu/acalder/)
2. [Jeffrey Heinz](https://www.jeffreyheinz.net)
3. [Heather Lynch](https://www.lynchlab.com)
4. [Meg Schedel](http://www.schedel.net)
5. [Ben Levine](https://levinegroup.org)
6. [Yifan Sun](https://sites.google.com/site/yifansunwebsite)

# Informational Interviewing (7/3)

# CV Workshop (7/10)

# Research Methods (7/17)

## Lit Search
1. What is a literature search anw why is it important?
   - A "key step in performing good authentic research"
   - Critical for formulating research questions and identifying gaps
   - Allows you to identify commonly used methods for addressing relevant research questions
   - Organized and systematic literature searchers are necessary because there is such and incredible number of published studies and data
   - [Literature search for research planning and identification of research problem](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5037943/)
2. Have you performed a literature search in the past? How?
3. Define your research question:
   - Talk to your advisor/supervisor/mentor
   - Ask for some key research papers relevant to your interests
   - Look for relevant references that are cited in other papers and read those
4. Determine key words and perform a search:
   - After reading other papers you can come up with a set of key words
   - Use these words to search places like Google Scholar/etc.
5. Decide which papers to read:
   - Skim the title/abstract/results
   - Does it seem directly relevant?
   - Is it not directly relevant but heavily cited?
     
   

## Effectively Reading Papers

1. Ultimately, there is no correct way and you need to take notes in the way that is best for you learning style
   - Personally, I like reading physically printed copies better than digital (but still read a lot of digital stuff)
2. What to highlight/take notes of?
   - Key findings that support or do not support your hypothesis
   - Methods that may be something you should investigate further
   - Papers that are referenced in the text that you should find and read
   - Future directions listed in the paper that may be of interest (possible research topic)
3. [How to Read a Paper](https://dl.acm.org/doi/pdf/10.1145/1273445.1273458)
4. [Art of reading a journal article: Methodically and effectively](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3687192/)
   

## How to write a research paper

1. Parts of a manuscript
   - Title, authors, affiliations, keywords
   - Abstract
       - Briefly present the paper's background and objectives (what knowledge gap is your study filling?)
       - Explain the main components of the methods
       - Summarize key results
       - Approximately 300-350 words
       - Needs to be succinct!
   - Introduction
       - Why was the study conducted?
       - Why should anyone care?
       - What is the question being addressed?
       - What is unknown about the question?
       - In what system will you be addressing this question?
       - Key measurements you will be using
       - Conclude with primary hypotheses + any secondary hypotheses
   - Methods
       - Arguably the most critical part of a manuscript
       - Should be written succinctly, but with enough detail where the study could theoretically be replicated by a skilled researcher
       - Need to describe all methods involved for data collection
   - Results
       - Organization of Results section should parallel the organization of the Methods section
       - Start by describing the system (sample sizes, demographics of individuals, survey time periods)
       - Then describe the results that correspond to each aspect described in the Methods
       - Do not discuss what your results mean in the Results section
   - Discussion
       - Placeing your findings in a broader scientific context
       - Before starting, determine which topics are most important to discuss in the Discussion section
       - Start with brief discussion of main findings and then dive into each of the findings you determined to be the most important
       - After you place your findings in a greater context, discuss limitations of the study
       - End with realistic conclusiong -- what do your findings mean for the broader research community?
   - Acknowledgments
   - Tables and Figures
       - Do not show the same data in a table and in a figure
       - Do not repeat information in a table that is already described in writing in the Results section
       - Ensure figures actually help readers better understand the methods or results
   - Literature Cited/References
2. [Scott's experimental paper](files/writing-sample-3.pdf)
3. [Scott's theoretical paper](files/writing-sample-1.pdf)

## Peer Review

1. The process:
   - Scientist study something
   - Scientists write about their results
   - Journal editor receives an article and sends it out for peer review
   - Peer reviewers read the article and provide feedback to the editor
   - Editor may send reviewer comments to the scientist who may then revise and resubmit the article for further review.
   - If an article does not maintain sufficiently high scientific standards, it may be rejected
   - If an article meets editorial and peer standards, it is published in a journal

## File Organization

1. If you do not actively think about adata organization, you may store files in random locations and then be unable to find them later
   - A clear folder structure is the most straightforward method to ensuring you can find your files
   - You need to think critically about the most logical folder structure
   - You want to organized your files and then keep that structure because your code will likely pull files from your computer and if you alter file directories it can get messy
2. Organization tips:
   - Use hierarchical file folder structures
   - Organize folders by meaningful categories based on contextual information
   - Try to stick to a naming convention based on elements that are important to a project
   - Avoid long file/folder names
   - Do not use spaces (use capitals, periods, underscores)
   - Use a consistent date format
   - Include a version number
3. Data Storage:
   - You need to backup your data regularly
   - Store it in more than one place
   - Store it in two different types of media
       - External hard drives
       - Google Drive, Dropbox, etc.
       - Hard copies (?)
   - If you do not have automatic backups set up, then you need to plan on regularly backing up your data manually


