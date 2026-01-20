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
  postgresql16
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
dnf install make gcc patch zlib-devel bzip2 bzip2-devel readline-devel sqlite sqlite-devel openssl-devel tk-devel libffi-devel xz-devel libuuid-devel gdbm-libs libnsl2
```
