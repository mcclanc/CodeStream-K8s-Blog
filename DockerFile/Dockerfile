FROM ubuntu

LABEL maintainer "Chris McClanahan <mcclanahanc@vmware.com>"
LABEL description "Container with the vSphere K8s CLIs and TKG CLIs"

RUN apt update && \
    apt install -y wget && \
    apt install -y unzip && \
    apt install -y gzip && \
    apt install -y python3 && \
    apt install -y expect && \
    apt install -y curl && \
    apt install -y python3-pip && \
    pip3 install requests && \
    wget --no-check-certificate https://<Enter Supervisor Cluster IP>/wcp/plugin/linux-amd64/vsphere-plugin.zip && \
    unzip vsphere-plugin.zip && \
    rm vsphere-plugin.zip && \
    wget --no-check-certificate <Enter URL to TKG CLI Download Location> && \
    gzip -d tkg-linux-amd64-v1.1.2-vmware.1.gz && \
    mv tkg-linux-amd64-v1.1.2-vmware.1 /usr/local/bin/tkg && \
    chmod +x /usr/local/bin/tkg
