# Adding files to GIT

## Identify the two main GIT project sections
  ### Git directory
  1. The .git folder
  2. Folder is created when you run the "git int" command
  3. It is the GIT repository
  4. The .git directory
      - Tracks your changes
      - Stores commit objects
      - Stores GIT configurations
  ### GIT Working Tree
  1. Files and subdirectories on your file system that are associated with a repository
  2. Contains the files of the current branch
  3. Files are retrieved from the compressed database in the .git folder
  4. Files are placed on disk ready for use or modification
  
## Identify the three states of data in GIT
- Committed
  - Data is considered committed when it is stored in your GIT database
- Modified
  - Means that changes have been made to files in the working tree but have not yet been committed.
- Staged
  - Refers to files that have been modified AND have been marked to be part of the next commit snapshot.
  
## Add files using the "add" and "commit" commands
- Step 1: Create/Add a file to the GIT Working Tree.
- Step 2: Add the file to the Staged list
  - $ git add [filename] (Adds only the specific file you named)
  - $ git add [directory] (Adds all changed files in the specified directory)
  - $ git add -A (Adds all changed files in the entire project)
- Step 3: Commit the Staged files
  - $ git commit (Commits all files in the Staged list)
  - $ git commit -a (Stages and commits all changed files. performs Steps 2 and 3 together)
  
## Useful GIT Commands
- $ git status (Gives you the status of the project including a list of files staged and untracked)
- $ git reset (Removes a file or files from the Staged list)
- $ git diff (Shows any changes made to committed files)
- $ git commit -m
  - Adds a commit message to the commit
  - In most organizations a commit message is a requirement.
- $ git log (List commands made to the repository in reverse chronological order)
