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
git config --global user.email "dhirajnimkande23@gmail.com"
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

Let me know if you want this turned into a PDF, Markdown file, or something else.

