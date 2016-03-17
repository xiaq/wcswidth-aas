# wcwidth as a service

Terminal softwares don't know how wide characters really are (😔😔😔):

![mac](https://raw.githubusercontent.com/xiaq/wcwidth-aas/master/mac.png)
![linux](https://raw.githubusercontent.com/xiaq/wcwidth-aas/master/linux.png)

wcwidth-as-a-service to the rescue (😄😄😄)! Simply GET a path to obtain its width:

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

- [ ] Replace all `wcwidth` implementations with a simple HTTP GET
- [ ] ... profit!
