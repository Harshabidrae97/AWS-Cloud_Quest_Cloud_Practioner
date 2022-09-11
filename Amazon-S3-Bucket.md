1 - The AWS Management Console is a web interface to access and manage the broad collection of services provided by Amazon Web Services.

2 - A bucket is a container for objects stored in Amazon S3. 
    Every object is contained in a bucket. 
    You can configure buckets so that they are created in a specific AWS Region.

3 - An Amazon S3 bucket name is globally unique, and the namespace is shared by all AWS accounts.
    After a bucket is created, the name of that bucket cannot be used by another AWS account in any AWS Region until the bucket is deleted .
    
4 - By default, new buckets, access points, and objects don't allow public access.
    However, users can modify bucket policies, access point policies, or object permissions to allow public access.
    Amazon S3 Block Public Access settings override these policies and permissions so that you can limit public access to these resources.
    
5 - By default, data is not encrypted in your Amazon S3 bucket.
    It is a best practice to encrypt your data either on the client side or through the Amazon S3 server side encryption options.
    
6 - You can access your bucket using the Amazon S3 console.
    Using the console UI, you can perform almost all bucket operations without having to write any code.
    
7 - Your data stored in Amazon S3 is referred to as an object.
    An object is a file and any metadata that describes that file.
    Amazon S3 stores files in a manner that the contents of your files are unreaed by Amazon S3.
    The metadata is a set of key-vaule pairs that describe the object.
    
8 - A key is the unique identifier for an object within a bucket.
    Every object in a bucket has exactly one key.
    The combination of a bucket, key, and version ID uniquely identifies each object.
    Amazon S3 is like a data map between "bucket + key + version" and the object itself.
    Every object in Amazon S3 can be uniquely addressed throught the combination of the web service endpoint, bucket name, key, and optionally, a version.
    
9 - Amazon S3 supports an unlimited number of objects of any file type such as images, text and audio files.

10 - You can host a static website using Amazon S3 by configuring your bucket for static webiste hosting, setting permissions, and adding an index document.
     Options like redirects, logging and error documents are also available.
     
11 - By default, all Amazon S3 resources (buckets, objects, and related subresources) are private and only the resource owners can access it.
     The resource owner can optionally grant access permissions to others by writing an access policy.
     
12 - Bucket policy and user policy are two of the access policy options available for you to grant permission to your Amazon S3 resources.
     Both use JSON-based access policy language.
     An Amazon Resource Name (ARN) uniquely identifies AWS resources.
     
13 - With Amazon S3, you can upload objects up to 5GB in size with a single put operation.
     For larger objects up to 5TB in size, use the multipart upload API.
 
 
 
 
 
 
 
 
 
 
 
 
