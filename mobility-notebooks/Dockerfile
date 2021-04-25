FROM jupyter/base-notebook
# Install from requirements.txt file
COPY --chown=${NB_UID}:${NB_GID} requirements_conda.txt /tmp/
RUN conda install --yes --file /tmp/requirements_conda.txt && \
    fix-permissions $CONDA_DIR && \
    fix-permissions /home/$NB_USER
    
COPY --chown=${NB_UID}:${NB_GID} requirements_pip.txt /tmp/
RUN pip install --requirement /tmp/requirements_pip.txt && \
    fix-permissions $CONDA_DIR && \
    fix-permissions /home/$NB_USER
