# Using Git and Visual Studio Code

## Remove removed (merged) branches from VS Code

### Install git-removed-branches

```bash
sudo npm install -g git-removed-branches

git removed-branches
```

### run command in project directory

`git removed-branches --prune`

add to keybindings.json to enable sync:

````
```json
[
  {
    "key": "ctrl+alt+s",
    "command": "git.sync"
  }
]
````
