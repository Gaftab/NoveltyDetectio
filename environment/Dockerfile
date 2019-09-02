FROM registry.codeocean.com/codeocean/miniconda3:4.6.14-python3.7.3-ubuntu18.04

ARG DEBIAN_FRONTEND=noninteractive

RUN pip install --upgrade --no-cache-dir --upgrade-strategy=only-if-needed \
      numpy==1.17.1 \
      pandas==0.25.1 \
      sklearn==0.0

COPY postInstall /
RUN /postInstall
