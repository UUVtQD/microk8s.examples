### Commands

```bash
microk8s.kubectl apply -f deployment.yaml 
microk8s.kubectl get po
microk8s.kubectl exec -ti -c a-container po/a-container-7844df568-d84hb -- bash 
  apt update; apt install -y stress
  apt install procps
  stress --vm 1 --vm-bytes 120M &
  stress --vm 1 --vm-bytes 250M
```

### References

- [Medium article](https://medium.com/@zhimin.wen/memory-limit-of-pod-and-oom-killer-891ee1f1cad8)
- [How to do Java JVM heap dump inkubernetes](https://danlebrero.com/2018/11/20/how-to-do-java-jvm-heapdump-in-kubernetes/)
- [Medium - Java heap dump](https://medium.com/@unniksk/kubernetes-java-heap-dump-slack-571b4caebb48)

### COnclusion

```bash 
lifecycle:
          preStop:
            exec:
```
doesn't work when pod killed by `OOM` :(
