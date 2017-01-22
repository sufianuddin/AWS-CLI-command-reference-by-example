##Enable existing S3 bucket for static website hosting

- Set existing S3 bucket *mywebsite* for hosting the website with default served document being *index.html* and error page for any 4xx error codes
being *error.html*

`aws s3 website s3://mywebsite/ --index-document index.html --error-document error.html`

- Make sure HTML pages of the bucket are accessible by anyone for reading, for settings see https://github.com/yuriskinfo/AWS-CLI-command-reference-by-example/blob/master/aws-s3-cp.md or https://github.com/yuriskinfo/AWS-CLI-command-reference-by-example/blob/master/aws-s3-sync.md

