
# VS Code Minimal Setup

This repository contains a clean, distraction-free VS Code setup including:

- `settings.json` – Editor & UI settings  
- `keybindings.json` – Custom keyboard shortcuts  
- `extensions.txt` – List of recommended extensions  
- `clean.code-workspace` – Workspace file for a minimalist layout

## Setup on a New Machine

1. **Clone the Repository**

```bash
cd ~
git clone git@github.com:AbuzarGhafari/my-snippets.git 
cd ~/my-snippets
```

2. **Install Extensions**

```bash
xargs -n 1 code --install-extension < ~/my-snippets/vscode-setup/extensions.txt
```


3. **Link Settings and Keybindings**

```bash
mkdir -p ~/.config/Code/User
cp ~/my-snippets/vscode-setup/settings.json ~/.config/Code/User/settings.json
cp ~/my-snippets/vscode-setup/keybindings.json ~/.config/Code/User/keybindings.json
```

4. **Open the Workspace**

```bash
# code ~/my-snippets/clean.code-workspace
```

5. **Update Setup**

```bash
cd ~/my-snippets
git pull
xargs -n 1 code --install-extension < ~/my-snippets/vscode-setup/extensions.txt
cp ~/my-snippets/vscode-setup/settings.json ~/.config/Code/User/settings.json
cp ~/my-snippets/vscode-setup/keybindings.json ~/.config/Code/User/keybindings.json
```
