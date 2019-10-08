# Docker_toturial result part1

```docker

HuanNing@HuanNing MINGW64 /
$ cd E:\pythondocker

HuanNing@HuanNing MINGW64 /e/pythondocker
$ docker

Usage:  docker [OPTIONS] COMMAND

A self-sufficient runtime for containers

Options:
      --config string      Location of client config files (default
                           "C:\\Users\\HuanNing\\.docker")
  -c, --context string     Name of the context to use to connect to the
                           daemon (overrides DOCKER_HOST env var and
                           default context set with "docker context use")
  -D, --debug              Enable debug mode
  -H, --host list          Daemon socket(s) to connect to
  -l, --log-level string   Set the logging level
                           ("debug"|"info"|"warn"|"error"|"fatal")
                           (default "info")
      --tls                Use TLS; implied by --tlsverify
      --tlscacert string   Trust certs signed only by this CA (default
                           "C:\\Users\\HuanNing\\.docker\\ca.pem")
      --tlscert string     Path to TLS certificate file (default
                           "C:\\Users\\HuanNing\\.docker\\cert.pem")
      --tlskey string      Path to TLS key file (default
                           "C:\\Users\\HuanNing\\.docker\\key.pem")
      --tlsverify          Use TLS and verify the remote
  -v, --version            Print version information and quit

Management Commands:
  builder     Manage builds
  config      Manage Docker configs
  container   Manage containers
  context     Manage contexts
  image       Manage images
  network     Manage networks
  node        Manage Swarm nodes
  plugin      Manage plugins
  secret      Manage Docker secrets
  service     Manage services
  stack       Manage Docker stacks
  swarm       Manage Swarm
  system      Manage Docker
  trust       Manage trust on Docker images
  volume      Manage volumes

Commands:
  attach      Attach local standard input, output, and error streams to a running container
  build       Build an image from a Dockerfile
  commit      Create a new image from a container's changes
  cp          Copy files/folders between a container and the local filesystem
  create      Create a new container
  diff        Inspect changes to files or directories on a container's filesystem
  events      Get real time events from the server
  exec        Run a command in a running container
  export      Export a container's filesystem as a tar archive
  history     Show the history of an image
  images      List images
  import      Import the contents from a tarball to create a filesystem image
  info        Display system-wide information
  inspect     Return low-level information on Docker objects
  kill        Kill one or more running containers
  load        Load an image from a tar archive or STDIN
  login       Log in to a Docker registry
  logout      Log out from a Docker registry
  logs        Fetch the logs of a container
  pause       Pause all processes within one or more containers
  port        List port mappings or a specific mapping for the container
  ps          List containers
  pull        Pull an image or a repository from a registry
  push        Push an image or a repository to a registry
  rename      Rename a container
  restart     Restart one or more containers
  rm          Remove one or more containers
  rmi         Remove one or more images
  run         Run a command in a new container
  save        Save one or more images to a tar archive (streamed to STDOUT by default)
  search      Search the Docker Hub for images
  start       Start one or more stopped containers
  stats       Display a live stream of container(s) resource usage statistics
  stop        Stop one or more running containers
  tag         Create a tag TARGET_IMAGE that refers to SOURCE_IMAGE
  top         Display the running processes of a container
  unpause     Unpause all processes within one or more containers
  update      Update configuration of one or more containers
  version     Show the Docker version information
  wait        Block until one or more containers stop, then print their exit codes

Run 'docker COMMAND --help' for more information on a command.

HuanNing@HuanNing MINGW64 /e/pythondocker
$ docker container --help

Usage:  docker container COMMAND

Manage containers

Commands:
  attach      Attach local standard input, output, and error streams to a running container
  commit      Create a new image from a container's changes
  cp          Copy files/folders between a container and the local filesystem
  create      Create a new container
  diff        Inspect changes to files or directories on a container's filesystem
  exec        Run a command in a running container
  export      Export a container's filesystem as a tar archive
  inspect     Display detailed information on one or more containers
  kill        Kill one or more running containers
  logs        Fetch the logs of a container
  ls          List containers
  pause       Pause all processes within one or more containers
  port        List port mappings or a specific mapping for the container
  prune       Remove all stopped containers
  rename      Rename a container
  restart     Restart one or more containers
  rm          Remove one or more containers
  run         Run a command in a new container
  start       Start one or more stopped containers
  stats       Display a live stream of container(s) resource usage statistics
  stop        Stop one or more running containers
  top         Display the running processes of a container
  unpause     Unpause all processes within one or more containers
  update      Update configuration of one or more containers
  wait        Block until one or more containers stop, then print their exit codes

Run 'docker container COMMAND --help' for more information on a command.

HuanNing@HuanNing MINGW64 /e/pythondocker
$ docker --version
Docker version 19.03.1, build 74b1e89

HuanNing@HuanNing MINGW64 /e/pythondocker
$ docker version
Client: Docker Engine - Community
 Version:           19.03.1
 API version:       1.40
 Go version:        go1.12.5
 Git commit:        74b1e89
 Built:             Thu Jul 25 21:17:08 2019
 OS/Arch:           windows/amd64
 Experimental:      false

Server: Docker Engine - Community
 Engine:
  Version:          19.03.1
  API version:      1.40 (minimum version 1.12)
  Go version:       go1.12.5
  Git commit:       74b1e89
  Built:            Thu Jul 25 21:17:52 2019
  OS/Arch:          linux/amd64
  Experimental:     false
 containerd:
  Version:          v1.2.6
  GitCommit:        894b81a4b802e4eb2a91d1ce216b8817763c29fb
 runc:
  Version:          1.0.0-rc8
  GitCommit:        425e105d5a03fabd737a126ad93d62a9eeede87f
 docker-init:
  Version:          0.18.0
  GitCommit:        fec3683

HuanNing@HuanNing MINGW64 /e/pythondocker
$ docker info
Client:
 Debug Mode: false

Server:
 Containers: 4
  Running: 0
  Paused: 0
  Stopped: 4
 Images: 21
 Server Version: 19.03.1
 Storage Driver: overlay2
  Backing Filesystem: extfs
  Supports d_type: true
  Native Overlay Diff: true
 Logging Driver: json-file
 Cgroup Driver: cgroupfs
 Plugins:
  Volume: local
  Network: bridge host ipvlan macvlan null overlay
  Log: awslogs fluentd gcplogs gelf journald json-file local logentries splunk syslog
 Swarm: inactive
 Runtimes: runc
 Default Runtime: runc
 Init Binary: docker-init
 containerd version: 894b81a4b802e4eb2a91d1ce216b8817763c29fb
 runc version: 425e105d5a03fabd737a126ad93d62a9eeede87f
 init version: fec3683
 Security Options:
  seccomp
   Profile: default
 Kernel Version: 4.9.184-linuxkit
 Operating System: Docker Desktop
 OSType: linux
 Architecture: x86_64
 CPUs: 2
 Total Memory: 1.952GiB
 Name: docker-desktop
 ID: 5KDO:FFU5:4GI6:H4GG:4OA3:3ZUG:WDKO:C4OC:E2WR:JN45:UFNE:M33N
 Docker Root Dir: /var/lib/docker
 Debug Mode: true
  File Descriptors: 29
  Goroutines: 44
  System Time: 2019-10-08T17:41:02.2737582Z
  EventsListeners: 1
 Registry: https://index.docker.io/v1/
 Labels:
 Experimental: false
 Insecure Registries:
  127.0.0.0/8
 Live Restore Enabled: false
 Product License: Community Engine


HuanNing@HuanNing MINGW64 /e/pythondocker
$ docker run hello-world

Hello from Docker!
This message shows that your installation appears to be working correctly.

To generate this message, Docker took the following steps:
 1. The Docker client contacted the Docker daemon.
 2. The Docker daemon pulled the "hello-world" image from the Docker Hub.
    (amd64)
 3. The Docker daemon created a new container from that image which runs the
    executable that produces the output you are currently reading.
 4. The Docker daemon streamed that output to the Docker client, which sent it
    to your terminal.

To try something more ambitious, you can run an Ubuntu container with:
 $ docker run -it ubuntu bash

Share images, automate workflows, and more with a free Docker ID:
 https://hub.docker.com/

For more examples and ideas, visit:
 https://docs.docker.com/get-started/


HuanNing@HuanNing MINGW64 /e/pythondocker
$ docker image ls
REPOSITORY              TAG                 IMAGE ID            CREATED             SIZE
gladcolor/get-started   part2               53bd4e2ed69e        2 hours ago         148MB
huanning/get-started    part2               53bd4e2ed69e        2 hours ago         148MB
friendlyhello           latest              53bd4e2ed69e        2 hours ago         148MB
friendlyhi              latest              53bd4e2ed69e        2 hours ago         148MB
gladcolor/cheers2019    latest              a777105ac44c        7 days ago          4.01MB
<none>                  <none>              14d66a79f035        7 days ago          356MB
python-barcode          latest              13d2ad475916        2 weeks ago         941MB
<none>                  <none>              f2d8fc311c70        2 weeks ago         941MB
python                  2.7-slim            f462855313cd        3 weeks ago         137MB
python                  3                   02d2bb146b3b        3 weeks ago         918MB
golang                  1.11-alpine         e116d2efa2ab        6 weeks ago         312MB
hello-world             latest              fce289e99eb9        9 months ago        1.84kB

HuanNing@HuanNing MINGW64 /e/pythondocker
$ docker container ls
CONTAINER ID        IMAGE               COMMAND             CREATED             STATUS              PORTS               NAMES

HuanNing@HuanNing MINGW64 /e/pythondocker
$ docker ls --all
unknown flag: --all
See 'docker --help'.

Usage:  docker [OPTIONS] COMMAND

A self-sufficient runtime for containers

Options:
      --config string      Location of client config files (default
                           "C:\\Users\\HuanNing\\.docker")
  -c, --context string     Name of the context to use to connect to the
                           daemon (overrides DOCKER_HOST env var and
                           default context set with "docker context use")
  -D, --debug              Enable debug mode
  -H, --host list          Daemon socket(s) to connect to
  -l, --log-level string   Set the logging level
                           ("debug"|"info"|"warn"|"error"|"fatal")
                           (default "info")
      --tls                Use TLS; implied by --tlsverify
      --tlscacert string   Trust certs signed only by this CA (default
                           "C:\\Users\\HuanNing\\.docker\\ca.pem")
      --tlscert string     Path to TLS certificate file (default
                           "C:\\Users\\HuanNing\\.docker\\cert.pem")
      --tlskey string      Path to TLS key file (default
                           "C:\\Users\\HuanNing\\.docker\\key.pem")
      --tlsverify          Use TLS and verify the remote
  -v, --version            Print version information and quit

Management Commands:
  builder     Manage builds
  config      Manage Docker configs
  container   Manage containers
  context     Manage contexts
  image       Manage images
  network     Manage networks
  node        Manage Swarm nodes
  plugin      Manage plugins
  secret      Manage Docker secrets
  service     Manage services
  stack       Manage Docker stacks
  swarm       Manage Swarm
  system      Manage Docker
  trust       Manage trust on Docker images
  volume      Manage volumes

Commands:
  attach      Attach local standard input, output, and error streams to a running container
  build       Build an image from a Dockerfile
  commit      Create a new image from a container's changes
  cp          Copy files/folders between a container and the local filesystem
  create      Create a new container
  diff        Inspect changes to files or directories on a container's filesystem
  events      Get real time events from the server
  exec        Run a command in a running container
  export      Export a container's filesystem as a tar archive
  history     Show the history of an image
  images      List images
  import      Import the contents from a tarball to create a filesystem image
  info        Display system-wide information
  inspect     Return low-level information on Docker objects
  kill        Kill one or more running containers
  load        Load an image from a tar archive or STDIN
  login       Log in to a Docker registry
  logout      Log out from a Docker registry
  logs        Fetch the logs of a container
  pause       Pause all processes within one or more containers
  port        List port mappings or a specific mapping for the container
  ps          List containers
  pull        Pull an image or a repository from a registry
  push        Push an image or a repository to a registry
  rename      Rename a container
  restart     Restart one or more containers
  rm          Remove one or more containers
  rmi         Remove one or more images
  run         Run a command in a new container
  save        Save one or more images to a tar archive (streamed to STDOUT by default)
  search      Search the Docker Hub for images
  start       Start one or more stopped containers
  stats       Display a live stream of container(s) resource usage statistics
  stop        Stop one or more running containers
  tag         Create a tag TARGET_IMAGE that refers to SOURCE_IMAGE
  top         Display the running processes of a container
  unpause     Unpause all processes within one or more containers
  update      Update configuration of one or more containers
  version     Show the Docker version information
  wait        Block until one or more containers stop, then print their exit codes

Run 'docker COMMAND --help' for more information on a command.


HuanNing@HuanNing MINGW64 /e/pythondocker
$ docker container ls --all
CONTAINER ID        IMAGE               COMMAND             CREATED             STATUS                        PORTS               NAMES
a5adda83fb2f        hello-world         "/hello"            44 seconds ago      Exited (0) 43 seconds ago                         hardcore_taussig
5fb38d8b2b97        friendlyhello       "python app.py"     2 hours ago         Created                                           beautiful_volhard
0f4305ce72d3        friendlyhello       "python app.py"     2 hours ago         Exited (137) 32 minutes ago                       nifty_chebyshev
1095b68abc69        hello-world         "/hello"            2 hours ago         Exited (0) 2 hours ago                            dreamy_dewdney
2e46fcb092eb        hello-world         "/hello"            13 days ago         Exited (0) 13 days ago                            angry_mccarthy

HuanNing@HuanNing MINGW64 /e/pythondocker
$ docker container ls -aq
a5adda83fb2f
5fb38d8b2b97
0f4305ce72d3
1095b68abc69
2e46fcb092eb
```


