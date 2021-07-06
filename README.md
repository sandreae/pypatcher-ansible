# py_patcher ansible playbook

## Prerequisites

- provision server with ssh access for root
- local user with ssh keys in home directory (by default this is `sam` user)

## Run

```sh
# setup the server with required user and permissions
# copies ssh keys from default users home directory
$ ansible-playbook setup-server.yml -u root
# install and setup services for pypatcher
$ ansible-playbook install-pypatcher.yml
```

## Example ansible hosts file with required vars

```
[pypatcher]
123.123.123.123

[pypatcher:vars]
lounge_music_url="https://path-to/lounge-music.mp3"  
icecast_server_url="my.stream.com"  
icecast_port=12345  
icecast_mount=stream  
icecast_password=BadPassWord  
```

## TODO

- automate server deploy
- change requirement for `sam` user
