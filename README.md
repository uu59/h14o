# h14o

https://www.google.co.jp/search?q=h14o&source=lnms&tbm=isch

h14o is a wrapper of [h2o](h2o.examp1e.net) for the casual reverse proxying.

## Usage

```console
$ ./h14o -h
Usage: ./h14o
Options:
  -p    Listen Port (default: 3333)
  -b    Listen Bind (default: 127.0.0.1)
  -f    Forward to here (default: http://localhost:3000/)
  -h    Show this message
```

```console
$ ./h14o
Starting to forward: https://127.0.0.1:3333 -> http://localhost:3000

[warning] failed to set TCP_FASTOPEN:Invalid argument
[warning] failed to set TCP_FASTOPEN:Invalid argument
[INFO] raised RLIMIT_NOFILE to 10240
h2o server (pid:49022) is ready to serve requests
...
```

Now you can visit https://127.0.0.1:3333/ to access http://localhost:3000/.
