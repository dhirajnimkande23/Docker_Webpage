# Docker_Webpage
Dockerize Apache WebPage 



Here's a **documented explanation** of each of the commands you provided. These commands involve **Docker** and **Git** operations, commonly used in deploying and version-controlling applications.

---

## 🐳 Docker Commands

### 1. **Build a Docker Image**

```bash
docker build -t dhiraj23/webpage .
```

* `docker build`: Command to build a Docker image.
* `-t dhiraj23/webpage`: Tags the image with the name `dhiraj23/webpage`.
* `.`: Refers to the current directory as the build context (where the `Dockerfile` is located).

✅ **Purpose**: Create a Docker image from your local code and Dockerfile.

---

### 2. **List Docker Images**

```bash
docker images
```

* Shows a list of locally available Docker images on your machine.
* Displays image name, tag, image ID, creation time, and size.

✅ **Purpose**: Verify if your image (`dhiraj23/webpage`) was built successfully.

---

### 3. **Log in to Docker Hub**

```bash
docker login
```

* Prompts for your Docker Hub **username** and **password**.
* Authenticates your local Docker CLI to interact with Docker Hub.

✅ **Purpose**: You must be logged in to push images to your Docker Hub repository.

---

### 4. **Push Docker Image to Docker Hub**

```bash
docker push dhiraj23/webpage:latest
```

* `docker push`: Uploads the image to Docker Hub.
* `dhiraj23/webpage:latest`: The image name and tag you're pushing.

✅ **Purpose**: Share your Docker image online so others can pull and run it.

---

## 🧑‍💻 Git Commands

### 5. **Check Installed Git Version**

```bash
git --version
```

* Displays the currently installed version of Git.

✅ **Purpose**: Ensure Git is installed and accessible on your system.

---

### 6. **Set Git Username (Global)**

```bash
git config --global user.name "dhiraj"
```

* Sets your Git global username to `"dhiraj"`.

✅ **Purpose**: Identifies you in your commits across all repositories.

---

### 7. **Set Git Email (Global)**

```bash
git config --global user.email "email address"
```

* Sets your Git global email address.

✅ **Purpose**: Associates your email with your commits (important for GitHub).

---

### 8. **List Git Configuration**

```bash
git config --list
```

* Displays all current Git configuration settings.

✅ **Purpose**: Verify that your Git username, email, and other settings are correct.

---

## Summary Table

| Command                          | Description                   |
| -------------------------------- | ----------------------------- |
| `docker build -t name .`         | Build Docker image with a tag |
| `docker images`                  | List Docker images            |
| `docker login`                   | Authenticate with Docker Hub  |
| `docker push name:tag`           | Push image to Docker Hub      |
| `git --version`                  | Check Git version             |
| `git config --global user.name`  | Set global Git username       |
| `git config --global user.email` | Set global Git email          |
| `git config --list`              | View current Git settings     |





---

## 📦 Commands Breakdown: Git & File Management

---

### 1. **Clone a GitHub Repository**

```bash
git clone https://github.com/dhirajnimkande23/Docker_Webpage.git
```

* Downloads the repository from GitHub to your local machine.
* The directory `Docker_Webpage` is created with all repo contents.

✅ **Purpose**: Start working with a remote project locally.

---

### 2. **Change Directory into Cloned Repo**

```bash
cd Docker_Webpage/
```

* Navigates into the cloned project directory.

✅ **Purpose**: Start working inside your cloned repository.

---

### 3. **Move Files into a Subdirectory**

```bash
mv Dockerfile nano.tar.gz Docker_Webpage/
```

* Moves `Dockerfile` and `nano.tar.gz` into a subdirectory called `Docker_Webpage/`.

✅ **Purpose**: Organize project files inside a specific folder.

> ⚠️ Note: If `Docker_Webpage/` is already your current directory, and there's a subfolder also named `Docker_Webpage/`, this can cause confusion. Double-check the folder structure.

---

### 4. **Change Directory Again**

```bash
cd Docker_Webpage/
```

* Moves into the inner `Docker_Webpage/` directory (if this exists).

✅ **Purpose**: Continue working from within the new directory where files were moved.

---

