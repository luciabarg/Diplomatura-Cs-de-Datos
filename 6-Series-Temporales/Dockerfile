FROM jupyter/minimal-notebook

COPY conda-requirements.txt /home/$NB_USER/

USER $NB_UID

RUN conda config --system --prepend channels defaults && \
    conda install --yes --file conda-requirements.txt && \
    conda remove --yes --force qt pyqt && \
    conda clean -tipsy 

COPY . /home/$NB_USER/

RUN cd /home/$NB_USER/ && ./get-x13as.sh
ENV XDG_CACHE_HOME /home/$NB_USER/.cache/
RUN MPLBACKEND=Agg python -c "import matplotlib.pyplot" 
