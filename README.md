#mysqlbackup-gcloud

A simple docker container to backup a mysql db to google cloud storage.  Easy to integrate with cron.

## Usage

You must have a google cloud service key available to use. Place the key in a volume named key.json.

### Backup

```
docker run --rm --link mysql:mysql --env BUCKET=bucket --env DB=db --env PREFIX=backup -v /path/to/key/dir:/app firstandthird/mysqlbackup-s3
```
