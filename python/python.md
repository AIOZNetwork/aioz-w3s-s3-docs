# Getting Started

In this tutorial, we'll guide you through the fundamental steps of interacting with AIOZ W3S using AWS S3 SDK for Python. Let's get started!

## 1. Install the dependencies

Before using AIOZ W3S, it is necessary to install the required dependencies. In this tutorial, we will be using [Poetry](https://python-poetry.org/) to handle the Python dependencies. So you need to install Poetry first as [this tutorial](https://python-poetry.org/docs/#installation). After you installed Poetry, to install the project dependencies, simply run the following command in your terminal:

```bash
poetry install 
poetry shell
```

## 2. Setup the environment

We will be setting up two environment variables, `ACCESS_KEY` and `SECRET_KEY`, which are required to access the AIOZ W3S service. Assign the values of these variables to the values of your credential that you created in the [AIOZ W3S dashboard](https://dashboard-beta.aioz.storage/access).

```bash
export ACCESS_KEY=<your-access-key>
export SECRET_KEY=<your-secret-key>
```

## 3. List all buckets

To list all buckets, you can use the following code:

```bash
python list_buckets.py
```

Other functionalities are straightforward and follow a similar pattern. You can check out the code example repository for a comprehensive understanding.
