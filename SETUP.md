# Setup

## Steps

- Create a Kubernetes cluster on AWS using kops.
- Follow https://kubernetes.github.io/ingress-nginx/deploy/
  - Use L4 ELB for AWS
- Run `kubectl apply -f blog.yaml`
- Create an A record in Route53 mapping `mattjmcnaughton.com` to the
  ingress ELB. Create `CNAMEs` for `blog.mattjmcnaughton.com` and
  `www.mattjmcnaughton.com` pointing to that A record.

