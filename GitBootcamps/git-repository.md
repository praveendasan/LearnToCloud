# GIT Repository

## A GIT repository is like a project in other Version control system(VCS)
- A data structure used to manage files and changes over time for a project
- Stored in a single parent folder on your local system
- Contains files and data associated with that specific project

## Two Types of Content
- Files associated with the project
- GIT repository data
  - Stored in the .git folder(all metadata is store here)
  - Repository objects
  - Repository history
  - Repository configurations
- ***Repositories ALWAYS exist locally.***
## Create repository
- Step 1: Create a new project folder on your local system
  - Be mindful about permissions when choosing where to create my folder.
- Step 2: From inside the new project folder run the command "git init"
  - "git init" command create the .git folder inside your project folder
  - Don't edit files inside .git folder, all repository objects live inside this folder.
  - Yet we can edit few files in .git folder
    - description file - stores the name and descritpion of the repository.
    - config file - stores the project/repository specific setting. edit this file using repository configuration tools
    - hooks folder - stores hook scripts which allow for custom git action
## Git Command
- $ git init (Initialized empty Git repository in '\\location\\.git\\')
- navigate to .git folder, inside we can see files config, description, HEAD, hooks/, info/, objects/ refs/

## Clone an Existing Repository
- Step 1: Navigate to a folder on your local system where you want to download and be mightful on folder permission
- Step 2: run the command "git clone"
  - git clone <url to existing repository>
  - if you want to project folder to be different using git clone <url> <new_folder_name>
- Clone is not checkout
  - Pulls down a complete copy of the repository
  - Checkout contains a complete project history.
