# Build the manager binary
FROM registry.redhat.io/openshift4/ose-helm-operator:v4.8.0

LABEL name="Citrix-cpx-istio-sidecar-injector-operator" \
      vendor="Citrix" \
      version="v0.9.9" \
      release="1" \
      summary="This is Citrix cpx istio sidecar injector operator helm operator." \
      description="This operator will deploy Citrix cpx istio sidecar injector to the cluster."

COPY licenses /licenses


ENV HOME=/opt/helm
COPY watches.yaml ${HOME}/watches.yaml
COPY helm-charts  ${HOME}/helm-charts
WORKDIR ${HOME}
