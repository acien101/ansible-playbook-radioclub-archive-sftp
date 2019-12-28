# Ansible Playbook RadioClub Archive

![](./pics/screenshot.png)

Ansible playbook for deploying [Docker-alpine-apache-ftp-server](https://github.com/acien101/docker-alpine-apache-ftp-server). A public FTP server built with docker. Works with apache and vsftpd inside a micro alpine linux docker. The aim of this project is to upload the satellite receptions to the FTP, to be public (but can be used for a lot of things).

Deployment based on [Anarres](https://github.com/anarres-org), so the remote server must be configured as Anarres (every server on RadioClub right now).

## How to deploy

You must have ansible installed.

```
$ ansible-playbook --ask-vault-pass -i custom/ea4rct/hosts.yml --limit "zulu" --tags "archive_ftp" full.yml
```

## Author

* Fran Acien
