# Docker Images
For more information on the images, instructions, and commands for additional platforms click on the name of the course you want to view.

## Images

| Name    	    | DockerHub 		      | Run 		   		         	  	    |
|---------------|-------------------------|-----------------------------------------|
| [cse1001](cse1001_vnc)	    | [tjoconnor/cse1001](https://hub.docker.com/r/tjoconnor/cse1001) 	  | docker run -d -p 6080:80 -v $PWD:/home/cse1001/workspace:rw -e VNC_PASSWORD=changeme --name test_command tjoconnor/cse1001_vnc  |
| [cse4001](cse4001) 	    | [tjoconnor/cse4001](https://hub.docker.com/r/tjoconnor/cse4001)	  | docker run -ti --name cse4001 tjoconnor/cse4001            |
| [cse4001_vnc](cse4001_vnc)	| [tjoconnor/cse4001_vnc](https://hub.docker.com/r/tjoconnor/cse4001_vnc)   | docker run --detach --publish 7080:80 --volume "${PWD}":/home/cse4001/workspace:rw --env VNC_PASSWORD=changeme --env RESOLUTION=1400x900 --name cse4001 tjoconnor/cse4001_vnc  |
| [cyber_ops](cyber_ops)		| [tjoconnor/cyber_ops](https://hub.docker.com/r/tjoconnor/cyber_ops)	  | docker run --cap-add=SYS_PTRACE --cap-add=SYS_ADMIN --cap-add=audit_control --security-opt seccomp=unconfined --privileged -ti  tjoconnor/cyber_ops |
| [cyber_ops_vnc](cyber_ops_vnc) | [tjoconnor/cyber_ops_vnc](https://hub.docker.com/r/tjoconnor/cyber_ops_vnc) | docker run -p8888:? --cap-add=SYS_PTRACE --cap-add=SYS_ADMIN --cap-add=audit_control --security-opt seccomp=unconfined --privileged tjoconnor/cyber_ops_vnc 		 |

## References

Original work by [Doro Wu](https://github.com/fcwu)

Adapted by [Frédéric Boulanger](https://github.com/Frederic-Boulanger-UPS)

## License
==================

Apache License Version 2.0, January 2004 http://www.apache.org/licenses/LICENSE-2.0

