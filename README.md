# macOS Terminal Cheat Sheet

Personal project (WIP) by Fabiano Araujo to help with macOS command line interface (CLI). 

🚧 WIP 🚧

# Index

- [General](#general)
- [Docker](#docker)
- [Git](#git)
- [GitHub](#github)
- [Virtual Environment](#virtual-environment)

## General
- `awk`: Processing structured text, like tables or databases.
- `cat filename`: Concatenate file contents.
- `cd`: Change directory (`/` = root folder; `..` = one level up).
- `clear`: Clear the terminal screen.
- `echo`: Display a line of text/string.
- `grep`: Search for patterns in text.
- `ls`: List files in directory.
- `mkdir`: Make a new directory.
- `rm -rf`: Remove directory recursively and forcefully.
- `sudo su`: Switch to the root user (administrative privileges).
- `tab`: Autocomplete command.

### Keyboard Shortcuts
- `Ctrl + U`: Deletes from the cursor to the beginning of the line.
- `Ctrl + K`: Deletes from the cursor to the end of the line.
- `Ctrl + W`: Deletes the word before the cursor.
- `Alt + D`: Deletes the word after the cursor (only in some terminals).
- `Ctrl + A`: Move cursor to the beginning of the line.
- `Ctrl + E`: Move cursor to the end of the line.
- `Ctrl + H`: Delete the character before the cursor (Backspace).
- `Ctrl + D`: Delete the character under the cursor or close the terminal if the line is empty.

## Docker
- `Ctrl-PQ`: Exit a container without terminating its main process.
- `docker build -t <repository>:<tag>`: Build a container.
- `docker buildx`: Docker CLI plugin to support multi-arch builds.
- `docker exec -it <repository>:<tag>`: Run a command in a running container.
- `docker history`: Show the history of an image.
- `docker image prune`: Remove unused images.
- `docker images`: List images.
- `docker inspect`: Gives the details of an image.
- `docker manifest inspect`: Inspect the manifest list of any image stored on Docker Hub.
- `docker pull <repository>:<tag>`: Pull an image or a repository.
- `docker ps`: List running containers. `-a` flag lists exited containers.
- `docker rm <repository>:<tag>`: Remove a container.
- `docker rmi image_name`: Remove an image.
- `docker rmi $(docker images -q) -f` Delete all images.
- `docker run -it <repository>:<tag> <app>`: Run an app in a container. `--it` flag connect the current terminal window to the container's shell.
- `docker run -d --name web1 --publish 8080:8080 <repository>:<tag>`: Run a web container.
- `docker start`: Start a container.
- `docker stop <repository>:<tag>`: Stop a running container.
- `docker version`: Show the Docker version information.

## Git
- `git add .`: Stages all changes in the repository.
- `git clone https://github.com/...`: Clone a repository.
- `git commit -am "Comments"`: Commit changes with a message.
- `git init`: Initialize a local Git repo.
- `git push origin main`: Push changes to the main branch.
- `git remote add origin <repo-url>`: Connect to a GitHub repo.
- `git rm -r --cached *__pycache__/`: Remove files or folders from remote repo.

## GitHub
- `gh repo create <repo-name> --private --clone`

## IDE
- `code .`: Open current directory in VS Code.

## Virtual Environment
- `pip freeze > requirements.txt`: Generate a requirements file.

### Base Python 
- `python -m venv venv`: Create virtual environment
- `source venv/bin/activate`: Activate environment
- `deactivate`: Deactivate environment

### Mistral UV
- `uv venv`: Create a virtual environment at .venv.
- `source .venv/bin/activate`: activate the virtual environment
- `deactivate`: deactivate environment

