## Rclone
```rlocne config # to manage remotes
   rclone listremotes # to see remotes
   rclone mount remote:/ ~/target  # target should be empty dir
   fusermount -u ~/target # unomount
```

## SSh
```ssh -L 8888:localhost:8888 server # forward remote port 8888 to local pc
   ssh -R 8888:localhost:8888 server # forward local port 8888 to remote pc
```

## Lid switch
``` sudo -H gedit /etc/systemd/logind.conf
    # Then simply comment / uncomment the line: HandleLidSwitch=ignore
    sudo systemctl restart systemd-logind
```

## Disk usage
``` du --max-depth=1 --block-size=M
    df -P
    df -h
```
