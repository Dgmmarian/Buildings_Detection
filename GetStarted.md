# Get Started

This guide will help you get started with our project.

## Prerequisites

- Install Git on windows https://git-scm.com/download/win
  then you can use the following command to clone repository locally and start working on the project on vscode
- Install Python 3.7 or higher
- Install required packages

## Clone the repository localy

To clone the repository, run the following command
```
git clone https://github.com/DataScientest-Studio/py_construction_illegales
```

## Install dependencies (not implemented yet, don't run)

Install the required dependencies using the following command (venv opened):
```
pip install -r requirements.txt
```

## Go to your cloned repository folder before running any git commands

```
cd C:\path\to\your-repo-name
```

## Pull the changes before working on the project or before push changes

```
git pull origin main
```

## Save the file and commit the changes to your Git repository:

```
git add GetStarted.md
git commit -m "NAME_YOUR_COMMIT"
git push
```




## Folder Structure

```
py_construction_illegales/
│
├── .vscode/                   # Visual Studio Code settings folder
│   ├── settings.json          # Project-specific settings for VSCode
│
├── data/                      # Data storage folder
│   ├── raw/                   # Raw, unprocessed data
│   ├── processed/             # Processed data ready for modeling
│   └── external/              # External data sources, if applicable
│
├── src/                       # Source code folder
│   ├── data_preprocessing/    # Data preprocessing code
│   │   ├── __init__.py        # Package initializer
│   │   ├── preprocessing.py   # Preprocessing functions
│   │   └── augmentation.py    # Data augmentation functions
│   ├── model/                 # Model-related code
│   │   ├── architecture/      # Model architecture code
│   │   │   ├── __init__.py    # Package initializer
│   │   │   └── architecture.py # Model architecture definition
│   │   ├── checkpoints/       # Model checkpoint storage
│   │   ├── __init__.py        # Package initializer
│   │   ├── training.py        # Model training functions
│   │   └── utils.py           # Utility functions for model management
│   ├── inference/             # Inference-related code
│   │   ├── __init__.py        # Package initializer
│   │   ├── predict.py         # Prediction functions
│   │   └── evaluation.py      # Model evaluation functions
│   └── visualization/         # Visualization code
│       ├── __init__.py        # Package initializer
│       ├── data_viz.py        # Data visualization functions
│       └── results_viz.py     # Results visualization functions
│
├── notebooks/                 # Jupyter Notebooks folder
│
├── output/                    # Output storage folder
│   ├── figures/               # Visualizations and plots
│   ├── results/               # Evaluation results and metrics
│   └── predictions/           # Model predictions
│
├── docs/                      # Documentation folder
│
├── .gitignore                 # Specifies files and folders to be ignored by Git
├── README.md                  # Overview and instructions for the project
├── requirements.txt           # Lists project dependencies and their versions
└── setup_venv.sh              # Shell script to automate setting up venv and installing dependencies
```

## Usefull Git commands

```
# Clone a remote repository from GitHub to your local machine
git clone repository_url

# Add all changes, including new files and modifications, to the staging area
git add .

# Commit the changes with a descriptive message
git commit -m "Descriptive message here"

# Push the changes to the remote repository on GitHub
git push

# Fetch the changes from the remote repository and merge them with the local branch
git pull origin main

# Check the status of your local repository, including staged, unstaged, and untracked changes
git status

# View the commit history of your local repository
git log

# Show the differences between the working directory and the latest commit
git diff

# Create a new branch
git checkout -b new_branch_name

# Switch to an existing branch
git checkout branch_name

# Merge changes from one branch into another
git merge source_branch_name

# Fetch the latest changes from the remote repository without merging
git fetch

# List all branches, both local and remote
git branch -a

# Delete a local branch
git branch -d branch_name

# Delete a remote branch
git push origin --delete branch_name

# Stash the changes in your working directory for later use
git stash

# List all stashed changes
git stash list

# Apply stashed changes to your working directory
git stash apply stash@{stash_number}

# Create and switch to a new branch starting from a specific commit
git checkout -b new_branch_name commit_hash

# Revert changes from a specific commit (creates a new commit)
git revert commit_hash

# Reset the working directory to a specific commit and discard all changes
git reset --hard commit_hash

