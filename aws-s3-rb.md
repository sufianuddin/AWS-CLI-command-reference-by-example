## Delete a bucket

- Delete an empty bucket, if it is not empty fails with the error *BucketNotEmpty*:

`aws s3 rb yurisk.info`

- Force deleting non empty bucket provided that objects in it have not been versioned:

`aws s3 rb s3://yurisk.com  --force`

- Look at https://github.com/yuriskinfo/AWS-CLI-command-reference-by-example/blob/master/aws-s3-rm.md for emptying the bucket