### 5. **Check Git Status**

```bash
git status
```

* Shows the current state of the working directory:

  * Untracked files
  * Changes staged for commit
  * Changes not staged

✅ **Purpose**: See what changes have been made or need to be committed.

---

### 6. **Stage a File for Commit**

```bash
git add Dockerfile
```

* Stages the `Dockerfile` to be committed.

✅ **Purpose**: Tells Git to include this file in the next commit.

---

### 7. **Commit with a Message**

```bash
git commit Dockerfile -m "apache2 dockerfile"
```

> ⚠️ **Note**: This command is **incorrectly structured**.

* The correct format should be:

```bash
git commit -m "apache2 dockerfile"
```

* If you’ve already used `git add Dockerfile`, Git knows what to commit.
* `Dockerfile` should **not** be placed between `commit` and `-m`.

✅ **Fix**:
Use:

```bash
git commit -m "apache2 dockerfile"
```

---

### 8. **Stage Multiple Files**

```bash
git add Dockerfile nano.tar.gz
```

* Stages both files for commit.

✅ **Purpose**: Prepare both files to be saved in Git history.

---

### 9. **Check Git Status Again**

```bash
git status
```

* Verifies that both files are staged and ready for commit.

---

### 10. **Commit All Staged Files**

```bash
git commit -m "webpage"
```

* Commits the staged changes with the message `"webpage"`.

✅ **Purpose**: Save your changes to the local Git history.

---

### 11. **Push Changes to GitHub**

```bash
git push origin main
```

* Pushes your commits to the remote `origin` (i.e., GitHub).
* Sends them to the `main` branch.



📦 Commands Breakdown: Git & File Management
1. Clone a GitHub Repository
git clone https://github.com/dhirajnimkande23/Docker_Webpage.git


Downloads the repository from GitHub to your local machine.

The directory Docker_Webpage is created with all repo contents.

✅ Purpose: Start working with a remote project locally.

2. Change Directory into Cloned Repo
cd Docker_Webpage/


Navigates into the cloned project directory.

✅ Purpose: Start working inside your cloned repository.

3. Move Files into a Subdirectory
mv Dockerfile nano.tar.gz Docker_Webpage/


Moves Dockerfile and nano.tar.gz into a subdirectory called Docker_Webpage/.

✅ Purpose: Organize project files inside a specific folder.



4. Change Directory Again
cd Docker_Webpage/


Moves into the inner Docker_Webpage/ directory (if this exists).

✅ Purpose: Continue working from within the new directory where files were moved.

5. Check Git Status
git status


Shows the current state of the working directory:

Untracked files

Changes staged for commit

Changes not staged

✅ Purpose: See what changes have been made or need to be committed.

6. Stage a File for Commit
git add Dockerfile


Stages the Dockerfile to be committed.

✅ Purpose: Tells Git to include this file in the next commit.

7. Commit with a Message
git commit Dockerfile -m "apache2 dockerfile"


⚠️ Note: This command is incorrectly structured.

The correct format should be:

git commit -m "apache2 dockerfile"


If you’ve already used git add Dockerfile, Git knows what to commit.

Dockerfile should not be placed between commit and -m.

✅ Fix:
Use:

git commit -m "apache2 dockerfile"

8. Stage Multiple Files
git add Dockerfile nano.tar.gz


Stages both files for commit.

✅ Purpose: Prepare both files to be saved in Git history.

9. Check Git Status Again
git status


Verifies that both files are staged and ready for commit.

10. Commit All Staged Files
git commit -m "webpage"


Commits the staged changes with the message "webpage".

✅ Purpose: Save your changes to the local Git history.

11. Push Changes to GitHub
git push origin main


Pushes your commits to the remote origin (i.e., GitHub).

Sends them to the main branch.

✅ Purpose: Share your updated project with collaborators or deploy from GitHub.

📄 Summary Table
Command	Description
git clone URL	Clone repo from GitHub
cd folder/	Change into project directory
mv file1 file2 dir/	Move files into a directory
git status	Show changes and untracked files
git add file	Stage file for commit
git commit -m "msg"	Commit staged changes
git push origin main	Push changes to main branch on GitHub




