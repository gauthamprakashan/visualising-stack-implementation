# Visualising the Stack Implementation
This project will help you visualise the implementation of a Stack using array. We will be using various web technologies used in front-end to visualise these concepts in a webpage.

Check ``CONTRIBUTING.md`` for contributing guidelines


## Steps to follow to start Contributing :scroll:

### 0. Star The Repo :star2:

Star the repo by pressing the topmost-right button to start your wonderful journey.


### 1. Fork the repo :fork_and_knife:

You can get your own fork/copy of <a href="https://github.com/devclub-biet-jhansi/visualising-stack-implementation">Visualising Stack Implementation</a> by using the <kbd><b>Fork</b></kbd> button at top-right of your screen.


### 2. Clone it to your local machine :busts_in_silhouette:

`NOTE: commands are to be executed on Linux, Mac, and Windows(using Powershell)`

You need to clone (download) it to local machine using

```sh
$ git clone https://github.com/devclub-biet-jhansi/visualising-stack-implementation.git
```

> This makes a local copy of the repository in your machine.

Once you have cloned the `visualising-stack-implementation` repository in Github, move to that folder first using change directory command on Linux, Mac, and Windows(PowerShell to be used).

```sh
# This will change directory to a folder visualising-stack-implementation
$ cd visualising-stack-implementation
```

Move to this folder for all other commands.

Now Make your contribution on the project and commit your changes to a new branch

### 3. Create a new branch :bangbang:

Whenever you are going to contribute. Please create a separate branch using command and keep your `master` branch clean (i.e. synced with remote branch).

```sh
# It will create a new branch with name Branch_Name and switch to branch Folder_Name
$ git checkout -b BranchName
```

Create a separate branch for contribution and try to use the same name of the branch as of folder.

To switch to the desired branch

```sh
# To switch from one folder to other
$ git checkout BranchName
```

To add the changes to the branch. Use

```sh
# To add all files to branch Folder_Name
$ git add .
```

Type in a message relevant for the code reviewer using

```sh
# This message get associated with all files you have changed
$ git commit -m 'relevant message'
```

Now, Push your awesome work to your remote repository using

```sh
# To push your work to your remote repository
$ git push -u origin BranchName
```

Finally, go to your repository in the browser and click on `compare and pull requests`.
Then add a title and description to your pull request that explains your precious effort.

Always feel free to drop a comment or create an issue if you find something missing. Our excellent contributors will always get it done.
 
Happy Coding 🎉🎉







# Schema Design and Mentor Mentee Mapping

## 1. To Create the Mentor Mentee Mapping, we send the unique employee id(uuid v4) from the employees table as a foreign key relation to the mentor_id and mentee_id primary keys of the Mentor table. 
## 2. Each Mentor can have multiple mentees. This mapping is preserved as both the keys together form the primary key and each mentor can have multiple mentees.
## 3. Historical data can also be acceseed without overwriting or violating other constraints. We have start_date and end_date for the duration of the mentorship. The end_date can be set as NULL, for an ongoing mentorship.

# Key Components

## Mentor ID (mentor_id): Unique identifier for mentors, referencing the id field of the employees table.
## Mentee ID (mentee_id): Unique identifier for mentees, also referencing the id field of the employees table.
## Start Date (start_date): Marks the beginning of the mentorship.
## End Date (end_date): Indicates the conclusion of the mentorship (nullable for ongoing relationships).

