# Create a bucket
```shell
aws s3 mb s3://prefixes-sope-123
```

# Create a folder within the bucket

```shell
#This creates a folder hello
aws s3api put-object --bucket="prefixes-sope-123" --key="hello/"
```

