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
  libpq-devel
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
