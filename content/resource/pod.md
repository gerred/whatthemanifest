+++
name = "Pod"
introduced = "1.0"
slug = "pod"
description = "A pod is a single scheduling unit inside of a Kubernetes cluster. Can contain multiple containers. More description text here."
+++


~~~yaml
apiVersion: v1
kind: Pod
spec:
  containers:
    -
      args:
        - "foo"
        - "bar"
      command:
        - "./start.sh"
      env:
        -
          name: "REDIS_URL"
          value: "redis://redis.default.cluster.local"
      image: "alpine"
      imagePullPolicy: ""
      name: ""
      ports:
        -
          containerPort: 8080
          protocol: "tcp"
      resources:
        cpu: "0.5"
        memory: "512M"
  restartPolicy: ""
  volumes:
    -
      emptyDir:
        medium: ""
      name: ""
      secret:
        secretName: ""
~~~
