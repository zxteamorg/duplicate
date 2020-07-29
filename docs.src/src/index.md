# Duplicate

Duplicate is opensource toolset to make continuous backup for your data.

Source data: Files, Directories, Block Devices
Storage Backends: Amazon Glacier, Google Cloud Coldline, B2 Cloud Storage

* `dupush` - Upload(push) your data to storage backend
* `dufetch` - Download(fetch) your data from storage backend

## Tools

### dupush

```
dupush --source=/dev/vg0/home-snaphot --target=gs://my-google-backup-bucket-1/home-snaphot-YYYYMMDD
```


## Similar projects

https://github.com/duplicati/duplicati
