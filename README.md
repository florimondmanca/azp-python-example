# azp-python-example

Example Python package published to [TestPyPI](https://test.pypi.org/) on tags using Azure Pipelines.

## Usage

Setup (do it once):

- Fork this repository.
- Edit the package name in `setup.py` to something unique to you, e.g. `<USERNAME>-example`.
- Set up the `pypi-credentials` variable group:
  - In Azure Pipelines, go to your project, then "Library" (under Pipelines), then "Add variable group".
  - Name it `pypi-credentials`.
  - Create an API token on TestPyPI, then add it as a secret `pypiTestToken` variable to the variable group.
  - Save the variable group.
- Create the pipeline for your repository, then run it.

Release your first version:

- In GitHub, create a new release for your repository, tagged as `0.0.1`.
- The pipeline will run again, and your package will soon be uploaded to TestPyPI.
