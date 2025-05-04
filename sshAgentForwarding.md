# SSH-Agent Forwarding

~/.ssh/config

```bash
Host name
    Hostname name.com
    User root
    PreferredAuthentications publickey
    IdentityFile ~/.ssh/privateKey
    AddKeysToAgent yes
    ForwardAgent yes
```

Make sure your local ssh-agent is running. To enable local ssh-agent automatically on every zsh, add this to your .zshrc

```zsh
if [ -z "$SSH_AUTH_SOCK" ] ; then
  eval "$(ssh-agent -s)" >/dev/null 2>&1
fi
```


