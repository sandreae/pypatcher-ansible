# py_patcher ansible playbook

## prerequisits

- provision server
- create `sam` user with sudo rights
- install ssh keys

## required host vars

```
lounge_music_url="https://path-to/lounge-music.mp3"  
icecast_server_url="my.stream.com"  
icecast_port=12345  
icecast_mount=stream  
icecast_password=BadPassWord  
```

## TODO

- automate server deploy and initial setup
- change requirement for `sam` user