# Part2
```
HuanNing@HuanNing MINGW64 /e/pythondocker
$ docker build --tag=friendlyhi .
Sending build context to Docker daemon  6.144kB
Step 1/7 : FROM python:2.7-slim
 ---> f462855313cd
Step 2/7 : WORKDIR /app
 ---> Using cache
 ---> 8c9cb1ca3c14
Step 3/7 : COPY . /app
 ---> Using cache
 ---> 5bc0a5824b56
Step 4/7 : RUN pip install --trusted-host pypi.python.org -r requirements.txt
 ---> Using cache
 ---> 8622419fc718
Step 5/7 : EXPOSE 80
 ---> Using cache
 ---> 58266a71feed
Step 6/7 : ENV NAME World
 ---> Using cache
 ---> 7a6d7125ca02
Step 7/7 : CMD ["python", "app.py"]
 ---> Using cache
 ---> 53bd4e2ed69e
Successfully built 53bd4e2ed69e
Successfully tagged friendlyhi:latest
SECURITY WARNING: You are building a Docker image from Windows against a non-Windows Docker host. All files and directories added to build context will have '-rwxr-xr-x' permissions. It is recommended to double check and reset permissions for sensitive files and directories.

HuanNing@HuanNing MINGW64 /e/pythondocker
$ docker push gladcolor/friendlyhi
The push refers to repository [docker.io/gladcolor/friendlyhi]
An image does not exist locally with the tag: gladcolor/friendlyhi

HuanNing@HuanNing MINGW64 /e/pythondocker
$ docker push friendlyhi
The push refers to repository [docker.io/library/friendlyhi]
f609c03614fd: Preparing
74e5b9271e7e: Preparing
b2f2935a4fb7: Preparing
a4f231ef8285: Preparing
912905f45a34: Preparing
411e68dbb588: Preparing
2db44bce66cd: Preparing
411e68dbb588: Waiting
2db44bce66cd: Waiting
denied: requested access to the resource is denied

HuanNing@HuanNing MINGW64 /e/pythondocker
$ docker stop friendlyhi
Error response from daemon: No such container: friendlyhi

HuanNing@HuanNing MINGW64 /e/pythondocker
$ docker container ls
CONTAINER ID        IMAGE               COMMAND             CREATED             STATUS              PORTS               NAMES

HuanNing@HuanNing MINGW64 /e/pythondocker
$ docker image ls
REPOSITORY             TAG                 IMAGE ID            CREATED             SIZE
huanning/get-started   part2               53bd4e2ed69e        2 hours ago         148MB
friendlyhello          latest              53bd4e2ed69e        2 hours ago         148MB
friendlyhi             latest              53bd4e2ed69e        2 hours ago         148MB
gladcolor/cheers2019   latest              a777105ac44c        7 days ago          4.01MB
<none>                 <none>              14d66a79f035        7 days ago          356MB
python-barcode         latest              13d2ad475916        2 weeks ago         941MB
<none>                 <none>              f2d8fc311c70        2 weeks ago         941MB
python                 2.7-slim            f462855313cd        3 weeks ago         137MB
python                 3                   02d2bb146b3b        3 weeks ago         918MB
golang                 1.11-alpine         e116d2efa2ab        6 weeks ago         312MB
hello-world            latest              fce289e99eb9        9 months ago        1.84kB

HuanNing@HuanNing MINGW64 /e/pythondocker
$ docker push 53bd4e2ed69e
The push refers to repository [docker.io/library/53bd4e2ed69e]
An image does not exist locally with the tag: 53bd4e2ed69e

HuanNing@HuanNing MINGW64 /e/pythondocker
$ docker push 53bd4e2ed69e
The push refers to repository [docker.io/library/53bd4e2ed69e]
An image does not exist locally with the tag: 53bd4e2ed69e

HuanNing@HuanNing MINGW64 /e/pythondocker
$ docker image push 53bd4e2ed69e
The push refers to repository [docker.io/library/53bd4e2ed69e]
An image does not exist locally with the tag: 53bd4e2ed69e

HuanNing@HuanNing MINGW64 /e/pythondocker
$ docker push gladcolor/friendlyhi
The push refers to repository [docker.io/gladcolor/friendlyhi]
An image does not exist locally with the tag: gladcolor/friendlyhi

HuanNing@HuanNing MINGW64 /e/pythondocker
$ docker login
Authenticating with existing credentials...
Login Succeeded

HuanNing@HuanNing MINGW64 /e/pythondocker
$ docker tag friendlyhi gladcolor/get-started:part2

HuanNing@HuanNing MINGW64 /e/pythondocker
$ docker image ls
REPOSITORY              TAG                 IMAGE ID            CREATED             SIZE
huanning/get-started    part2               53bd4e2ed69e        2 hours ago         148MB
friendlyhello           latest              53bd4e2ed69e        2 hours ago         148MB
friendlyhi              latest              53bd4e2ed69e        2 hours ago         148MB
gladcolor/get-started   part2               53bd4e2ed69e        2 hours ago         148MB
gladcolor/cheers2019    latest              a777105ac44c        7 days ago          4.01MB
<none>                  <none>              14d66a79f035        7 days ago          356MB
python-barcode          latest              13d2ad475916        2 weeks ago         941MB
<none>                  <none>              f2d8fc311c70        2 weeks ago         941MB
python                  2.7-slim            f462855313cd        3 weeks ago         137MB
python                  3                   02d2bb146b3b        3 weeks ago         918MB
golang                  1.11-alpine         e116d2efa2ab        6 weeks ago         312MB
hello-world             latest              fce289e99eb9        9 months ago        1.84kB

HuanNing@HuanNing MINGW64 /e/pythondocker
$ docker push gladcolor/get-started:part2
The push refers to repository [docker.io/gladcolor/get-started]
f609c03614fd: Preparing
74e5b9271e7e: Preparing
b2f2935a4fb7: Preparing
a4f231ef8285: Preparing
912905f45a34: Preparing
411e68dbb588: Preparing
2db44bce66cd: Preparing
411e68dbb588: Waiting
2db44bce66cd: Waiting
74e5b9271e7e: Pushed
b2f2935a4fb7: Pushed
a4f231ef8285: Pushed
f609c03614fd: Pushed
411e68dbb588: Pushed
912905f45a34: Pushed
2db44bce66cd: Pushed
part2: digest: sha256:3b6a6fe93a426bc95f764e837118f9107bd1e2455c91bb5d1782122209d73a8f size: 1788
```

