# Use AIOZ W3S with Postman

In this document, we will show you how to use AIOZ W3S with Postman.

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

Before you can use AIOZ W3S with Postman, you must install Postman and configure it.

1. [Install Postman](https://www.postman.com/downloads/)
2. Configure credentials.

- Create a new request.
- In Authorization tab, select AWS Signature.
- Fill in the Access Key and Secret Key fields.
- In Advanced settings, fill in the Service Name field with `s3` and the Region field with `us-east-1`.

After you have installed and configured Postman, the following sections show you how to use it. For completed examples, see the [Amazon S3 API Reference](https://docs.aws.amazon.com/AmazonS3/latest/API/Type_API_Reference.html).

## Create a bucket

```http
PUT / HTTP/1.1
Host: s3-beta.aioz.storage/bucket-name

```

## List buckets

```http
GET / HTTP/1.1
Host: s3-beta.aioz.storage

```

## List objects

```http
GET /bucket-name HTTP/1.1
Host: s3-beta.aioz.storage
```

## Upload object

```http
PUT /bucket-name/object-name HTTP/1.1
Host: s3-beta.aioz.storage

```

## Get object

```http
GET /bucket-name/object-name HTTP/1.1
Host: s3-beta.aioz.storage

```

## Delete object

```http
DELETE /bucket-name/object-name HTTP/1.1
Host: s3-beta.aioz.storage

```

## Delete multiple objects

```http
POST /?delete HTTP/1.1
Host: s3-beta.aioz.storage
  
```

## Delete bucket

```http
DELETE /bucket-name HTTP/1.1
Host: s3-beta.aioz.storage

```

## Copy object

```http
PUT /dest-bucket-name/dest-object-name HTTP/1.1
Host: s3-beta.aioz.storage
x-amz-copy-source: /bucket-name/object-name

```

