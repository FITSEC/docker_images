If you need help with the installation of docker click [here](https://github.com/FITSEC/docker_images/tree/main/cse1001_vnc/docker_help).
Keep in mind that the instructions are tailored for the CSE1001 course, but the steps will be the same. 

Pull/run commands:
These commands include the bind/mount of a folder from the docker to your host computer. You can remove '-v' and the file path following it if you don't want to do that, and you can add -rm after run if you'd like the container to remove itself after every time you use it.

```
docker run --rm -it -p 9020:8080 -p 9021:5900 tjoconnor/cyber_ops_vnc

```

# References

EntryPoint.sh startup script copied and modified from https://github.com/iphoneintosh/kali-docker.
