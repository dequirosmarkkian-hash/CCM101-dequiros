# Storage Types Research

## Comparison of Cloud Storage Types

| Storage Type       | Description                                                                                                                                               | Primary Use Case                                                                                       | Cloud Provider Example        |
| ------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------ | ----------------------------- |
| **Block Storage**  | Stores data in fixed-size blocks that can be managed individually. The blocks can be attached to virtual machines and used like a traditional hard drive. | Best for operating systems, databases, and applications that require fast and consistent disk access.  | AWS Elastic Block Store (EBS) |
| **File Storage**   | Stores data as files organized into folders and directories. Multiple systems can access the same file system over a network.                             | Best for shared files, documents, content management, and applications that need a shared file system. | AWS Elastic File System (EFS) |
| **Object Storage** | Stores data as objects together with metadata and a unique identifier. Objects are stored inside containers called buckets.                               | Best for large amounts of unstructured data such as images, videos, backups, and documents.            | Amazon S3                     |

## Why Object Storage Is Suitable for the Client

Object Storage is suitable for the client's photo-sharing application because it is designed to store large amounts of unstructured data such as images. It can organize files as objects inside buckets and is well suited for applications that need scalable access to many uploaded files.

