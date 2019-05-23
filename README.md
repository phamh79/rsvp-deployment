# rsvp-deployment
## Local evn
Images are from Docker hub repo so make sure it is logged-in.
For Kubernetest, execute [follow this step](https://kubernetes.io/docs/tasks/configure-pod-container/pull-image-private-registry/#registry-secret-existing-credentials)

At local folder
#### Docker swarm
```
docker stack deploy -c docker-compose.yml <stack-name>
```

#### Kubernetes

```
kubectl apply -f ./
```
How to run on FE
#### Docker
Open browser @localhost:80

#### Kubernetes
- Load source code at [rsvp-react-client](https://github.com/phpppd/rsvp-react-client)
- Modify .env.development - REACT_APP_GATEWAY 's value to <Minikube's IP>:<rsvp-gateway's Port>

```
kubectl describe service rsvp-gateway
```
