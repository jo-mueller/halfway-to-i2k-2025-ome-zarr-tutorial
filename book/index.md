# Halfway to I2K 2025: OME-ZARR basics
(tutorial:main)=

Welcome to the guide pages for the OME-ZARR basics workshop.
To prepare for the course, please follow the instructions below.

## Installation

If you haven't already installed Python on your device, 
please do so by following the [instructions](https://github.com/conda-forge/miniforge?tab=readme-ov-file#requirements-and-installers)
for your respective platform.

Next, we are going to create a separate Python environment for the stuff we need in this course.
To do so, install [uv](https://docs.astral.sh/uv/), which is our package manager of choice for this course:

```bash
pip install uv
```

Next, clone this repository and its contents:

```bash
git clone https://github.com/jo-mueller/halfway-to-i2k-2025-ome-zarr-tutorial.git
cd halfway-to-i2k-2025-ome-zarr-tutorial
```

Then, create a new virtual environment to separate this course's dependencies from your other Python projects:

```bash
uv venv
```

Use the appropriate command for your operating system:

````{tab-set}
```{tab-item} Windows
```bash
.venv\Scripts\activate
```

```{tab-item} macOS/Linux
```bash
source .venv/bin/activate
```
````

Lastly, install everything needed for the workshop:

```bash
uv pip install -e .
```

Open Jupyter lab to interact with the provided notebooks like this:

```bash
jupyter lab
```

That's it - you're good to go!

## Contents

We will do three basic things in this course:

- [Generate some ome-zarr data](tutorial:create_ome_zarr): Write some Python code to convert microscopy data into the OME-ZARR format.
- [Upload the data to cloud storage](tutorial:upload_to_cloud): Upload the generated OME-ZARR data to an S3-compatible cloud storage service.
- [View the data from the web](tutorial:view_from_web): Use a web-based viewer to access and visualize the data directly from the cloud.