# megacmd commands for synching

## login with your user account

```bash
mega-login username password
```

## start synchronization

```bash
mega-sync /local/path /cloud/path
```

## watch transfers

```bash
watch mega-transfers --summary
```

```bash
watch mega-transfers --show-syncs --limit=25
```

```bash
watch mega-sync
```

## enable synchronization of hidden files (.*)

```bash
mega-exclude -d ".*"
```

see https://github.com/meganz/MEGAcmd/issues/392