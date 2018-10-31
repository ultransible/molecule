Dockerfile for Dubian Buster with systemd


## Usage

You can run container with:
```bash
docker run -dt -v /sys/fs/cgroup:/sys/fs/cgroup:ro --tmpfs /run --tmpfs /run/lock --security-opt seccomp=unconfined  ultransible/debian_10_systemd:v1 name_container 
```
## Build the container

If you want to re-build the container, you have to clone the repo and trigger the building:
```bash
git clone https://github.com/ultransible/molecule.git
cd molecule/OS_systemd/debian10
docker build .
```

## repo github


[repo github](https://github.com/ultransible/molecule)
