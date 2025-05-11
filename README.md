# Productive Git Commit Helper

A simple script to streamline your Git workflow. It helps you quickly stage changes, write a commit message, and push to your repository — all in one step.

## 🔧 What it does

This script:

1. Stages all your changes (`git add .`)
2. Prompts you to enter a commit message
3. Commits with the provided message
4. Pushes to the remote repository

## 💻 Usage

```bash
@read -p "Enter commit message: " msg; git add .; git commit -m "$msg"; git push

🧠 Why use this?

This tool is perfect for:

    Solo developers or small teams

    Fast prototyping and frequent commits

    Reducing typing overhead during the dev cycle

```

✅ Example
Enter commit message: Add README and basic git script
✅And it will do:
git add .
git commit -m "Add README and basic git script"
git push

📂 How to set up

1. As an alias (bash/zsh)

Add this line to your ~/.bashrc or ~/.zshrc:
alias gpush='read -p "Enter commit message: " msg; git add .; git commit -m "$msg"; git push'

Then run:
source ~/.bashrc # or ~/.zshrc
Now, simply use:
gpush

🧑‍💻 Contributing

Feel free to fork, improve or suggest changes via pull request. Let's help developers stay in flow. ⚡

if you are newbie
just create Makefile in your project folder
and add this script to it:
commit:
@git add .
@read -p "Enter commit message: " msg; \
 git commit -m "$$msg"; \
 git push

then every time you want to make commit, write in terminal:
make commit (press enter)
