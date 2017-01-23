## List S3 objects, buckets and/or their contents

- Get a list of all the buckets under user account:

`aws s3 ls`

- Recursively list contents of a given bucket *yurisk.info*:

`aws s3 ls yurisk.info --recursive`

- Recursively list contents of a given bucket printing sizes in a friendly format:

`aws s3 ls yurisk.com --recursive --human`

- List contents of a bucket, add summary for number of objects and their total size:

`aws s3 ls  yurisk.info --summarize --human`

- Get access-list associated with the bucket provided you have permissions to do so on this bucket:

`aws s3api get-bucket-acl --bucket yurisk.info`
