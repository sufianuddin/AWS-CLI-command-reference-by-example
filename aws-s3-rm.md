## Delete S3 object

- Simulate running the command without deleting anything:

`aws s3 rm s3://yurisk.info --dryrun --rec`

- Delete recursively contents of a bucket, bucket itself is not deleted (read further):

`aws s3 rm s3://yurisk.info --recursive`

- Delete recursively all files in a bucket except JPEG and PNG:

`aws s3 rm s3://yurisk.info --recursive --exclude "*.jpg"  exclude "*.png" `

- Delete only files with a given extension (here JPG):

`aws s3 rm s3://yurisk.info --recursive --exclude "*" include "*.jpg"`

- Delete an empty bucket:

`aws s3api delete-bucket --bucket yurisk.info`