```
HuanNing@HuanNing MINGW64 /e/pythondocker
$ docker swarm init
Swarm initialized: current node (4wphjhicchau7azj21ken4r6f) is now a manager.

To add a worker to this swarm, run the following command:

    docker swarm join --token SWMTKN-1-50ura87hfyu3yuefxm88twehe4hsc94e535prrapc9831lap9z-6ryu4s7iy8sr2w624qenjlw9x 192.168.65.3:2377

To add a manager to this swarm, run 'docker swarm join-token manager' and follow the instructions.


HuanNing@HuanNing MINGW64 /e/pythondocker
$ docker stack deploy -c docker-compose.yml getstartedlab
Creating network getstartedlab_webnet
Creating service getstartedlab_web

HuanNing@HuanNing MINGW64 /e/pythondocker
$ docker service ls
ID                  NAME                MODE                REPLICAS            IMAGE                         PORTS
yvny7wyajrac        getstartedlab_web   replicated          5/5                 gladcolor/get-started:part2   *:4000->80/tcp

HuanNing@HuanNing MINGW64 /e/pythondocker
$ docker stack services getstartedlab
ID                  NAME                MODE                REPLICAS            IMAGE                         PORTS
yvny7wyajrac        getstartedlab_web   replicated          5/5                 gladcolor/get-started:part2   *:4000->80/tcp

HuanNing@HuanNing MINGW64 /e/pythondocker
$ docker service ps getstartedlab_web
ID                  NAME                  IMAGE                         NODE                DESIRED STATE       CURRENT STATE           ERROR               PORTS
7zkaes0h8n4d        getstartedlab_web.1   gladcolor/get-started:part2   docker-desktop      Running             Running 3 minutes ago            
17z9qpxrd9t7        getstartedlab_web.2   gladcolor/get-started:part2   docker-desktop      Running             Running 3 minutes ago            
nmgycgh2brfh        getstartedlab_web.3   gladcolor/get-started:part2   docker-desktop      Running             Running 3 minutes ago            
bx5sfmsz4dlh        getstartedlab_web.4   gladcolor/get-started:part2   docker-desktop      Running             Running 3 minutes ago            
llrlsvqftri0        getstartedlab_web.5   gladcolor/get-started:part2   docker-desktop      Running             Running 3 minutes ago            

HuanNing@HuanNing MINGW64 /e/pythondocker
$ docker container ls -q
5edc30661da8
872baa8e11e4
7e2d6909ee59
55fa2e1e8421
42ff116b7eaa
eb5133c0e4dd

HuanNing@HuanNing MINGW64 /e/pythondocker
$ curl -4 http://localhost:4000
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100   118  100   118    0     0    139      0 --:--:-- --:--:-- --:--:--   139<h3>Hello World!</h3><b>Hostname:</b> eb5133c0e4dd<br/><b>Visits:</b> <i>cannot connect to Redis, counter disabled</i>

HuanNing@HuanNing MINGW64 /e/pythondocker
$ curl -4 http://localhost:4000
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100   118  100   118    0     0    138      0 --:--:-- --:--:-- --:--:--   138<h3>Hello World!</h3><b>Hostname:</b> eb5133c0e4dd<br/><b>Visits:</b> <i>cannot connect to Redis, counter disabled</i>

HuanNing@HuanNing MINGW64 /e/pythondocker
$ curl -4 http://localhost:4000
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100   118  100   118    0     0    139      0 --:--:-- --:--:-- --:--:--   139<h3>Hello World!</h3><b>Hostname:</b> eb5133c0e4dd<br/><b>Visits:</b> <i>cannot connect to Redis, counter disabled</i>

HuanNing@HuanNing MINGW64 /e/pythondocker
$ curl -4 http://localhost:4000
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100   118  100   118    0     0    139      0 --:--:-- --:--:-- --:--:--   139<h3>Hello World!</h3><b>Hostname:</b> eb5133c0e4dd<br/><b>Visits:</b> <i>cannot connect to Redis, counter disabled</i>

HuanNing@HuanNing MINGW64 /e/pythondocker
$ docker container ls -q
5edc30661da8
872baa8e11e4
7e2d6909ee59
55fa2e1e8421
42ff116b7eaa
eb5133c0e4dd

HuanNing@HuanNing MINGW64 /e/pythondocker
$ docker container ls -q
5edc30661da8
872baa8e11e4
7e2d6909ee59
55fa2e1e8421
42ff116b7eaa
eb5133c0e4dd

HuanNing@HuanNing MINGW64 /e/pythondocker
$ docker container ls -q
5edc30661da8
872baa8e11e4
7e2d6909ee59
55fa2e1e8421
42ff116b7eaa
eb5133c0e4dd

HuanNing@HuanNing MINGW64 /e/pythondocker
$ docker stack ps
"docker stack ps" requires exactly 1 argument.
See 'docker stack ps --help'.

Usage:  docker stack ps [OPTIONS] STACK

List the tasks in the stack

HuanNing@HuanNing MINGW64 /e/pythondocker
$ docker stack ps app
nothing found in stack: app

HuanNing@HuanNing MINGW64 /e/pythondocker
$ docker stack ps
"docker stack ps" requires exactly 1 argument.
See 'docker stack ps --help'.

Usage:  docker stack ps [OPTIONS] STACK

List the tasks in the stack

HuanNing@HuanNing MINGW64 /e/pythondocker
$ docker stack ps getstartedlab_web.1
nothing found in stack: getstartedlab_web.1

HuanNing@HuanNing MINGW64 /e/pythondocker
$ docker stack rm getstartedlab
Removing service getstartedlab_web
Removing network getstartedlab_webnet

HuanNing@HuanNing MINGW64 /e/pythondocker
$ docker swarm leave --force

```
