# conda-singularity-docker

Contains anaconda and singularity 2.4.6. Used to run Snakemake w/ singularity on mac. Later versions of singularity will not run inside a container. You must run the image as follows, or singularity will complain.

```
docker run -it --privileged=True --cap-add=SYS_ADMIN samesense/conda-singularity-docker
```
