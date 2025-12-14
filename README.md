# Decolonizing Technology and Building the Small Internet

The goal of this workshop is to start rebuilding our capacity for imagining what technology can be.


## Small internet today

- [Monastery of Blamensir](https://blamensir.neocities.org/)
- [Count Kagurasuzu](https://swanchime.itch.io/count-kagura)
- [Neocities](https://neocities.org/)

## Setup

Currently the setup instructions assume that you have access to a Mac. I will add setup for Linux and Windows if there is demand.

### Track 1: Indiviual, deploy on personal neocities website

This track lets you download the skeleton code and start editing and publishing
your website right away with minimal setup.

1. Download this repository as a zip and unzip it.
2. Create a neocities account on https://neocities.org/
3. Edit your website and uplaod the html file.
4. You can start editing the your website from the neocities web editor.
    a. I find it nice to have one window with the editor and another with the website.
    b. To see your changes take place, you will need to refresh the page after you save.

### Track 2: Collaborative, deploy on webmar27.neocities.org

This track is a way for us to collaborate on the same website. Each person can
take on designing a card for a specific day of the advent calendar. We will
then merge these changes and can view them together.

#### Setting your editor
Some options you might want to consider:
1. Sublime Text - https://www.sublimetext.com/#light
2. VS Code - https://code.visualstudio.com/
3. VIM - https://www.vim.org/download.php

#### GitHub
1. Create a GitHub account. Github is a platform that allows you to store, share, and collaborate on code.
2. Install brew. Brew is a package manager that makes it easy to install and update software on your Mac. You can do this by running this command in your terminal:
    ```
    /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
    ```
3. Install GitHub CLI.
    ```
    brew install gh
    ```
4. Configure Git locally:
    ```
    git config --global user.name "Your Name"
    git config --global user.email "youremail@example.com"
    ```
5. Authenticate GitHub CLI. Follow the directions on the screen, I find it easiest to authenticate through the browser:
    ```
    gh auth login
    ```
6. Clone this repository:
    ```
    gh repo clone oalmatov/workshop
    ```
7. Start your own branch:
    ```
    git checkout -b <my-branch-name>
    ```
8. Run the website:
    ```
    python3 -m http.server 3000
    ```
9. Code!
10. When you're done, commit and push your changes to your branch:
    ```
    git add .
    git commit -m "Your commit message"
    git push origin <my-branch-name>
    ```
11. Ping Omar and he'll review your changes and merge them into the main branch. The changes will be deployed to webmar27.neocities.org/advent-calendar
