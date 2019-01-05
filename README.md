# Linux Desktop container role

Creates a linux development environment with the tools that I use.

# Variables

 - `username` - Username that will have the configuration files installed.
 - `gpg_key` - If set, install this key as your GPG key, also it configures your
   git to use it.
 - `gpg_hash` - The respective hash of your GPG key.
 - `git_name` - The name that you want to be displayed in your commits
 - `git_email` - Your email
 - `extra_git_repos` - A list of `{repo:... location:...}` of additional git
   repositories to clone.
 
# Notes

- Save your wallpaper to `${HOME}/.wallpaper.jpg`

## Requirements

This role is meant to be run in a **Debian Linux** system.

## Example Playbook


```yaml
    - hosts: desktops
      roles:
         - opsxcq.linux-desktop
```
