# Strategic Communications Developer Onboarding

This document serves as a semi-comprehensive setup for new developers working on code based projects under the stewardship of the Department of Web Communications. **It assumes starting with a factory reset computer** running Mac OSX, please skip steps as needed if you already have a partially configured system.

Before we begin, you must have a GitHub account. If you do not already have one, we recommend you create an account with your personal email address and use it for all of your activity on GitHub. We do not monitor your activity on the platform and your contributions to all UA projects will be credited to you personally.

## Install Dependencies

1. Install Git by running `xcode-select --install`
2. Install [homebrew](https://brew.sh/)
3. Install the GitHub CLI `brew install gh`
4. Install Node `brew install node`
5. Install PHP `brew install php`
6. Install composer `brew install composer`

## Git Configuration

1. Set your name in Git to match your full name or GitHub username.
2. Set your email to the **same email you use for GitHub**

Run each line one at a time.

```sh
git config --global user.name "Your Name"
git config --global user.email "you@email.com"
```

Optional configuration. Run each line one at a time.

```sh
git config --global checkout.defaultRemote "origin"
git config --global core.trustctime "false"
git config --global core.precomposeunicode "false"
git config --global core.untrackedCache "true"
git config --global diff.renames "copies"
git config --global fetch.prune "true"
git config --global fetch.pruneTags "true"
git config --global init.defaultBranch "main"
git config --global push.autoSetupRemote "true"
```

## SSH Setup

GitHub has more robust documentation on setting up an SSH key and configuring it for use with GitHub specifically.

- [Connecting to GitHub with SSH](https://docs.github.com/en/authentication/connecting-to-github-with-ssh)
- [Authorizing SSH for use with SAML SSO](https://docs.github.com/en/enterprise-cloud@latest/authentication/authenticating-with-saml-single-sign-on/authorizing-an-ssh-key-for-use-with-saml-single-sign-on)

## Authenticating with GitHub

Run `gh auth login` and follow the prompts for browser based authentication, then test to ensure the authentication was successful by running `gh auth status`. It should give a message similar to the following:

```txt
✓ Logged in to github.com as YourUsername (oauth_token)
✓ Git operations for github.com configured to use https protocol.
✓ Token: *******************
```

You can double check by cloning a repository from the organization and making a commit. The commit should be linked to your GitHub account.

## Software

- [UA VPN](https://oit.ua.edu/services/internet-networking/vpn/)
- [Docker](https://www.docker.com/)
- [Bruno](https://www.usebruno.com/)
- [Microsoft Remote Desktop](https://apps.apple.com/us/app/microsoft-remote-desktop/id1295203466?mt=12)

While not required, it is recommended to use [Visual Studio Code](https://code.visualstudio.com/) and the following extensions:

- [Comment Anchors](https://marketplace.visualstudio.com/items?itemName=ExodiusStudios.comment-anchors)
- [GitHub Markdown Preview](https://marketplace.visualstudio.com/items?itemName=bierner.github-markdown-preview)

More extentions may be required / recommended by repositories

### Broswers

You may use whatever browser you want but you must have the ability to test on Chrome, Firefox, and Safari

You may find these extensions helpful

- WAVE Accessibility [Firefox](https://addons.mozilla.org/en-US/firefox/addon/wave-accessibility-tool/) | [Chrome](https://chromewebstore.google.com/detail/wave-evaluation-tool/jbbplnpkjmmeebjpijfedlgcdilocofh)
- React dev tools [Firefox](https://addons.mozilla.org/en-US/firefox/addon/react-devtools/) | [Chrome](https://chromewebstore.google.com/detail/react-developer-tools/fmkadmapgofadopljbjfkapdkoienihi)

## Recommended organization

It can be helpful to create a folder to store most repositories you're working on in one place. We recommend using a "Developer" folder in your home directory.

1. Create a "Developer" folder in your home folder
2. Inside "Developer" create a folder called "wordpress"
3. Inside "wordpress" create two folders named "themes" and "plugins"
4. Inside the "themes" folder, clone the theme repositories
5. Inside the "plugins" folder, clone the plugin repositories
6. Inside the "Developer" folder, create a folder called "sites" This is where you'll clone any sites from Pantheon
7. Inside the "Developer" folder, you may also clone any other repository or clone them in subfolders of your preference

To get child themes to work, download the latest version of theme 3 from <https://alabama.box.com/s/f3os9nh59u5ie4hppdxo536po2ybto96> and unzip it into the "themes" folder
