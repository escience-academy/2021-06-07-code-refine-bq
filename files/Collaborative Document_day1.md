# Collaborative Document

2021-06-07-code-refine-bq day 1.

Welcome to The Workshop Collaborative Document.

This Document is synchronized as you type, so that everyone viewing this page sees the same text. This allows you to collaborate seamlessly on documents.

----------------------------------------------------------------------------

## 👮Code of Conduct

Participants are expected to follow these guidelines:
* Use welcoming and inclusive language.
* Be respectful of different viewpoints and experiences.
* Gracefully accept constructive criticism.
* Focus on what is best for the community.
* Show courtesy and respect towards other community members.

If you think the code has been violated: contact a trainer, or write to training@esciencecenter.nl.
 
## ⚖️ License

All content is publicly available under the Creative Commons Attribution License: [creativecommons.org/licenses/by/4.0/](https://creativecommons.org/licenses/by/4.0/).

## 🙋Getting help

To ask a question, type `/hand` in the chat window.

To get help, type `/help` in the chat window.

You can ask questions in the document or chat window and helpers will try to help you.

## 🖥 Workshop website

[link](https://escience-academy.github.io/2021-06-07-code-refine-bq/)

🛠 Setup

[link](https://escience-academy.github.io/2021-06-07-code-refine-bq#setup)


## 👩‍🏫👩‍💻🎓 Instructors

Barbara Vreede, Jens Wehner, Sven van der Burg

## 🧑‍🙋 Helpers
Mateusz Kuzak


## 🗓️ Agenda
* 09:00	Welcome
* 09:15	Collaboration with Git and GitHub
* 10:15	Coffee break
* 10:30	Collaboration with Git and GitHub
* 11:30	Coffee break
* 11:45	Collaboration with Git and GitHub
* 12:30	Lunch
* 13:30	Introduction to Continuous Integration
* 14:30	Coffee break
* 14:45	Introduction to Continuous Integration
* 15:45	Wrap-up
* 16:00	END

## 🧠 Collaborative Notes
### Introduction
* Software Engineering is Programming integrated over **time**
* Software engineering tools:
    * Version Control
    * Gitlab/Github
    * Code Review
    * Testing
* Software engineering tools will slow down development time in the beginning, but will speed it up once the project gets more complex.
* When to use what software engineering tool depends on:
    * The number of collaborators
    * How long should the code last?
    * How may people use it?

### Collaboration with Git and GitHub
#### Creating a new repository
* Public repository: Everyone on internet can see your project (but not edit)
* Private repostiory: You're the only people that can see your project
* Don't put your data in you software repo, use e.g. [zenodo](https://zenodo.org/) or [dryad](https://datadryad.org/stash)
* README file: documentation for you project
* Gitignore file: makes sure some files are ignored by git
* [Choose a license](https://choosealicense.com/): e.g. Apache
    * People cannot use your code if you don't add a license!
    * It's a good idea to talk to the legal department about licensing.
    * Open-source is a good idea!
        * Other people can use your code
        * You can use your code if you change institution
#### Adding files to your repository
* Create a new file
    * Click 'Add file' -> 'Create new file'
* Edit the file
* Commit the file
    * Scroll down, add a commit message and hit 'commit new file'

#### Insights
* Click 'Insights' in top horizontal navbar
* Click 'Network' in left navbar
    * Network shows a graphical overview of all your commits

#### Contributing
* By default no one can edit code in your repository apart from you. You can invite collaborators in 'Settings' -> 'Manage access'.
* Invitations are in the 'notifications' top-right alarm bell button. Or in your email box.

The collaboration process:
* Create a new branch (with a good name)
* Commit changes
    * Use clear commit messages, and commit one conceptual change at a time (which can be a lot files!).
* Create a pull request -> a request for merging the changes on your branch into the main branch (if you are using GitLab, this was renamed to Merge Request!)
* Request a review
* Review the code
    * Be nice, be positive, give constructive criticism, consider the context
* Merge pull request, the commits are now in the main branch
* Delete the branch (there is no need for it anymore)


* Why a draft pull request?
    * You basically mark it as 'not done yet'. It can be useful to mark it as such.

#### BREAKTIME! Get back at 10:30

### Exercise: Working as a project collaborator (in breakout rooms)

- Log into Github and create a new repository
- Make the repository public
- clone it to your desktop
- add some code
- push the changes to the repository
- Add one person as a collaborator (settings -> Manage Access). Make sure everyone in the group has a collaborator.
- Clone that repo
- make changes on a new branch
- push the changes
- submit a Pull Request
- wait for approval
- At the same time review a collaborators Pull Request
- (Optionally) Learn about [protecting branches](https://docs.github.com/en/github/administering-a-repository/about-protected-branches) and try it out.

### Collaboration in a distributed setting
* Kickout your collaborator (Settings --> Manage access)
* You cannot edit files in a project if you're not a collaborator
Process:
* Create a 'Fork' (a copy of the repository on your own account/namespace)
* Commit changes (you can very well do this in the main branch, because it is in your own account)
* Create a Pull Request, merging your fork's main branch in the original repository main branch.
* Do review

**BREAKTIME: Get back at 11:45**

### Exercise: Working as an external contributor (in breakout rooms)
- Remove your group member(s) as collaborators from your repository
- Fork another group members repo (Repository page, top right corner)
- Create an issue on the original repository
- Clone your forked repo to your computer
- Make some changes, use a somewhat real-world example so it makes sense to review it (but don't overdo it).
- Push it to your fork
- Make a change and commit it to the main branch
- push the changes
- make a pull request from your fork to the main repository mentioning the issue
- Consider turning your Pull Request into a draft Pull Request.
- let your code be reviewed by tagging the repo owner using (@Username)
- At the same time review Pull Request using comments on individual lines. Try to act as if it was a real peer review as much as possible.
- Accept or reject the Pull Request
- (Optionally) learn about [merge conflicts](https://www.atlassian.com/git/tutorials/using-branches/merge-conflicts) and try it out in your collaboration.

### Exercise: Recap Collaboration with Git and Github
Take a few minutes to write down your thoughts on what we just learned about Collaboration with Git and Github:
* What questions do you still have?
* Whether there are any incremental improvements that can benefit your projects?
* What’s nice that we learned but is overkill for your current work?


### Feedback
#### What went well? :thumbsup: 
* Working in breakout rooms are nice.
* A good overview of what all you can do with Github
* Good time managment, really nice insight from instrcutors
* Great support duringa activities and use of coffe-breaks.
* Very nice interactivity between instructors
* Nice interactivelly organized course
* Good time management and break out rooms with the same groups
* Practicing everything step by step is really nice for learning.
* Very practical, empathetic instructors and schedule is respected
* Nice way of learning new techniques
* The idea of the shared document is great, putting a short resume of the class helps when it happens to get a bit lost
* Nice pace, good break timing
* 
* Good pace + showing an actual project helps to frame the theory
* Useful to have breakout rooms to make practice
* Good gradual introduction di Github


#### What could be improved? :thumbsdown: 
* I think it could have been faster
* The course is introductory to git/ collaboration tools. For those with a bit more knowledge, it might feel a bit slow. (but the level should (and is) adapted to majority) 
* the demo about forking was a bit fast, but that was for the sake of having a break ;) <-- I quote that
* The breakout rooms could be with two people working together, so we can't interrupt our roommates :) 
* It would be great if we have detailed PDFs (tutorial about exercise ?)
* since often the tasks required collaboration in couples, maybe breakout rooms of 2 people might have been more practical (?)
* Small command line example would be nice
* Sometimes there is no correspondence between what is state in the explanantion of the exercise and the exercise itself. 


### Exercise: Setup Continuous Integration on Github
You will work on the exercise **individually** in breakout rooms so you can help each other out and ask questions if needed.

In this exercise, you will:
- Create a repository on GitHub
- Commit code to the repository and set up linting with GitHub Actions
- *Linting* is the process of checking your code for errors or code style violations.

#### Step 1: Create a new repository on GitHub
- **Before** you create the repository, select **"Initialize this repository
  with a README"** (otherwise you try to clone an empty repo).

#### Step 2: Clone your own repository, add code, commit, and push

Clone the repository.

Add a file `example.py` containing:

```python
def print_temperature():
    print(temperature)
```

Then stage the file (`git add <filename>`), commit (`git commit -m "some commit message"`),
and push the changes (`git push origin main`).


#### Step 3: Enable automated testing

In this step we will enable GitHub Actions.
Select "Actions" from your GitHub repository page. You get to a page
"Get started with GitHub Actions". Select the button for "Set up
this workflow" under Python Application.

GitHub creates the following file for you in the subfolder `.github/workflows`:


   ```yaml
   # This workflow will install Python dependencies, run tests and lint with a single version of Python
   # For more information see: https://help.github.com/actions/language-and-framework-guides/using-python-with-github-actions

   name: Python application

   on:
     push:
       branches: [ main ]
     pull_request:
       branches: [ main ]

   jobs:
     build:

       runs-on: ubuntu-latest

       steps:
       - uses: actions/checkout@v2
       - name: Set up Python 3.8
         uses: actions/setup-python@v2
         with:
           python-version: 3.8
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install flake8 pytest
           if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
       - name: Lint with flake8
         run: |
           # stop the build if there are Python syntax errors or undefined names
           flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
           # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
           flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
       - name: Test with pytest
         run: |
           pytest
   ```

Remove the last part:
```yaml
   - name: Test with pytest
     run: |
       pytest
```
We will get back to this in the lesson on testing.

Commit the change by pressing the "Start Commit" button.

#### Step 4: Verify that github action has been automatically run

Observe in the repository how the github action fails. While the github action is executing, the repository has a yellow marker.
This is replaced with a red check mark, once it is done.

Also browse the "Actions" tab and look at the steps there and their output.

You should be able to find that the linter complains:
``` F821 undefined name 'temperature'.```

#### Step 5: Fix the undefined name error
Indeed we forgot to define a variable `temperature`

Let's fix that:
```python
temperature = 10

def print_temperature():
    print(temperature)
```
Commit this change!

#### Step 5: Verify that github action runs succesfully
Now that you fixed the bug in your code the github action should succeed.

#### Step 6: Understanding github action yaml syntax
This is the part of the github action yaml configuration that is responsible
for the linting step:
```yaml
    - name: Lint with flake8
      run: |
        # stop the build if there are Python syntax errors or undefined names
        flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
        # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
        flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
```        
It basically just calls the program `flake8` with some arguments. `flake8` is a python linter.


### notes
pypi.yml includes settings to publish your code/package on pypi. 

build.yml includes installation, tests and linters i.e. tools that check your codes against code styles and errors. 

### Exercise: Recap Continuous Integration
Take a few minutes to write down your thoughts on what we just learned about Continuous Integration:
* What questions do you still have?
* Whether there are any incremental improvements that can benefit your projects?
* What’s nice that we learnt but is overkill for your current work?


### Documentation

* More documentation is better, but more documentation also takes more time.
* Trade-off: is the effort worth the outcome?
* Small effort made in documenting your project goes a long way!
* Documentation types:
    * in-code documentation (comments)
    * README
    * project documentation automated e.g. with Sphinx, deployed to ReadtheDocs
    * project website

Why is documentation important?
* Let other people know how the code works.
* Let yourself know how the code works (later on).
* People that use your code 
* Visibility of the project (making it usable)

#### Exercise: good/bad documentation

Write down your thoughts in the collaborative documents.
Respond with emojis :+1: :scream_cat: to your colleagues' answers.
- Think of projects of which you like the documentation. What do you like about them?
- Think of projects for which you don’t like the documentation. What don’t you like about them? Are you missing anything?

**NB: You can choose a mature library with lots of users for this exercise, but try to also think of less mature projects you had to collaborate on, or papers you had to reproduce.**


#### In-code documentation
- How to make code more easily understandable?
- What info should go into comments?
- What info should go into docstrings?


### Exercise: Writing good comments
Let's take a look at two example comments (comments in python start with `#`):
#### Comment A
```python
# Now we check if temperature is larger than -50:
if temperature > -50:
    print('do something')
```

#### Comment B
```python
# We regard temperatures below -50 degrees as measurement errors
if temperature > -50:
    print('do something')
```
 Which of these comments is best? Can you explain why?
 Write your answer in the collaborative document (before looking at others' answers)


### Writing docstrings
The bare function:
```python=
def mean_temperature(data):
    temperatures = data['Air temperature (degC)']
    return sum(temperatures)/len(temperatures)
```

Adding a docstring: structured comment associated to code.

- What does the method do?
- What goes in?
- What comes out
```python=
def mean_temperature(data):
    """
    Get the mean temperature
    
    Args:
        data (pandas.Dataframe): A pandas dataframe with air temperature measurements
        
    Returns:
        The mean air temperature (float)
    """
    temperatures = data['Air temperature (degC)']
    return sum(temperatures)/len(temperatures)
```
This is a google-style docstring, but there are other styles. Python parses this docstring, so you can call it as help:
```python=
help(mean_temperature)
```

The structure allows automatic generation of documentation: it is not just structured for humans, but also for machines!



### Exercise Adding in-code documentation

 Update this code snippet so it is well-documented:

 ```python
 import pandas as pd
 
 def x(a, print_columns=False):
    b = pd.read_excel(a)
    column_headers = list(b.columns.values)
    if print_columns:
        print("\n".join(column_headers))
    return column_headers
 ```
 1. Work individually on your solution (5 minutes)
 2. One person screen-shares their solution, discuss and together settle on a final solution. (5 minutes)
 3. Share final solution in collaborative document.

* Group 1:
```python 
 import pandas as pd
 
 def column_header_reader(excel_file, print_columns=False):
    """
    The function returns the column headers of the imported excel_file.
    
    Args:
      excel_file: imported Excel file to be saved into a pandas DataFrame.
      print_columns: boolean value (optional). If print_columns is True the list is also displayed.
    
    Output:
      column_headers: list of column headers of the Excel file.
      
    """
    dataframe = pd.read_excel(excel_file)
    column_headers = list(dataframe.columns.values)
    if print_columns:
        print("\n".join(column_headers))
    return column_headers
```

* Group 2:
```python
import pandas as pd

def getColNames(filepath, print_columns=False):
    ''' 
    Reads an excel file into a pandas dataframe and returns the column names in a List
    Args:
        filepath: string (path of the CSV file directory)
        print_columns: Boolean 

    Return:
        Column Headers in List format ('strings')
    '''

   # Reads an CSV file and stores it in a Pandas DataFrame 
   dataframe= pd.read_excel(filepath)
   
   # Keeps all the Column Names in a List 
   column_headers = list(dataframe.columns.values)
   
   # if TRUE prints the column_headers (1 per line)
   if print_columns:
       print("\n".join(column_headers))
   
   return column_headers
   ```
* Group 3:
```python
import pandas as pd
 
def x(a, print_columns=False):

    """
    Takes an excel sheet as input and returns the column headers
    
    Parameters
    ----------
    a : excel sheet 
        
    print_columns : (Bool). If you want to print the columns, 'print_columns=True'

    Returns
    -------
    column_headers : lists the values of the columns of the excel sheet


    """
   b = pd.read_excel(a)
   column_headers = list(b.columns.values)
   if print_columns:
       print("\n".join(column_headers))
   return column_headers
```  
* Group 4:
```python
"""
It parses an excel file and returns a list containing column headers.

args:
    a (String): String containing the path to an excel file.
    print_columns (Bool): If true, the method prints the header of each column of file a. Default: False.
    
returns:
    column_headers (list): A list containing all column headers in an excel file.
"""
```
* Group 5:
```python
import pandas as pd
 
def x(file_name, print_columns=False):
	"""
	Get the column names of an Excel input file.
    
    Dependencies: pandas.
    
	Args:
		file_name (Excel file): input excel data to retrieve column names from.
		print_columns (bool, optional): decide whether to print the column names, default=False.
		
	Returns: The columns names (list).
 	"""
    
    table = pd.read_excel(file_name)
    column_headers = list(table.columns.values)
    if print_columns:
        print("\n".join(column_headers))
    return column_headers
```

#### Sven's option
 ```python
 import pandas as pd
 
 def get_spreadsheet_columns(file_loc, print_columns=False):
     """
     Gets and prints the spreadsheet's header columns
     
     Args:
         file_loc(str): The file location of the spreadsheet
         print_columns (bool, optional): A flag used to print the columns to the console
     Returns: 
         a list of column headers
     """
    b = pd.read_excel(a)
    column_headers = list(b.columns.values)
    if print_columns:
        print("\n".join(column_headers))
    return column_headers
 ```


## 📚 Resources
More workshops by us: [escience-academy.github.io](https://escience-academy.github.io/)
We will have a workshop on Reproducible Computational Environments Using Containers in September
Automatically (using keywords) and manually linking a pull request to an issue: https://docs.github.com/en/issues/tracking-your-work-with-issues/creating-issues/linking-a-pull-request-to-an-issue
Or: [Mastering issues](https://guides.github.com/features/issues/) (for all the ways to reference users, pull requests, labels etc. in GitHub issues)
### Jupyter diffing
[nbdime](https://nbdime.readthedocs.io/en/latest/)
Notebook: 
https://www.kaggle.com/
https://www.colab.research.google.com/