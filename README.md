# alpine-unrar
APKBUILD for unrar by rarlab.com to build the non-free version

## How to build

Some steps have been picked from the [Creating an Alpine package](https://wiki.alpinelinux.org/wiki/Creating_an_Alpine_package) guide.


1. Add the development tools for Alpine packages

```sh
apk add alpine-sdk
```


2. Generate keys for signing the build

```sh
abuild-keygen -a -i
```


3. Clone the git repo

```sh
git clone https://github.com/chereskata/alpine-unrar.git; cd alpine-unrar/unrar
```


4. Generate checksums and build the package

```sh
abuild checksum; abuild -r
```


