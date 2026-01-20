# Ps3toolchain

This is a fork of [ps3dev/ps3toolchain](https://github.com/ps3dev/ps3toolchain)

This fixes any broken links I found and provides instructions on how to setup the toolchain inside Docker

## Dependencies

As far as I'm aware only [Docker](https://www.docker.com/) is needed, everything else is handled inside the Docker container.

## How to install

Run these commands

```bash
git clone https://github.com/BriellaBugs/ps3toolchain
cd ps3toolchain
docker build -t ps3toolchain .
```

## How to run

```bash
cd /path/to/ps3toolchain.git/
docker run -it --rm -v "$PWD"/..:/build ps3toolchain
./toolchain.sh
# Use the toolchain for whatever here
exit
```
