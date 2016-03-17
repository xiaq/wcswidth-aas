# wcwidth as a service

Terminal softwares don't know how wide characters really are :disappointed::disappointed::disappointed::

![mac](https://raw.githubusercontent.com/xiaq/wcwidth-aas/master/mac.png)
![linux](https://raw.githubusercontent.com/xiaq/wcwidth-aas/master/linux.png)

wcwidth-as-a-service to the rescue :smile::smile::smile:! Simply GET a path to obtain its width:

```sh
> curl http://wcwidth.xiaq.me/Hello
5
> curl http://wcwidth.xiaq.me/こんいちは
10
> curl http://wcwidth.xiaq.me/蛤蛤
4
> curl http://wcwidth.xiaq.me/🌚
2
```

What to do next:

- [ ] Just replace all `wcwidth` implementations in glibc, Cairo, vim, libvte and tmux with a dead-simple HTTP GET
- [ ] ... profit!
