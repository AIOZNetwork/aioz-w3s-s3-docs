# Getting Started

In this tutorial, we'll guide you through the fundamental steps of interacting with AIOZ W3S using AWS S3 SDK for Go. Let's get started!

## 1. Install the Dependencies

To install the project dependencies, simply run the following command in your terminal:

```bash
go get
```

## 2. Setup the Environment

We will be setting up two environment variables, `ACCESS_KEY` and `SECRET_KEY`, which are required to access the AIOZ W3S service. Assign the values of these variables to the values of your credential that you created in the [AIOZ W3S dashboard](https://w3s.storage/access-grants).

```bash
export ACCESS_KEY=<your-access-key>
export SECRET_KEY=<your-secret-key>
```

## 3. List all buckets

To list all buckets, you can use the following code:

```bash
go run main.go
```

To choose which other functions to run, you uncomment the function in `main.go`.
