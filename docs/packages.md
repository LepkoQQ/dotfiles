# Packages to install

## Fedora

### My lists

```sh
sudo dnf install \
  git \
  alacritty \
  zsh \
  fzf \
  ripgrep \
  chezmoi \
  kubernetes1.35 \
  k9s \
  postgresql16 \
  libpq-devel \
  libmemcached-awesome-devel \
  jq \
  inkscape \
  chromium \
  awscli2 \
  gimp \
  sqlitebrowser
```

From third-party repos (google them)

```sh
iosevka-fonts iosevka-term-fonts
docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
slack
code
```

List installed packages

```sh
dnf list --installed
```

### Other lists

Development packages

```sh
sudo dnf install make automake gcc gcc-c++
```

Development packages recommended by **pyenv**

```sh
sudo dnf install make gcc patch zlib-devel bzip2 bzip2-devel readline-devel sqlite sqlite-devel openssl-devel tk-devel libffi-devel xz-devel libuuid-devel gdbm-libs libnsl2
```

Install **pyenv**

```sh
curl -fsSL https://pyenv.run | bash
```

Install **virtualenv** and **pip**

```sh
sudo dnf install python3-virtualenv python3-pip
```

Install **virtualenvwrapper**

```sh
sudo pip install virtualenvwrapper
```

### Other packages

- nvm
  - [installation](https://github.com/nvm-sh/nvm?tab=readme-ov-file#installing-and-updating)
  - you dont need shell config in .zshrc if you have the nvm plugin enabled
- pass-cli (Proton Pass)
  - [installation](https://protonpass.github.io/pass-cli/get-started/installation/#quick-install)

### Asus specific packages

- asusctl
  - battery charge limit is reset to 100% on boot by default
  - use `asusctl` to set it and `asusd` service will remember it
  - [installation](https://asus-linux.org/guides/fedora-guide/)
  - [documentation](https://wiki.archlinux.org/title/Asusctl#Charge_limit)
