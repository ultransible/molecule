# systemd Docker Container 

Dockerfile for Dubian stretch with systemd [Facebook ReDex](http://fbredex.com/)


## Usage

You can run container with:
```bash
docker run -dt -v /sys/fs/cgroup:/sys/fs/cgroup:ro --tmpfs /run --tmpfs /run/lock --security-opt seccomp=unconfined  ultransible/debian_9_systemd:v1 name_container 
```
## Build the container

If you want to re-build the container, you have to clone the repo and trigger the building:
```bash
git clone https://github.com/ultransible/molecule.git
cd molecule/OS_systemd/debian9
docker build .
```

## repo github


[repo github](https://github.com/ultransible/molecule)
