
xcode-select --install

https://github.com/conda-forge/miniforge - Miniforge3-MacOSX-arm64.sh
use chmod +x to change the execution permissions first

https://pytorch.org/get-started/locally/



# Installing Homebrew
$ /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

==> Next steps:
- Run these two commands in your terminal to add Homebrew to your `$PATH`:
    (echo; echo 'eval "$(/opt/homebrew/bin/brew shellenv)"') >> ~/.zprofile
    eval "$(/opt/homebrew/bin/brew shellenv)"

Check if brew is installed
brew

$ brew list

$ brew deps --tree --installed

$ brew doctor

brew install reattach-to-user-namespace

brew install wget

brew install tmux


# tmux file setup
.tmux.conf ---- File Start
set -g default-terminal "screen-256color"
set-window-option -g mode-keys vi

# Enable mouse control (clickable windows, panes, resizable panes)
set-option -g mouse on

set-option -g history-limit 5000

unbind P
bind-key P command-prompt -p 'save history to filename:' -I '~/tmux.history' 'capture-pane -S - ; save-buffer %1 ; delete-buffer'

bind-key -T copy-mode-vi 'y' send -X copy-pipe-and-cancel 'reattach-to-user-namespace pbcopy'
bind-key -T copy-mode-vi Enter send -X copy-pipe-and-cancel 'reattach-to-user-namespace pbcopy'
.tmux.conf ---- File End

# Copy this file to ~./tmux.conf
Run this command to use the configuration
tmux source-file ~/.tmux.conf

# To Copy from tmux
Press control b followed by [. 
Use the h-j-k-l or arrow keys to move to the line you need to select.
"Shift + v" will select the whole line. 
Now move to the other end of the selection. 
Tmux will highlight your selection in yellow. 
Then press y or return to copy it to the clipboard.


# to keep mac from going to sleep
caffeinate

# To install requirements
pip install -r requirements.txt

#Add extension to files (when we download bulk and the file extensions are not included)
Open Terminal
Navigate to the folder with the files you need to add extension for
Use this command
for i in *; do mv "$i" "$i.jpg”; done

chmod +x FILENAME #to change the permissions to execute

# to install lfs (large file storage on git
git lfs install
