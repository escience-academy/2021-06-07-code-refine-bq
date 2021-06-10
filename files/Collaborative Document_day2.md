# Collaborative Document

2021-06-07-code-refine-bq day 2.

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
 
training@esciencecenter.nl - in case of violation
 
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

## Post-workshop survey

[link](https://www.surveymonkey.com/r/RMPB3TP)

## 👩‍🏫👩‍💻🎓 Instructors

Sven van der Burg, Jens Wehner

## 🧑‍🙋 Helpers

Barbara Vreede, Sarah Alidoost,


## 🗓️ Agenda
* 09:00	Welcome
* 09:15	Documentation Part II
* 10:15	Coffee break
* 10:30	Documentation Part II
* 11:30	Coffee break
* 11:45	Introduction to Testing in python
* 12:30	Lunch
* 13:30	Introduction to Testing in python
* 14:30	Coffee break
* 14:45	Writing Modular Code
* 15:45	Wrap-up
* 16:00	END



### README

- Easiest thing to add, first thing a user or collaborator sees!


### Exercise: Design a README file
 You are going to design a README file for an example project.

 #### The example project
 Here's [the example project](https://github.com/escience-academy/coderefinery-documentation-example-project).
 For this project we transformed the code snippets from the previous episode into a single script [analyse_spreadsheet.py](https://github.com/escience-academy/coderefinery-documentation-example-project/blob/main/analyse_spreadsheet.py)
 
 Let's take a look at [the script](https://github.com/escience-academy/coderefinery-documentation-example-project/blob/main/analyse_spreadsheet.py). 
 You don't need to understand the script completely, all you need to know is:
 * The functions `mean_temperature` and `get_spreadsheet_columns` from previous episode are in there.
 * We added a `main` function that is called when you run the script 
 (you could run this python script by calling `python analyse_spreadsheet.py` on the command line). 
 It will prompt the user for a file name, print the columns in the spreadsheet, and print the mean
 temperature.
 
 That's all there is to this project! (You can ignore the other files in the repository, we'll get back to them in episode 4)

 #### The exercise (10 minutes)
 1. Think of what sections should go in the README file for this project.
 5. Discuss your ideas on the README file in the breakout room. What should definitely be included? Write down a short list in the collaborative document. You don't have to write out the whole README file.

  
 (Optional): Write out the full README and use [https://hemingwayapp.com/](https://hemingwayapp.com/) to analyse your README file and make your writing bold and clear!
 
#### Answers
Group 1:
* Main description: This is a code for calculating the mean temperature based on the excel files on the input.
* Sections:
* System requirement
* Dependencies ==> Python 3, pandas library
* Licence protection
* Research / Commercial purposes
* How to install and run the code
* The aim of the code

Group 2:
* Main function fuctionality description.
* Input data format (example of how is the input data)
* Ouput data obtained (example of the output data)
* Example of the whole pipeline (workflow)
* License
 
Group 3:
 * the purpose/goal of the code 
 * how to use it, including what is input and what is the output 
 * data format
 * authors and references 
 * license 
 * if it can be used for commercial purposes or only for research
 * exception of the code use 
 * examples
 
Group 4:
 * general description
 * installation instructions 
 * Dependencies
 * References/credits
 * Functions description (IO)
 * Description of workflow
 
Group 5:
- copy/paste of main function explanation? (or adaptation to it)
- example of code usage (code snippet)
- give hints on alternative usage of code (e.g. with different data sources)
- changelog


Our list:
- a descriptive project title
- motivation (why does the project exist)
- how to set it up (requirements, installation instructions)
- copy-pasteable quick start code example
- recommended citation

Main take away: what does the user need to know? A good readme file is key for your project!

### Sphinx and ReadtheDocs demo

- If a README is not enough: easily create user documentation
- Create nicely formatted html pages from markdown files with Sphinx (language-independent!). 
- ReadtheDocs connects to your github and deploys your sphinx documentation for free.
- Documentation files are in the `docs/` folder.
- Write markdown files and run sphinx on these files.
- API reference is created automatically from the docstrings

#### Do it yourself:
- Open with Anaconda Navigator

Open a terminal in jupyter lab by clicking on terminal tab. 
Make sure if python is installed by typing: python3 --version
and sphinx-build --version
and sphinx-quickstart --version

if not, you can install it by:
```
pip install sphinx
```

let's make a new directory by:
```
mkdir doc-example
```

and move into that:
```
cd doc-example
```

Then type `sphinx-quickstart` to run sphinx.

to answer questions, just use defaults (press Enter).

### Exercise: Add content to your example documentation
Follow instructions in **exercise 1** in https://coderefinery.github.io/documentation/sphinx/


### Exercise: Deploy Sphinx documentation to Read the Docs

In this exercise we will fork an example repository on GitHub and deploy it to Read the Docs. The example project contains a script for counting the frequency distribution of words in a given file and some documentation generated using Sphinx. For bigger projects, we can have more source files.

We will use GitHub for this exercise but it will also work with any Git repository with public read access.

Go to the [word-count project](https://github.com/coderefinery/word-count/generate) template on GitHub and fork it to your namespace.

#### Clone the repository
The repository contains following two folders, among few other files and folders:
* **source** folder contains the source code
* **doc** folder contains the Sphinx documentation
 
The doc folder contains the Sphinx configuration file (conf.py) and the index file (index.rst) and some contents (other RST files). The conf.py file has been adjusted to be able to autogenerate documentation from sources.

#### Build HTML pages locally
Inside the cloned repository, build the documentation and verify the result in your browser:
    
```sphinx-build doc _build ```

#### Test HTML pages links

Inside the cloned repository, check the integrity of all internal and external links:

```sphinx-build doc -W -b linkcheck -d _build/doctrees _build/html```

#### Enable the project on Read the Docs

**Import a project to Read the Docs by connecting to GitHub**

* Log into [Read the Docs](https://readthedocs.org/) and visit your [dashboard](https://readthedocs.org/dashboard/)
* Click “Import a Project”
* Select “Connect to GitHub”, and choose the word-count repository (if you don’t see this check your connections)
* Rename the project to a unique name (e.g. “youruser-word-count”)
* Click “Next”

#### Verify the result

That’s it! Your site should now be live on http://youruser-word-count.readthedocs.io (replace project name). Note that if your Git repo name contained underscores, they get converted to hyphens.

**Paste the link to your documentation behind your name in the collaborative document**

#### Verify refreshing the documentation

* Finally, make some changes to your documentation
* Add documentation related to other functions
* Prerequisites and how to use the program
* Rules for contribution
* Some example results (figures, tables, …)
* Commit and push them, and verify that the documentation website refreshes after your changes (can take few seconds or a minute)


### Hosting websites/homepages on Github pages (skipped)

- Write markdown files in your repository
- These files (and html files) will be deployed to a webpage for free!
- Exercise on this: [Hosting websites/homepages on Github Pages](https://coderefinery.github.io/documentation/gh-pages/)

### Questions to recap:
#### What questions do you still have?
- Q: can you document like this from a private repository? A: You can write, but you cannot host for free on RtD.

#### Are there any incremental improvements that can benefit your projects?
- API generated automatically provides a nice overview

#### What is nice that we learned but is overkill for your current work?
- full fledged RtD

### Take-home: documentation
- it is important to document code
- depending on the purpose and state of the project, documentation needs to meet different criteria


### Testing
- if your project is expected to last longer than 6 months, tests are worth the effort!
- Write small programs to run parts of your code, and verify the output
- Tests need: input, and reference to verify the output
- Unit tests test the small individual parts of your project
- Integration tests test the project more cohesively
- There Are Many Reasons To Test!
    - Preserve expected functionality, detect errors early on
    - Makes it easy to detect new errors early
    - Helps users confirm the code was installed correctly
    - Ensures reproducibility of the project and its derivatives
    - Facilitate refactoring of the code(= rewriting while maintaining functionality)
    - Help getting new developers on board by showing functionality, and preventing them from breaking the project (because then tests would show it)
    - Tests help manage complexity!
    - Tests are an important check for users: "If this package does not have tests, I will not use it."
    - You write tests while developing anyway! By formalizing them, you do not need to throw them away and you can reuse them in the future.
- Making sure you write tests:
    - Code review can help you develop tests, by someone else requesting or requiring them
    - CodeCov metrics (e.g.) tells you how much of your code is covered by tests (and guilts you into writing more)

Make a new file called `temperature_test.py`. Write code, and run it.
```python=
def fahrenheit_to_celsius(temp_f):
    """Convert temperature in Fahrenheit to Celsius
    """
    temp_c = (temp_f-32)*(5.0/9.0)
    return temp_c
```
Simply execute the function:
```python=
print(fahrenheit_to_celsius(temp_f = 100))
```
But it is better to use a testing framework.
```python=
import pytest

def test_fahrenheit_to_celsius():
    temp_c = fahrenheit_to_celsius(temp_f = 100)
    expected_result = 37.7777777
    assert abs(temp_c - expected_result) < 1.0e-6
```
Run this file using `pytest`:
```
pytest temperature_test.py
```
Tip! Comparing floating point numbers may cause inadvertent failure; thus, testing them like this is more fool-proof!

### Exercise

See also this [coderefinery github page](https://github.com/coderefinery/testing/blob/main/content/pytest.md)

In this exercise we will make a simple Python function and use
[pytest](http://doc.pytest.org) to test it.

* This is easy to use by almost any project and doesn't rely on any
  other servers or services.
* The downside is that you have to remember to run it yourself.

We will try to
keep things simple so that those who do not use Python can follow.

1. Create a new directory and change into it:
   ```bash=
   mkdir pytest-example
   cd pytest-example
   ```

2. Then create a file called `example.py` and copy-paste the following code into it:
   ```python=
   def add(a, b):
       return a + b


   def test_add():
       assert add(2, 3) == 5
       assert add('space', 'ship') == 'spaceship'
   ```
   This code contains one genuine function and a test function.
   `pytest` finds any functions beginning with `test_` and treats them
   as tests.

3. Let us try to test it with pytest:
   ```shell
   $ pytest -v example.py

   ============================================================ test session starts =================================
   platform linux -- Python 3.7.2, pytest-4.3.1, py-1.8.0, pluggy-0.9.0 -- /home/user/pytest-example/venv/bin/python3
   cachedir: .pytest_cache
   rootdir: /home/user/pytest-example, inifile:
   collected 1 item

   example.py::test_add PASSED

   ========================================================= 1 passed in 0.01 seconds ===============================
   ```
   Yay! The test passed!

   Hint for participants trying this inside Spyder or IPython: try `!pytest -v example.py`.

4. Let us break the test!
   Introduce a code change which breaks the code and check
   whether pytest detects the change:
   ```shell
   $ pytest -v example.py

   ============================================================ test session starts =================================
   platform linux -- Python 3.7.2, pytest-4.3.1, py-1.8.0, pluggy-0.9.0 -- /home/user/pytest-example/venv/bin/python3
   cachedir: .pytest_cache
   rootdir: /home/user/pytest-example, inifile:
   collected 1 item

   example.py::test_add FAILED

   ================================================================= FAILURES =======================================
   _________________________________________________________________ test_add _______________________________________

       def test_add():
   >       assert add(2, 3) == 5
   E       assert -1 == 5
   E         --1
   E         +5

   example.py:6: AssertionError
   ========================================================= 1 failed in 0.05 seconds ==============
   ```
   Notice how pytest is smart and includes context: lines that failed,
   values of the relevant variables.



 #### Optional exercise: Testing with numerical tolerance (5 min)
In the above exercise we have compared integers.  In this optional exercise we
want to learn how to compare floating point numbers since they are more tricky
(see also ["What Every Programmer Should Know About Floating-Point Arithmetic"](https://floating-point-gui.de/)).

The following test will fail and this might be surprising. Try it out:
   ```python
   def add(a, b):
       return a + b


   def test_add():
       assert add(0.1, 0.2) == 0.3
   ```

Your goal: find a more robust way to test this addition. #hint pytest.approx



### Testing with Continuous Integration
Running tests can be done locally, but also on the repository itself. For this, we continue on the Continuous Integration lesson from yesterday.

First, make sure a test is added to `example.py` on the repository:
```python=
def test_add():
  assert add(1,2)==3
```

Add pytest to your GitHub Actions workflow file (`/.github/workflows/python-app.yml`):
```yaml=
    - name: Test with pytest
      run: |
          pytest example.py
```

When you commit, the workflow will be triggered. Check Actions > Python Application to view the progress/results of your action.

### Exercise: Test design

Write tests for the following functions/classes. Also test the error condition:
```python=
#1
def factorial(n):
    """
    Computes the factorial of n.
    """
    if n < 0:
        raise ValueError('received negative input')
    result = 1
    for i in range(1, n + 1):
        result *= i
    return result


# 2
def count_word_occurrence_in_string(text, word):
    """
    Counts how often word appears in text.
    Example: if text is "one two one two three four"
             and word is "one", then this function returns 2
    """
    words = text.split()
    return words.count(word)


# 3
# Hint look at python tempfile module, specifically mkstemp
def count_word_occurrence_in_file(file_name, word):
    """
    Counts how often word appears in file file_name.
    Example: if file contains "one two one two three four"
             and word is "one", then this function returns 2
    """
    count = 0
    with open(file_name, 'r') as f:
        for line in f:
            words = line.split()
            count += words.count(word)
    return count


# 4
# Hint look at monkeypatching for functions
import time
def check_time_to_now_even(seconds):
    """
    Checks whether time difference between now and given time in seconds is even
    """
    if seconds < 0:
        raise ValueError('received negative input')
   
    now=time.time()
    return (seconds-now)%2 == 0


# 5
class Pet:
    def __init__(self, name):
        self.name = name
        self.hunger = 0
    def go_for_a_walk(self):  # <-- how would you test this function?
        self.hunger += 1
        
```
Some further advice:
- you can write multiple tests for the same function
- you can write multiple asserts in the same test
- this exercise would allow you to write tests in the same file, but usually you would separate:
    - source code and tests in two different directory, where the structure of the source code (i.e. folders) matches the structure of the tests
    - source code and tests in different files in the same directory. E.g. have a file called `test_XXX.py` testing the methods of `XXX.py` in that same directory.


### Solutions 

#### Ex. 1
```python=
def test_factorial():
    assert factorial(0) == 1
    assert factorial(1) == 1
    assert factorial(2) == 2
```

#### Ex. 2
```python=
def test_count_word_occurrence_in_string():
    assert count_word_occurrence_in_string('AAA BBB', 'AAA') == 1
    assert count_word_occurrence_in_string('AAA AAA', 'AAA') == 2
    # What does this last test tell us?
    assert count_word_occurrence_in_string('AAAAA', 'AAA') == 1
```

#### Ex. 3
```python=
import tempfile
import os

def test_count_word_occurrence_in_file():
    _, temporary_file_name = tempfile.mkstemp()
    with open(temporary_file_name, 'w') as f:
        f.write("one two one two three four")
    count = count_word_occurrence_in_file(temporary_file_name, "one")
    assert count == 2
    os.remove(temporary_file_name)
```

#### Ex. 4
```python=
def test_check_time(monkeypatch):
  def mocktime():
    return 2
  monkeypatch.setattr(time,"time",mocktime)
  assert check_time_to_now_even(0) == 1
  assert check_time_to_now_even(1) == 0
```

#### Ex. 5
```python=
def test_pet():
    p = Pet('asdf')
    assert p.hunger == 0
    p.go_for_a_walk()
    assert p.hunger == 1

    p.hunger = -1
    p.go_for_a_walk()
    assert p.hunger == 0
```


### Modular code
- Add building blocks to change the functionality of your code, instead of having to rewrite the whole thing
- Reusing components also facilitates reading/interpreting as you develop
- Modular code is an extra step: you write something, then make it modular
- What makes a good building block?
    - A clear interface
    - A good name
    - Testability (makes it reliable)
    - No side effects
    - No 'state' (should always do the same, regardless of how often I call it)
- How do we define the modules? How do we segment?
    - Write tests
    - Give good names (look for Kate Gregory, Naming is hard, let's do better)
    - Fail, and rewrite
    - Read books!
    - Read good code
    - Do not duplicate your code (instead: reuse!)
- Rules for complexity
    - Not too big
    - Not too small: blocks should not consist of too many sub-blocks
- Rules for consistency
    - Consistent formatting
    - Consistent naming
- Use existing libraries: many problems have already been solved
- Solve problems now, don't think ahead too much


### Exercise

Download data from [here](https://raw.githubusercontent.com/coderefinery/modular-type-along/master/data/temperatures.csv). Use right click -> "save link as"; or via the commandline:
```bash
wget https://raw.githubusercontent.com/coderefinery/modular-type-along/master/data/temperatures.csv
```

create a file `plot.py` with the following content
```python=
import pandas as pd
from matplotlib import pyplot as plt

num_measurements = 25

# read data from file
data = pd.read_csv('temperatures.csv', nrows=num_measurements)
temperatures = data['Air temperature (degC)']

# compute statistics
mean = sum(temperatures)/num_measurements

# plot results
plt.plot(temperatures, 'r-')
plt.axhline(y=mean, color='b', linestyle='--')
plt.savefig('25.png')
plt.clf()
```

Typing `python3 plot.py` in the terminal should create a file `25.png` with the output:
<img src="https://raw.githubusercontent.com/JensWehner/code-refinery-modcode/main/25.png" />
Change this code to make it more modular
Hints:
- make options more generic
- docstrings
- introduce version control
- use github
- unit_tests
- command line interface
- introduce functions
- improve plotting
- modules
- use a `main()` function to enable module import

Paste your code here and explain as a group what you did:


 #### Group2
 Modules:
```
def get_column (filename, num_measurements, column):
    """This method reads the column data within the file"""
    data = pd.read_csv(filename, nrows=num_measurements)
    column_info = data[column]
    return column_info

def compute_mean (data, n_samples):
    """This method computes the mean of the given data"""
    return sum(data)/num_measurements

def line_plot(data, mean):
    """Plot the given data againts its mean"""
    figure = plt.figure()
    plt.plot(data, 'r-', label = 'Temperatures')
    plt.axhline(y=mean, color='b', linestyle='--', label = 'Mean')
    plt.grid()
    plt.title("Temperature vs mean")
    plt.legend()
    plt.show()
    return figure

def save_plot(figure, fig_name):
    figure.savefig(fig_name)
```
Main: 
```
import pandas as pd
from matplotlib import pyplot as plt

if __name__ == '__main__':
    
    num_measurements = 25
    filename = 'temperatures.csv'
    column = 'Air temperature (degC)'
    column_info = get_column (filename, num_measurements, column)
    
    mean = compute_mean (column_info, num_measurements)
    
    figure = line_plot(column_info, mean)
    save_plot(figure, str(num_measurements)+'.png')
```
Test: 
```
import pytest

def test_get_column ():
    filename = 'temperatures.csv'
    column = 'Air temperature (degC)'
    num_measurements = 3
    
    result = get_column (filename, num_measurements, column)
    expected_result = [-0.2, -0.3, -0.7]
    assert list(result) == expected_result)
```


#### Our solution
See [the coderefinery instructor guide](https://coderefinery.github.io/modular-type-along/instructor-guide/)


## 📚 Resources

* [Documentation](https://coderefinery.github.io/documentation/)
* [Testing](https://coderefinery.github.io/testing/)
* [Modular code](https://coderefinery.github.io/modular-type-along/)
* [post-workshop survey](https://www.surveymonkey.com/r/RMPB3TP)
* [wikipedia's README page](https://en.wikipedia.org/w/index.php?title=README)
* [A curated list of awesome readmes](https://github.com/matiassingers/awesome-readme)
* [Hosting websites/homepages on Github Pages](https://coderefinery.github.io/documentation/gh-pages/)
* [Testing in Matlab](https://www.mathworks.com/help/matlab/matlab-unit-test-framework.html)
* [Kate Gregory: "Naming is hard, let's do better"](https://www.youtube.com/watch?v=MqugiGzricQ)
* [eScience Academy future courses](https://escience-academy.github.io/)