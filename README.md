# Squid
Docker container for squid proxy


## Quickstart
```
docker run --name squid -d \
  --publish 3128:3128 \
  chriskalmar/squid:3.5.27
```

Using your own config file:
```
docker run --name squid -d \
  --publish 3128:3128 \
  --volume $PWD/squid.conf:/etc/squid/squid.conf:ro \
  chriskalmar/squid:3.5.27
```



## Attribution
Derived from [sameersbn/docker-squid](https://github.com/sameersbn/docker-squid)


## License

MIT License

Copyright (c) 2019 Chris Kalmar

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
