# Integration of git with github

## 1. Create a GitHub Account

If you don't already have a GitHub account, you'll need to create one at https://github.com/.

## 2. Install Git

If Git is not already installed on your computer, download and install it from the official Git website (https://git-scm.com/).

## 3. Configure Git

After installing Git, you need to configure your identity with the following commands. Replace "Your Name" and `your@email.com` with your actual name and email address.

    git config --global user.name "Your Name"
    git config --global user.email "your@email.com"

    git config --global user.name "Sahil Alam"
    git config --global user.email "sahilalam.iitm@gmail.com"

## 4. Generate SSH Key (Optional, but recommended)

To securely connect to GitHub, it's a good practice to use an SSH key. You can generate one using the following command:

    ssh-keygen -t rsa -b 4096 -C "your@email.com"
    
    ssh-keygen -t rsa -b 4096 -C "sahilalam.iitm@gmail.com"

This command generates an SSH key pair. You can then add your public key (usually located in ~/.ssh/id_rsa.pub) to your GitHub account by going to GitHub Settings > SSH and GPG keys.

## 5. Create a GitHub Repository

Login to your GitHub account and click on the "+" button in the upper right corner to create a new repository. Follow the instructions on the GitHub website to create a repository.

## 6. Clone the GitHub Repository

To start working with an existing GitHub repository, you need to clone it to your local machine. Use the following command, replacing username and repository with your GitHub username and repository name:

    git clone git@github.com:username/repository.git

## 7. Make Changes and Commit

Create or edit files in the local repository, then use Git to stage and commit your changes:

    git add .
    git commit -m "Your commit message"

## 8. Push Changes to GitHub

To update the repository on GitHub, push your changes:

    git push origin master

This command pushes your local changes to the master branch on GitHub. You can replace master with the name of your branch if you are working on a different branch.

## 9. Pull Changes from GitHub

To retrieve the latest changes from GitHub, use the git pull command:

    git pull origin master

## 10. Collaborate with Others

You can invite collaborators to your GitHub repository and manage permissions through the repository settings on the GitHub website.
