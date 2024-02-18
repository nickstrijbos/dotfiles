## Usage

### Install

This playbook includes a custom shell script located at `bin/dotfiles`. This script is added to your $PATH after installation and can be run multiple times while making sure any Ansible dependencies are installed and updated.

This shell script is also used to initialize your environment after installing `Arch` and performing a full system upgrade as mentioned above.

> NOTE: You must follow required steps before running this command or things may become unusable until fixed.

```bash
bash -c "$(curl -fsSL https://raw.githubusercontent.com/nickstrijbos/dotfiles/main/bin/dotfiles)"
```

If you want to run only a specific role, you can specify the following bash command:
```bash
curl -fsSL https://raw.githubusercontent.com/nickstrijbos/dotfiles/main/bin/dotfiles | bash -s -- --tags comma,seperated,tags
```