FROM biocontainers/biocontainers:vdebian-buster-backports_cv1
MAINTAINER biocontainers <biodocker@gmail.com>
LABEL    software="relion-bin-plusmpi" \ 
    base_image="biocontainers/biocontainers:vdebian-buster-backports_cv1" \ 
    container="relion-bin-plusmpi" \ 
    about.summary="parallel toolkit for 3D reconstructions in cryo-electron microscopy" \ 
    about.home="http://www2.mrc-lmb.cam.ac.uk/relion/index.php/Main_Page" \ 
    software.version="1.4dfsg-4-deb" \ 
    upstream.version="1.4" \ 
    version="1" \ 
    about.copyright="2014, Sjors Scheres at the MRC Laboratory of Molecular Biology" \ 
    about.license="GPL-2+" \ 
    about.license_file="/usr/share/doc/relion-bin-plusmpi/copyright" \ 
    extra.binaries="/usr/bin/relion_autopick,/usr/bin/relion_autopick_mpi,/usr/bin/relion_find_tiltpairs,/usr/bin/relion_image_handler,/usr/bin/relion_mask_create,/usr/bin/relion_particle_polish,/usr/bin/relion_particle_polish_mpi,/usr/bin/relion_particle_sort,/usr/bin/relion_particle_sort_mpi,/usr/bin/relion_postprocess,/usr/bin/relion_preprocess,/usr/bin/relion_preprocess_mpi,/usr/bin/relion_project,/usr/bin/relion_reconstruct,/usr/bin/relion_refine,/usr/bin/relion_refine_mpi,/usr/bin/relion_run_ctffind,/usr/bin/relion_run_ctffind_mpi,/usr/bin/relion_stack_create,/usr/bin/relion_star_compare,/usr/bin/relion_star_datablock_ctfdat,/usr/bin/relion_star_datablock_singlefiles,/usr/bin/relion_star_datablock_stack,/usr/bin/relion_star_loopheader,/usr/bin/relion_star_plottable,/usr/bin/relion_star_printtable,/usr/bin/relion_tiltpair_plot,/usr/bin/relion_autopick,/usr/bin/relion_autopick_mpi,/usr/bin/relion_find_tiltpairs,/usr/bin/relion_image_handler,/usr/bin/relion_mask_create,/usr/bin/relion_particle_polish,/usr/bin/relion_particle_polish_mpi,/usr/bin/relion_particle_sort,/usr/bin/relion_particle_sort_mpi,/usr/bin/relion_postprocess,/usr/bin/relion_preprocess,/usr/bin/relion_preprocess_mpi,/usr/bin/relion_project,/usr/bin/relion_reconstruct,/usr/bin/relion_refine,/usr/bin/relion_refine_mpi,/usr/bin/relion_run_ctffind,/usr/bin/relion_run_ctffind_mpi,/usr/bin/relion_stack_create,/usr/bin/relion_star_compare,/usr/bin/relion_star_datablock_ctfdat,/usr/bin/relion_star_datablock_singlefiles,/usr/bin/relion_star_datablock_stack,/usr/bin/relion_star_loopheader,/usr/bin/relion_star_plottable,/usr/bin/relion_star_printtable,/usr/bin/relion_tiltpair_plot" \ 
    about.tags=""

USER root
ENV DEBIAN_FRONTEND noninteractive
RUN apt-get update && (apt-get install -t buster-backports -y relion-bin+mpi || apt-get install -y relion-bin+mpi) && apt-get clean && apt-get purge && rm -rf /var/lib/apt/lists/* /tmp/*
USER biodocker
