## Working with S3 storage

* When working via high-level AWS CLI tool remember the following points:

  * name that ends in a slash is a folder or a bucket all other names are filenames or key names inside the bucket
  
  * always use forward slash for S3 bucket paths, use whatever suits you for local OS paths
  
  * some commands work on folders/buckets only, so they ignore last slash anyway: *sync*, *mb*, *rb*, *ls*
  
  * long options starting with "--" can be shorten to the least recognizable, e.g. --recursive => --rec
  
* Include and Exclude filters for the names:

  * Wildcards supported: *, ?, [sequence], [!negated sequence]
  
  * any number of filters can be combined
  
  * if filters overlap in their action the latest in position on CLI wins
  
  * filters are evaluated against SOURCE directory. If an individual file name given, 
  the directory name containing this file is used instead
  
  * by default ALL files are included already, so giving just include filters without exclude does nothing
   
