FROM alpine

ENV KUSTOMIZE_VERSION 3.7.0

ADD https://github.com/kubernetes-sigs/kustomize/releases/download/kustomize%2Fv${KUSTOMIZE_VERSION}/kustomize_v${KUSTOMIZE_VERSION}_linux_amd64.tar.gz /tmp/

RUN tar -xvf /tmp/kustomize_v${KUSTOMIZE_VERSION}_linux_amd64.tar.gz -C /usr/local/bin/ && \
    chmod +x /usr/local/bin/kustomize

ENTRYPOINT [ "kustomize" ]
