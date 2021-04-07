# Build the manager binary
FROM quay.io/operator-framework/helm-operator:v1.3.0
LABEL name="Citrix adc istio ingress gateway Operator" \
      vendor="Citrix" \
      version="v0.9.5" \
      release="1" \
      summary="This is Citrix adc istio ingress gateway helm operator." \
      description="This operator will deploy Citrix adc istio ingress gateway to the cluster."

COPY licenses /licenses

ENV HOME=/opt/helm
COPY watches.yaml ${HOME}/watches.yaml
COPY helm-charts  ${HOME}/helm-charts
WORKDIR ${HOME}
