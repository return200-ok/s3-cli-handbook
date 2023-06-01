# s3-cli-handbook

Synopsis
```
aws s3 <Command> [<Arg> ...]
```
Available Commands

    cp
    ls
    mb
    mv
    presign
    rb
    rm
    sync
    website

## Top AWS S3 CLI Commands

1. Create a New S3 Bucket
```
$ aws s3 mb s3://tgsbucket
make_bucket: tgsbucket
```
2. Delete an S3 Bucket

Make use of the rb option. Remove bucket is referred to as rb.

The provided bucket is deleted by the next command:
```
$ aws s3 rb s3://tgsbucket
remove_bucket: tgsbucket
```
Use the -force option as illustrated below to remove a bucket and all of its items:
```
$ aws s3 rb s3://tgsbucket --force
delete: s3://tgsbucket/demo/getdata.php
delete: s3://tgsbucket/ipallow.txt
delete: s3://tgsbucket/demo/servers.txt
delete: s3://tgsbucket/demo/
remove_bucket: tgsbucket
```
3. List bucket
```
 aws s3 ls --endpoint-url=
```
4. List file from bucket
```
aws s3 ls --endpoint-url=https:// s3://bucket_name --recursive --human-readable --summarize
```
5. Push to bucket
```
aws s3 cp 
```

