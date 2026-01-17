# Ps3toolchain

This is a fork of [ps3dev/ps3toolchain](https://github.com/ps3dev/ps3toolchain)

I mostly just made this to fix issues I find without pushing to the main repo, as nobody seems to be responding there anymore.

Currently I have fixed a few broken links in the libraries and un-commented the build script auto-run line.

## Dependencies

As far as I'm aware only [Docker](https://www.docker.com/) is needed, everything else is handled inside the Docker container.

## How to install

Run these commands

```bash
git clone https://github.com/BriellaBugs/ps3toolchain
cd ps3toolchain
docker build -t ps3toolchain .
docker run -it --rm -v "$PWD":/build ps3toolchain # Enter the docker instance
```
Inside the docker instance:
```bash
./toolchain.sh
exit
```

## How to run

```bash
cd /path/to/your/ps3toolchain/git/clone
docker run -it --rm -v "$PWD":/build ps3toolchain 
```
