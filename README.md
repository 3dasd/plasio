# 3dasd examples viewer

This was forked from [plasio](https://github.com/verma/plasio). See the original readme there.

## Deploying changes

Build and ship files:

```sh
gulp
tar -czf /tmp/plasio.tar.gz build/
scp /tmp/plasio.tar.gz asdasd.hu:/tmp/
```

Deploy (on asdasd.hu):

```sh
cd /var/www/html/3dasd
tar -xzf /tmp/plasio.tar.gz
rm -r examples
mv build examples
```