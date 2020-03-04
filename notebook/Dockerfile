FROM jupyter/minimal-notebook:latest

MAINTAINER Frank Roeder "piperly@icloud.com"

ENV JUPYTER_ENABLE_LAB yes


COPY requirements.txt /tmp/
RUN pip install --requirement /tmp/requirements.txt && \
    fix-permissions $CONDA_DIR && \
    fix-permissions /home/$NB_USER

COPY jupyter_notebook_config.py /etc/jupyter/
# Fix permissions on /etc/jupyter as root
USER root
RUN fix-permissions /etc/jupyter/

USER $NB_UID
