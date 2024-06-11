# Project Managment API

## Description
- a web application designed to manage project progress between clients and executors, using a chess clock-like timer to monitor responsibilities and time spent on tasks.

## Instalation

```bash
    git clone https://github.com/georgetoloraia/Management_Backend.git
    cd managment_project
    pip install -r requirements,txt
    python manage.py migrate
    python manage.py runserver

    if using virtual env | venv/Source/activate or research in web
```

## Contributing
Contributors should follow these guidelines to create and manage branches for their tasks:

1. **Create Your Branch**:  
Each contributors should create their own branch and name it according to the task they are working on. For example, if you are working on the timer functionaly, you might name your branch `timer-functionality`,
- **command for create branch**
```bash
    git checkout -b timer-functionality
```

2. **Create Separate Applications for Separate Tasks:

For better organization and modularity, create separate Django applications for separate tasks, Use Django's `startapp` command to create a new application for your task:

- command:

```bash
    python manage.py atartapp <app_name>
```
Replace `<app_name>` with the name of the application relevant to your task. for example:
```bash
    python manage.py atartapp timer
```

3. Make Your Changes:

work on your task within the separate application. Make sure add `Documentation` for your changes.

4. Commit Your Changes:

After Changes commit:

```bash
    git add .
    git commit -m "add commit message"
```

5. Push your Branch:

```bash
    git push origin timer-functionality
```

6. Merge ehith the Main Branch:

When your task is completed and reviewed, merge you branch with the main branch. Follow these step:

1. Ensure you are on the `main` branch and it is up to date:

```bash
    git checkout main
    git pull origin main
```

2. Merge your branch eith the `main` branch:

```bash
    git checkout main
    git merge timer-functionality
```

3. Reslove any merge conflicts if they are.

4. Push the uptadet `main` branch to the remote repository:

```bash
    git push origin main
```
