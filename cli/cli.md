# Using AIOZ W3S with AWS CLI

In this document, we will show you how to use AIOZ W3S with AWS CLI.

## Table of Contents

1. [Prerequisites](#prerequisites)
2. [Create a bucket](#create-a-bucket)
3. [List buckets](#list-buckets)
4. [List objects](#list-objects)
5. [Upload object](#upload-object)
6. [Get object](#get-object)
7. [Delete object](#delete-object)
8. [Delete multiple objects](#delete-multiple-objects)
9. [Delete bucket](#delete-bucket)
10. [Copy object](#copy-object)

## Prerequisites

Before you can use AIOZ W3S with AWS CLI, you must install the AWS CLI and configure it.

1. [Install AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-install.html)
2. [Configure AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-configure.html)

After you have installed and configured AWS CLI, the following sections show you how to use it. For completed examples, see the [AWS CLI S3 examples](https://docs.aws.amazon.com/cli/latest/userguide/cli-services-s3-commands.html).

## Create a bucket

```bash
aws s3 --endpoint-url https://s3-beta.aioz.storage mb s3://my-bucket
```

## List buckets

```bash
aws s3 --endpoint-url https://s3-beta.aioz.storage ls
```

## List objects

```bash
aws s3 --endpoint-url https://s3-beta.aioz.storage ls s3://bucket-name
```

## Upload object

```bash
aws s3 --endpoint-url https://s3-beta.aioz.storage cp /path/to/file s3://bucket-name
```

## Get object

```bash
aws s3 --endpoint-url https://s3-beta.aioz.storage cp s3://bucket-name/file /path/to/file
```

## Delete object

```bash
aws s3 --endpoint-url https://s3-beta.aioz.storage rm s3://bucket-name/file
```

## Delete multiple objects

This command will delete all objects in the bucket `bucket-name`.

```bash
aws s3 --endpoint-url https://s3-beta.aioz.storage rm s3://bucket-name/ --recursive
```

## Delete bucket

```bash
aws s3 --endpoint-url https://s3-beta.aioz.storage rb s3://bucket-name
```

## Copy object

```bash
aws s3 --endpoint-url https://s3-beta.aioz.storage cp s3://bucket-name/file s3://bucket-name/file
```

