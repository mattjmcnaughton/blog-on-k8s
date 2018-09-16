# blog-on-k8s

This project contains the code necessary to run my
[blog](https://github.com/mattjmcnaughton/blog) on Kubernetes.
I plan to use it as a "test" application for Kubernetes.

## Steps

- Create a Kubernetes cluster on AWS using kops. Follow my [A Kubernetes of
  One's Own Series](http://mattjmcnaughton.com/post/a-kubernetes-of-ones-own-part-0/)
  for step by step instructions.
- Run `kubectl apply -f blog.yaml` to create the deployment and service.
- Create an A record in Route53 mapping `YOURDOMAIN.com` to the
  service ELB.
