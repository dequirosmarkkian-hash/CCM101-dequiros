# MinIO Deployment

## Deployment Overview

For this laboratory activity, I deployed MinIO as an S3-compatible object storage server using Docker in a KillerCoda Ubuntu Playground.

## Docker Command

The following Docker command was used to deploy the MinIO server:

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
-e "MINIO_ROOT_USER=cloudadmin" \
-e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
minio/minio server /data --console-address ":9001"
```

## Port Configuration

Two ports were mapped during deployment:

* **Port 9000** – MinIO API port
* **Port 9001** – MinIO Web Console

The web interface was accessed through port **9001**.

## Login Credentials

The environment variables configured the MinIO administrator account:

* Username: `cloudadmin`
* Password: `CloudNova2026!`

## Environment Variables

The `-e` flags are used to define environment variables inside the Docker container.

The following variables were used:

```text
MINIO_ROOT_USER=cloudadmin
MINIO_ROOT_PASSWORD=CloudNova2026!
```

`MINIO_ROOT_USER` defines the administrator username, while `MINIO_ROOT_PASSWORD` defines the administrator password.

## Storage Bucket

After accessing the MinIO Web Console, I created the following bucket:

```text
client-photos
```

I then uploaded a sample file into the bucket to verify that the object storage system was working correctly.

## Verification

I verified the deployment by checking that the `minio-server` Docker container was running. I also accessed the MinIO Web Console, created the `client-photos` bucket, and uploaded a sample file.

## Screenshots

### MinIO Deployment

![MinIO Deployment](screenshots/minio-deployed.png)

### Bucket and Uploaded File

![MinIO Bucket Upload](screenshots/minio-bucket-upload.png)
