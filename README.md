# CodeStream-K8s-Blog
The scripts and Pipeline source for the vSphere-vRA-Tanzu Blog

This content is assocaited to the blog post located at:  http://blogs.vmware.com/management/2020/08/v7-vra-tanzuv.html

In detail this blog will setup a vRealize Automation Cloud Code Stream pipeline that will create a Supervisor Namespace with an associated storage policy, deploy a Tanzu Kubernetes cluster in the namespace, and automatically set it up in Code Stream as an endpoint for use by other pipelines. All of this will then be added to Service Broker as a self-service catalog item with an approval policy attached.
