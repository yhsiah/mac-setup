# Mac Setup Helper

## What is this?

As someone who works in tech, I need to set up a fresh macbook for myself once every so often when starting a new job, or getting a new laptop. This is a set of guidance notes to help make that process easier for myself, and maybe even others who might find this useful.

I will attempt to keep this setup guide minimal and simple, and not add anything unneccessary. I also intend to automate some of this process at some point.

For reference, I am a QA Engineer and so you may find this to be slightly oriented towards that.

## First Booting the MacBook (WIP)

Run through the setup and sign in using your Apple ID.

When asked if you would like to user FileVault to encrypt the disk, say yes. There is no harm in doing so with a modern MacBook, there is no performance loss and it renders your laptop useless if you lose it. Some companies will require you to have this turned on.

## Some quick tips for new Macbook users

If you came from using Windows, like myself a few years ago - here's some quick tips to help with your productivity.

### Spotlight Search is your friend

Use spotlight search for everything. Think of it as the start menu in windows.

Open it by pressing `⌘ command` and `space` at the same time. You can type in names of apps/programs, file names, folders etc. and launch them by tapping `enter`. You can even do calculations in here.

### Use Multiple Desktops

With macOS you can use multiple desktops and switch between them easily. Think of it like swiping between screens on your smart phone.

You can do this by using the built-in gestures on the trackpad. Swipe up using 3 fingers. This puts you in `Mission Control` view, showing all your open windows.

You can use `Mission Control` to click and switch between different windows, and you can also move your cursor up to the top of the view to add desktops and switch between them. You can also click and drag windows to place them in other desktops.

When out of the `Mission Control` view, you can use a 3 finger swipe on the trackpad, left or right, to switch between your desktops.

Also note that maximising a window in MacOS fills the entire screen and acts like an additional desktop.

## Other notes about using MacOS

The `⌘ command` key is used for everything the `control` key is usually used for in a Windows machine. Copy is `⌘ command` + `c` and paste is `⌘ command` + `v`.

The touchbar is fairly pointless, but looks cool I guess.

## Setting up (WIP)

- Open Terminal
- Install homebrew with `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"`
- Use homebrew to install the usual suspects (in general, `cask` is used to install anything with a UI, otherwise a normal bres install is used)
    - `brew install git` for git
    - `brew install node` for node js / npm
    - `brew install nvm` for node version manager
    - `brew install zsh` for zsh
    - `brew cask install chrome` for google chrome
    - `brew cask install spotify` for spotify
    - `brew cask install visual-studio-code` for vscode
    - `brew cask install postman` for postman
- Install Oh My Zsh with `sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`
- Make the terminal pretty with themes (TODO)

Other useful things:
- install xcode from the app store, if you want to be able to use Simulator to run emulated mobile ios devices
- install spectacle for a nice way and easy to manage windows (although note this is no longer maintained, but still works fine). You can install this with `brew cask install spectacle`. Shortcuts with spectacle:
    - `option + cmd + f` to maximise the window without making it go fullscreen.
    - `option + cmd + left arrow` for moving a window to the left half of your desktop.
    - `option + cmd + right arrow` for moving a window to the right half of your desktop.
    - You can see all the available shortcuts by clicking the spectacle icon in the top corner of your screen when it is running.

## Setting up Git (WIP)

- generate a new ssh key
- add it to your github account
- add the new work email to your github as a secondary email address
- set your git config on your machine with `git config --global user.name <username>` and `git config --global user.email <email>`, and set differently per work repo using `git config user.email <work-email>` while in the repo, if you'd like.

## Notes on your bash profile / zsh profile (TODO)
