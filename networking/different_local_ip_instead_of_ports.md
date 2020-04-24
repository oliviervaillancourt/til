# Using different 127.0.0.x instead of different port

Mind blown when learned this trick from @clemensv where instead of using differents to run docker container locally, you can just use different ip address in the `127.0.0.x` range

```
docker run -d --rm -p 127.0.0.11:80:80 nginx && \
    docker run -d --rm -p 127.0.0.12:80:80 nginx
```

No clashes

Original link: [Twitter post](https://twitter.com/clemensv/status/1244589698674286594)
