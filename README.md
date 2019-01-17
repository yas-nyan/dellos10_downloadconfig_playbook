# dellos10_saveconfig_playbook
**You can get config files from your lovely swiches.**


## b
## how to use
0. make oparator account
```txt:
(config)# username admin password PASSWORD role sysadmin

```

1. clone
2. edit configuration files(hosts,credential.yml)
```yml:hosts
[dell]
dell1    ansible_host=xxx.xxx.xxx.xxx
```

```yml:credential.yml
ansible_user: delluser
ansible_password: dellIsNumberOne
timeout: 30
save_dir: ./backups
```

3. excute
```bash:~/
$ ansible-playbook -i hosts all_save.yml
```
