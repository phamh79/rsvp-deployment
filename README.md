# rsvp-deployment
## Local evn
Images are from Docker hub repo so make sure it is logged-in.
For Kubernetest, execute [follow this step](https://kubernetes.io/docs/tasks/configure-pod-container/pull-image-private-registry/#registry-secret-existing-credentials)

At local folder
### Docker swarm
```
docker stack deploy -c docker-compose.yml <stack-name>

```

### Kubernetes

```
kubectl apply -f ./

```