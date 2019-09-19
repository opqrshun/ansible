


##setup
```
ansible-playbook -i host_file site.yml --tags setup --extra-vars "server=server_name user=user_name nginx=proxy"
```

##setup roles
```
 --tags user,python,firewalld,selinux etc...
```

nginx(proxy)
```
--tags nginx --extra-vars "server=server_name user=user_name nginx=proxy"
```

create_user(ssh)
```
--tags user --extra-vars "server=server_name user=user_name create_user=user_name key_passphrase=passphrase "
```


--ask-become-pass=sudo password

## OS
- centos7
- debian

## roles
--tags
- user
- docker
- php
- python
- pip (venv)
- node (n)
- go
- nginx
- unit
- firewalld
- selinux (httpd)
