# Demo 7 - Securing communication between OpenShift Clusters with Submariner in Advanced Cluster Management for Kubernetes

Repository for store the k8s resources in a GitOps way

* Check the [GitOps Repo](https://github.com/RedHat-EMEA-SSA-Team/ns-gitops/tree/seczones) to deploy this app with GitOps.

NOTE: All of this commands needs to be performed in the ACM Hub cluster to deploy through GitOps.

* Deploy the GuestBook App in cluster Managed 1

```
oc apply -k guestbook-app/acm-resources
```

* Deploy the Redis Master App in Cluster Managed 1

```
oc apply -k redis-master-app/acm-resources
```

* Deploy the Redis Slave App in Cluster Managed 2

```
oc apply -k redis-slave-app/acm-resources
```
