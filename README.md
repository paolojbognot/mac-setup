# mac-setup
This repo contains all of the information on the apps / settings I use on my Mac.

---

## To-Do List
- [] Install MongoDB
- [] Install MySQL
- [] Upload TLM projects to GitHub
    - Delete all package-lock.json files
    - Refactor TLM projects to use proper CDN paths
- Test
- Update the documentation
    - [] Document Mac Setup Process
    - [] Create a repo for this
    - [] Catalog and document settings
    - [] Map out a proper sequence
    - [] Take screenshots

## Unorganized Apps that I use 100%

### Things to Install on Mac for Development

INSTALL NVM

- [] Homebrew `brew.sh`

### Homebrew `casks`

- [] iterm2
- [] bash
    - [] Oh My Bash
    - [] vcprompt
    - [] fortune
    - [] cowsay
- [] git
- [] rectangle-pro
- [] alt-tab

- [] NVM / Node.js
- [] Caffeine / amphetamine / keepingyouawake ???
- [] raycast
- [] insomnia

- [] chrome

- [] firefo
- [] slack
- [] discord

- [] stats
- [] itsycal


### Firefo
- [] uBlock Origin
- [] privacy badger
- [] tabliss


### VSCode - Themes
- [] Just black
- [] Night Owl


### VSCode - Extensions
- [] FontSize Shortcuts
- [] vscode-icons
- [] Prettier
- [] ESLint

### VSCode - Settings
 - Notable settings:
 ```json
{
  "editor.linkedEditing": true,
  "editor.snippetSuggestions": "top",
}
 ```
- editor.linkedEditing
    - Automatically edit a closing tag when editing an opening tag
- editor.snippetSuggestions
    - Puts the most relevant auto complete options at the top
- Cursor Blinking
    - Set to `expand`
- Render Whitespace
    - Set to `boundary`
- Terminal > Integrated: Cursor Blinking
    - Checked ✅
- Terminal > Integrated: Cursor Style
    - Set to `line`



### How to install MongoDB using Homebrew
- Here is the link: https://www.mongodb.com/docs/manual/tutorial/install-mongodb-on-os-x/
- Steps to install in terminal (iTerm2):
    - `brew tap mongodb/brew`
    - `brew update`
    - `brew install mongodb-community@7.0` - always double check if 7.0 is the latest stable version
    - Now make sure to set the Mongod process to automatically run in the background using brew services

### MongoDB Commands
- `brew services start mongodb-community@7.0` - Automatically runs `mongod` in the background on computer startup
- `brew services stop mongodb-community@7.0` - Manually terminate `mongod` from running in the background
- `mongosh` - Start the MongoDB Shell