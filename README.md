# Ps3toolchain

This is a fork of [ps3dev/ps3toolchain](https://github.com/ps3dev/ps3toolchain)

I mostly just made this to fix issues I find without pushing to the main repo, as nobody seems to be responding there anymore.

Currently I have fixed a few broken links in the libraries and un-commented the build script auto-run line.

## How to use

### Dependencies

As far as I'm aware only [Docker](https://www.docker.com/) is needed, everything else is handled inside the instance.

### How to install

Run these commands

```bash
git clone https://github.com/BriellaBugs/ps3toolchain
cd ps3toolchain
docker build -t ps3toolchain .
```

The toolchain script will run during the docker build, if you don't want this, comment out `RUN /build/toolchain.sh` at the end of the `Dockerfile`, note that you will have to run it yourself on an interactive shell or similar if you want it to work.
