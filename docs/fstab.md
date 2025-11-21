# fstab configuration

## Documentation

- [CachyOS Wiki](https://wiki.cachyos.org/configuration/automount_with_fstab/)
- [Arch Wiki](https://wiki.archlinux.org/title/Fstab)
- [`mount` man page](https://linux.die.net/man/8/mount)

## Configuration

My configuration for automounting a new BTRFS drive for steam games and old NTFS drives from the Windows installation:
```
# My other drives
UUID=587afbd0-8602-4ec0-9273-7d0770402e34 /media/LinuxGames btrfs defaults,nofail,user,exec,noatime,compress=zstd,space_cache=v2,commit=120 0 0
UUID=B6DA31C2DA317FA3                     /media/Downloads  ntfs3 defaults,nofail,uid=1000,gid=1000,rw,user,exec,umask=000 0 0
UUID=7EEC6385EC633695                     /media/Archive    ntfs3 defaults,nofail,uid=1000,gid=1000,rw,user,exec,umask=000 0 0
```

### BTRFS

The BTRFS options are taken and modified from the default CachyOS installed partitions, for example:
```
UUID=SOMETHING /home btrfs subvol=/@home,defaults,noatime,compress=zstd,space_cache=v2,commit=120 0 0
```

I added `nofail,user,exec` to the set of options to make it mountable by a non-root user.

> [!NOTE]
> Don't forget to add `exec` explicitly if you add `user` since it assumes `noexec` otherwise (even if default includes `exec`, `user` will override it since it is read in order).

### NTFS

The NTFS options are taken from the CachyOS wiki and mostly used unchanged.
