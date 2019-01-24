# Homework Grading Scripts
--

Simple scripts to automate a bit of the homework grading process for instructors and TA's.

Scripts include:
```batch_submit_issues.sh```

## batch_submit_issues.sh

This script will batch submit the homeowrk grading issues for all github repos (student homework repos) in the current path.

### Installation

The shell script relies on the ``` github/hub ``` tool to create issues by command line. Follow the [installation instructions] (https://github.com/github/hub) found at their github page to install the tool on your device.

User documentation for the Hub tool can be found [here] (https://hub.github.com/hub.1.html). It extends many git commands and also provides new commands of its own.

### Usage

1. Download all the homework repos to your local machine. When grading the homework, modify the ```ISSUE_TEMPLATE.md``` file in each repo rather than making an issue through the github webiste.
2. Copy ```push_hw_issues.sh``` into the parent directory of all the homework repos.
3. Modify the ```title``` variable in the shell script as the issue title you want to specify, e.g. "SEDS HW 1 Grade".
4. Once you are ready to send out the issues to _all_ the students, simply run the shell script.  
_NOTE: the hub command for creating issues will automatically copy the url of the new issue to your computer's clipboard. This can be avoided by using the alternative command provided in the script. However, you will get an error as the function tries to print the url to your terminal. The issue will still be created, but it will print the url and followed by 'No such file or directory'._

