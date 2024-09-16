# Push Repository
This repository was made locally for the purpose of adding to GitHub remotely.
## Creating a local repository
<details>
<summary>how to create a local repository</summary>
  First we must create a new directory and initialise it as a Git repository before we can add it to GitHub.

  1. Using bash create a new directory
  ```sh
  mkdir <my new repository>
  ```
  2. Navigate into the new directory
  ```sh
  cd <my new repository>
  ```
  3. Initialise the directory as a Git repository with default branch **main**
  ```sh
  git init -b main
  ```
  4. Create a new file
  ```sh
  echo "Welcome to my new repository" > README.md
  ```
  5. Add the file to be tracked by Git
  ```sh
  git add README.md
  ```
  6. Create a commit for our new file
  ```sh
  git commit -m "created README"
  ```
</details>

## Adding the repository to GitHub
Now that we have created our repository we can go ahead and add it to GitHub.

1. Add GitHub as our remote origin for the repository
 ```sh
 git remote add origin https://github.com/<GitHubUsername>/<my_new_repository>.git
 ```
2. Push your repository to the remote origin we just set at GitHub.
 ```sh
 git push -u origin main
 ```
3. Set a personal access token and copy it somewhere safe if you have not.
4. Enter GitHub username and access token when prompted.
