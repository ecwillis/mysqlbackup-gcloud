#mysqlbackup-gcloud

A simple docker container to backup a mysql db to google cloud storage.  Easy to integrate with cron.

## Usage

### Backup

```
docker run --rm --link mysql:mysql --env BUCKET=bucket --env DB=db --env PREFIX=backup -v /path/to/key/dir:/app firstandthird/mysqlbackup-s3
```
