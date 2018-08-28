# kubeguestbook
Kube guestbook on OpenShift

# Deploy Reddis and wait for the pod status to become ready (1/1)

```
oc new-app docker.io/kubeguide/redis-master
```

# Deploy the guestbook and wait for the pod status to become ready (1/1)

```
oc new-app docker.io/kubernetes/guestbook
```

# Create a route by exposing the guestbook service

``
oc expose service guestbook
```

# Visit the app at hostname that is returned. 

```
oc get route
```
