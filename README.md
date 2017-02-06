# singularity-samtools

Singularity for samtools

## Prerequisites

- Singularity 2.2 must be installed on your system. [Here](http://singularity.lbl.gov/docs-quick-start-installation) is the instruction. 

## Build

1. Download `Singularity` file from this git repository.

1. Create an empty container image of 200MB:

    ```bash
    $ sudo singularity create -s 200 samtools.img
    ```

1. Bootstrap the image using the `Singularity` image definition file you downloaded from the previous step:

    ```bash
    $ sudo singularity bootstrap samtools.img Singularity
    ```

## Run

```bash
$ singularity run samtools.img --help
```

## Other Notes

- This uses Alpine Linux as base image.
- Note that the image definition file being used here contains a bunch of commands that downloads and compiles the source code of samtools, which is the main reason why the container image requires about 200MB. It would be nice if Singularity provides a way to shrink the image down to the only necessary size. Another workaround would be `Dockerfile`.