# Install Metrics Server
*resource: https://blog.codewithdan.com/enabling-metrics-server-for-kubernetes-on-docker-desktop/*

Metrics Server is not installed by default. And then won't work due to TLS.

`helm repo add metrics-server https://kubernetes-sigs.github.io/metrics-server/`

`helm upgrade --install metrics-server metrics-server/metrics-server -f metrics-server-helm-values.yaml`

