## Add an object to the S3 storage setting its various parameters
- Add local file *index.html* to the bucket *yurisk.info* at the location */tag/nmap/* and
set website redirection to the http://yurisk.info, also set ACL to public read

`aws s3api put-object  --bucket yurisk.info --key /tag/nmap/index.html --website-redirect-location http://yurisk.info --body  C:/Users/yurisk.info/tag/nmap/index.html --acl public-read`
