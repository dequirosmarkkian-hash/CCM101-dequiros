# Mission Reflection

This laboratory activity helped me understand why object storage is commonly used for applications that need to manage large amounts of unstructured data. Object storage is better suited for storing millions of photos because images can be stored as individual objects with associated metadata inside buckets. Unlike traditional block storage, object storage is designed to handle large collections of files and can be accessed by applications through web-based interfaces and APIs.

Docker made deploying the MinIO storage server easier because I did not have to manually install and configure every component of the storage software. By using a Docker command, I was able to download the MinIO image, create a container, configure the required ports, and provide the administrator credentials through environment variables. This made the deployment process more organized and repeatable.

A bucket is a storage container used to organize objects in object storage. In this laboratory, I created a bucket named `client-photos` and uploaded a sample file to demonstrate that the storage server was working correctly.

Large enterprise companies can protect object storage data from physical server failures by using redundancy, replication, backups, and geographically distributed storage systems. These techniques can help ensure that copies of important data remain available even when individual hardware or storage systems fail.

My confidence in using the Linux command line is also improving. Running Docker commands and checking the status of the MinIO container gave me more experience working with a Linux-based environment. I learned that command-line tools can make cloud deployment tasks faster and more manageable. Overall, this activity helped me connect Docker, Linux, cloud storage, and GitHub documentation into one practical cloud computing workflow.
