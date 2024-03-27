` 32768 - 60999 ` open the port numbers in the security groups. <br />
install the docker and ssh plugins/addons <br />

open docker socket service file ` vi /lib/systemd/system/docker.service `  and updata  <br /> 
`ExecStart=/usr/bin/dockerd -H tcp://0.0.0.0:4243 -H unix:///var/run/docker.sock --containerd=/run/containerd/containerd.sock `
