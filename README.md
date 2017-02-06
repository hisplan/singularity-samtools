# singularity-samtools

Singularity for samtools

## Prerequisites

- Singularity 2.2 must be installed on your system. [Here](http://singularity.lbl.gov/docs-quick-start-installation) is the instruction. 

## Build

1. Download `Singularity` file from this git repository.

1. Create a 200MB empty image:

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

## Notes

- This uses Alpine Linux as base image.
