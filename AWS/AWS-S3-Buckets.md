# AWS S3

- Amazon S3 is one of the main building blocks of AWS
- It's advertised as "infinitely scaling" storage

## Amazon S3 Use cases

- Backup and storage
- Disaster Recovery
- Archive
- Hybrid Cloud Storage
- Application hosting
- Media hosting
- Data lakes & big data analytics
- Software delivery
- Static website

## Amazon S3 Buckets

- Amazon S3 allows people tto store objects (files) in "buckets" (directories)
- Buckets must have a globally unique name (across all regions and all accounts)
- Buckets are defined at the region level
- S3 look like a global service but buckets are created in a region
- Naming convention:
  - No uppercase, No underscore
  - 3-63 characters long
  - ...

## Amazon S3 - Objects

- Objects (files) have a key
- The `key` is the __FULL__ path:
  - `s3://mybucket/my_file.txt`
  - `s3://my-bucket/my_folder/another_folder/my_file.txt`
- The key is composed of `prefix` + `object name`
  - s://my-bucket/my_folder/another_folder/my_file.txt
    - prefix: `my_folder/another_folder/`
    - object name: `my_file.txt`
