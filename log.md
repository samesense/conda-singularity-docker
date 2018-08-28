### 2018_08_28
* Sigularity will fail later b/c of tar. This is a fix, but is screws up apt-get. `RUN apt-get install -y bsdtar && ln -sf $(which bsdtar) $(which tar)` It should be added to the final image.
* Perhaps any docker container w/ a Dockerfile does not have this issue.
* tar issue: https://github.com/singularityware/singularity/issues/1570
